# Chapter 8: Implementation Support — From Hardware to User Interface

## The Big Picture

Previous chapters covered *what* to design, *who* to design for, and *what rules* to follow. This chapter covers the **technical infrastructure** that makes UI implementation possible. The story is one of **increasing abstraction** — moving from raw hardware management up to conceptual architectures that separate the UI from the application logic.

```
                     Higher abstraction
                           ↑
              ┌─────────────────────┐
              │  UIMS / Architectures │  ← Conceptual separation
              │  (Seeheim, MVC, PAC)  │
              ├─────────────────────┤
              │  Interaction Toolkits │  ← Pre-built widgets
              │  (Swing, AWT, Qt)     │
              ├─────────────────────┤
              │  Windowing Systems    │  ← Device independence
              │  (X11, Windows, macOS)│
              ├─────────────────────┤
              │  Programming Paradigms│  ← How input is handled
              │  (Event loop, Callbacks)│
              └─────────────────────┘
                     ↓
                     Hardware
```

---

## 1. THE FOUNDATION — WINDOWING SYSTEMS

### The Problem

Before windowing systems, each application controlled the entire screen. You couldn't run multiple apps at once, and every developer had to write hardware-specific code.

### What a Windowing System Does

1. **Device independence** — provides an abstract interface to screens, keyboards, and mice. Developers write once; the windowing system talks to different device drivers.
   - Image models: pixels, PostScript, GKS, PHIGS
2. **Resource sharing** — multiple applications can run simultaneously in their own windows, isolated from each other.

### Architecture: Three Approaches

| Approach | How It Works | Portability |
|----------|-------------|-------------|
| Each app manages itself | Every app handles window synchronization | Poor |
| OS kernel manages | Windowing built into the OS | Moderate (tied to OS) |
| **Separate process manages** | A dedicated window manager handles everything | **Best** |

### The Client-Server Architecture (The Winner)

```
Client Apps (1..n)
    ↓
  Abstract Terminals (one per client)
    ↓
  Server (Resource Manager)
    ↓
  Device Driver
    ↓
  Keyboard / Mouse / Screen
```

**X Windows (X11)** is the canonical example:
- Application clients → X11 server → device drivers → hardware
- **Window manager is a separate client** — enforces policies (focus, tiling vs. overlapping, inter-client communication)
- Uses X protocol for server-client communication
- Pixel-based imaging model

---

## 2. PROGRAMMING THE APPLICATION — Two Paradigms for Handling Input

Before widgets and frameworks, you had to write the input-handling loop yourself. Two approaches emerged:

### Paradigm 1: Read-Evaluation Loop

```
repeat
  read-event(myevent)
  case myevent.type
    type_1: do processing
    type_2: do processing
    ...
  end case
end repeat
```

**Flow**: start → read input → process → quit? → end

**Good for**: modal dialogs (just nest another loop)
**Bad for**: complex UIs with many event types (switch gets huge)

### Paradigm 2: Notification-Based (Callbacks)

```java
menu.setAction("Save", mySave);
menu.setAction("Quit", myQuit);
// Notifier dispatches events to callbacks
```

**Flow**: register callbacks → notifier reads input → dispatches to appropriate handler

**Good for**: non-modal interfaces (just add another handler)
**Bad for**: modal dialogs (need mode flags everywhere)

### The Warning: "Going with the Grain"

Your framework's paradigm **biases** what's easy and what's hard:

| If you use... | Modal dialogs are | Non-modal dialogs are |
|---------------|-------------------|----------------------|
| Event loop | Easy (nested loop) | Hard (complex main loop) |
| Callbacks | Hard (mode flags) | Easy (add handler) |

**Don't let implementation drive design** — choose the paradigm that fits your interaction, not the other way around.

---

## 3. INTERACTION TOOLKITS — Pre-Built Widgets

### The Problem

Raw windowing systems give you pixels and events. Every button requires you to: detect mouse enter → draw highlight → detect click → draw pressed → detect release → fire action. That's tedious and error-prone.

### The Solution

**Toolkits** provide **interaction objects** (widgets/gadgets) that bundle input and output into reusable components:

```java
Button saveBtn = new Button("Save");
saveBtn.onClick(() -> saveFile());
```

### Benefits

- Programming at the level of **user perception** (buttons, menus, sliders) rather than pixels
- **Consistency** — same look and feel across applications
- **Generalizability** — same widget works everywhere
- Amenable to **object-oriented programming**

### Example: Java AWT & Swing

| Toolkit | Built on | Paradigm | Architecture |
|---------|----------|----------|-------------|
| **AWT** | Native platform | Notification-based (1.0: subclass, 1.1+: callbacks) | Abstract Windowing Toolkit |
| **Swing** | AWT | Notification-based | Higher-level, uses MVC |

---

## 4. UIMS — User Interface Management Systems

### The Problem

Toolkits are still too low-level for **non-programmers**. Also, the application logic (what the app does) gets tangled with the presentation (how it looks), making it hard to change either independently.

### The Solution

**UIMS** sits above toolkits and enforces a **separation** between application semantics and presentation.

### Benefits of Separation

| Benefit | What It Means |
|---------|---------------|
| **Portability** | Same app runs on different systems (swap presentation layer) |
| **Reusability** | Presentation or functionality reused across projects |
| **Multiple interfaces** | Same functionality, different UIs (desktop, mobile, web) |
| **Customizability** | Designers and users can modify the UI without touching code |

### UIMS Concerns

1. **Conceptual architecture** — how to think about UI structure
2. **Implementation techniques** — how to build it (state machines, event languages, constraints)
3. **Support infrastructure** — tools and environments (Visual Basic, Interface Builder)

### Related Terms

- **UIDS** — User Interface Development System (focus on tooling)
- **UIDE** — User Interface Development Environment (both UIMS + UIDS, e.g., Visual Basic)

---

## 5. THE SEEHEIM MODEL — The Classic UIMS Architecture

### Three Layers

```
Presentation (lexical — what users see & touch)
      ↔
Dialogue Control (syntactic — flow & sequencing)
      ↔
Functionality / Application Interface (semantic — what the app does)
```

| Layer | Handles | Analogy |
|-------|---------|---------|
| **Presentation** | Rendering, input events | The "look" |
| **Dialogue Control** | Sequencing, valid transitions | The "conversation" |
| **Functionality** | Actual computation | The "work" |

### The Switch

A direct communication path between Presentation and Functionality, bypassing Dialogue Control. Needed for **rapid semantic feedback** (e.g., highlighting a file icon when dragged over a folder — the app needs to respond before dialogue flow allows it). The switch is an **implementation necessity**, not a conceptual ideal.

### Feedback Levels

| Level | Example | Speed |
|-------|---------|-------|
| **Lexical** | Mouse movement | Fast |
| **Syntactic** | Menu highlights | Medium |
| **Semantic** | Sum of numbers changes | Slowest (needs switch for speed) |

---

## 6. ARCH/SLINKY — Refining Seeheim

### Five Layers Instead of Three

```
Physical → Lexical → Dialogue → Functional Core Adaptor → Functional Core
```

| Added Layer | Purpose |
|-------------|---------|
| **Physical** | Separates raw hardware from presentation |
| **Functional Core Adaptor (FCA)** | Adapts app's internal API for the dialogue layer |

### The "Slinky" Analogy

Like a slinky spring, any layer can be **thicker** (more complex) depending on the system:
- Drawing app → thick Physical/Lexical (complex rendering)
- Form app → thick Dialogue (complex navigation)
- Database app → thick FCA (complex data adaptation)

---

## 7. MVC — Model-View-Controller

### The Components

| Component | Role |
|-----------|------|
| **Model** | Internal state / data / logic |
| **View** | Screen rendering (output) |
| **Controller** | Input processing |

### Idealized Flow

```
Input → Controller → Model → View → Output
```

### The Problem

In graphical interfaces, **input only has meaning in relation to output**. A mouse click at (x,y) is meaningless without knowing *what* was drawn at (x,y). The Controller doesn't know that — the View does. So the Controller **talks to the View** in practice, violating the clean separation.

**Result**: MVC is cleaner in theory than in practice. But it's the most widely used model (Java Swing, Rails, iOS).

---

## 8. PAC — Presentation-Abstraction-Control

### The Components

| Component | Role |
|-----------|------|
| **Abstraction** | Logical state of component (like Model) |
| **Presentation** | Manages both input and output (unlike MVC's split) |
| **Control** | Mediates between them |

### PAC vs. MVC

| Dimension | MVC | PAC |
|-----------|-----|-----|
| Input/Output | Split (Controller + View) | Unified (Presentation) |
| Hierarchy | Flat | Hierarchical (Control objects communicate) |
| Practical use | More common | Cleaner separation but less used |

PAC is closer to Seeheim in spirit. MVC is more common in practice.

---

## 9. IMPLEMENTATION TECHNIQUES FOR UIMS

### How Do You Actually Build the Dialogue Controller?

| Technique | How It Works |
|-----------|-------------|
| **Menu networks** | Navigate through menus and screens |
| **State transition diagrams** | Formal states and transitions |
| **Grammar notations** | Define valid sequences like a language |
| **Event languages** | Reactive event-driven code |
| **Declarative languages** | Say *what*, not *how* |
| **Constraints** | Say what should be *true*, not what should *happen* |
| **Graphical specification** | Draw the UI, link to code (Visual Basic, Dreamweaver) |

### Constraints — A Special Note

Instead of programming what *happens* step by step, you declare what should *always be true*. The system maintains the constraint. Example: "the OK button is enabled only when all required fields are filled." Used in groupware (ALV — Abstraction-Link-View).

### Graphical Specification — The Most Popular Approach

In practice, most UIs are built by **drawing components on screen** and **linking actions** via scripts or code (Visual Basic, Dreamweaver, Flash). Its limitation: hard to "see" the overall paths through the system — focus is on individual screens.

---

## 10. THE DRIFT OF DIALOGUE CONTROL

Dialogue control has shifted across three levels over time:

| Level | Where Control Lives | Example |
|-------|-------------------|---------|
| **Internal control** | Within the application code | Read-evaluation loop |
| **External control** | Separate from semantics/presentation | UIMS dialogue controller |
| **Presentation control** | Embedded in the presentation layer | Graphical specification (Visual Basic) |

The trend has been toward presentation control — what you see is what you get, with the flow embedded in the visual design.

---

## KEY CONCEPTS FOR EXAM

1. **Windowing systems**: device independence + resource sharing for multiple apps
2. **Three architectures**: app manages, kernel manages, separate process manages (most portable)
3. **Client-server**: clients ↔ abstract terminals ↔ server ↔ device drivers
4. **X Windows**: client-server, separate window manager, pixel-based, X protocol
5. **Read-evaluation loop**: repeat → read event → case → process
6. **Notification-based**: register callbacks, notifier dispatches
7. **Going with grain**: modal (loop-easy) vs non-modal (callbacks-easy); don't let implementation drive design
8. **Toolkits**: interaction objects (widgets), consistency, OO programming
9. **Java AWT/Swing**: AWT (native, notification), Swing (on AWT, MVC)
10. **UIMS**: separation of presentation and application semantics
11. **Seeheim**: Presentation ↔ Dialogue Control ↔ Functionality (+ switch for rapid feedback)
12. **Lexical/Syntactic/Semantic**: feedback levels (mouse, highlight, data change)
13. **Arch/Slinky**: 5 layers (Physical → Lexical → Dialogue → FCA → Functional Core), slinky analogy
14. **MVC**: Model (state), View (rendering), Controller (input) — pipeline but controller talks to view
15. **PAC**: Abstraction, Presentation (unified I/O), Control (hierarchical)
16. **Implementation techniques**: state diagrams, grammars, events, declarations, constraints, graphical
17. **Constraints**: say what's true, not what happens
18. **ALV**: Abstraction-Link-View for groupware
19. **Dialogue control drift**: internal → external → presentation
