# Chapter 8: Implementation Support - HCI Notes

## Overview
Chapter 8 covers implementation support for HCI: programming tools, windowing systems, application programming paradigms, interaction toolkits, and User Interface Management Systems (UIMS).

---

## 1. IMPLEMENTATION SUPPORT – FIVE KEY AREAS

1. **Programming tools** – levels of services for programmers
2. **Windowing systems** – core support for separate and simultaneous user-system activity
3. **Programming the application and control of dialogue**
4. **Interaction toolkits** – bring programming closer to level of user perception
5. **User interface management systems** – controls relationship between presentation and functionality

---

## 2. INTRODUCTION

### How Does HCI Affect the Programmer?
- Advances in coding have elevated programming from hardware specific → interaction-technique specific
- Layers of development tools:
  - Windowing systems
  - Interaction toolkits
  - User interface management systems

---

## 3. ELEMENTS OF WINDOWING SYSTEMS

### Device Independence
- Programming the abstract terminal device drivers
- Image models for output and (partially) input:
  - Pixels
  - PostScript (MacOS X, NextStep)
  - Graphical Kernel System (GKS)
  - Programmers' Hierarchical Interface to Graphics (PHIGS)

### Resource Sharing
- Achieving simultaneity of user tasks
- Window system supports independent processes
- Isolation of individual applications

---

## 4. ROLES OF A WINDOWING SYSTEM

### Architecture
- **Application programs** → Windowing System → **Devices**
- Windowing system provides:
  - Multiple application control
  - Device independence
- Manages multiple windows, mouse, keyboard

---

## 5. ARCHITECTURES OF WINDOWING SYSTEMS

### Three Possible Software Architectures
All assume device driver is separate; differ in how multiple application management is implemented:

1. **Each application manages all processes**
   - Everyone worries about synchronization
   - Reduces portability of applications

2. **Management role within kernel of operating system**
   - Applications tied to operating system

3. **Management role as separate application**
   - Maximum portability

---

## 6. THE CLIENT-SERVER ARCHITECTURE

### Components
- **Clients**: Application programs (1 to n)
- **Abstract Terminals**: One per client (1 to n)
- **Server**: Resource Manager
- **Device Driver**: Connects to mouse, keyboard, screen
- **Devices**: Mouse, keyboard, windows

---

## 7. X WINDOWS ARCHITECTURE

### Structure
- Application client → X11 server → Device drivers → Mouse/Keyboard/Screen
- Window manager client as separate entity

### Key Features
- Pixel imaging model with some pointing mechanism
- X protocol defines server-client communication
- **Separate window manager client** enforces policies for input/output:
  - How to change input focus
  - Tiled vs. overlapping windows
  - Inter-client data transfer

---

## 8. PROGRAMMING THE APPLICATION

### Two Paradigms

#### 1. Read-Evaluation Loop
- **Flow**: start → read input → process input → quit? → end
- **Code structure**:
  ```
  repeat
    read-event(myevent)
    case myevent.type
      type_1: do type_1 processing
      type_2: do type_2 processing
      ...
      type_n: do type_n processing
    end case
  end repeat
  ```

#### 2. Notification-Based
- Register callbacks with notifier
- Notifier reads input and sends to appropriate callback
- **Code structure**:
  ```java
  void main(String[] args) {
    Menu menu = new Menu();
    menu.setOption("Save");
    menu.setOption("Quit");
    menu.setAction("Save", mySave);
    menu.setAction("Quit", myQuit);
    ...
  }
  int mySave(Event e) { // save the current file }
  int myQuit(Event e) { // close down }
  ```

---

## 9. GOING WITH THE GRAIN

### System Style Affects Interfaces
- **Modal dialogue box**:
  - Easy with event-loop (just have extra read-event loop)
  - Hard with notification (need lots of mode flags)
- **Non-modal dialogue box**:
  - Hard with event-loop (very complicated main loop)
  - Easy with notification (just add extra handler)

### Warning
- **Beware!** If you don't explicitly design it will just happen
- **Implementation should not drive design**

---

## 10. USING TOOLKITS

### Interaction Objects
- Input and output intrinsically linked
- Example: Button (move → press → release → move)
- Toolkits provide this level of abstraction

### Benefits
- Programming with interaction objects (widgets, gadgets)
- Promote consistency and generalizability
- Through similar look and feel
- Amenable to object-oriented programming

---

## 11. INTERFACES IN JAVA

### Java Toolkit – AWT (Abstract Windowing Toolkit)
- Java classes for buttons, menus, etc.
- **Notification based**:
  - AWT 1.0 – need to subclass basic widgets
  - AWT 1.1 and beyond – callback objects

### Swing Toolkit
- Built on top of AWT – higher level features
- Uses MVC architecture (see later)

---

## 12. USER INTERFACE MANAGEMENT SYSTEMS (UIMS)

### Definition
- UIMS add another level above toolkits
- Toolkits too difficult for non-programmers

### Concerns of UIMS
- Conceptual architecture
- Implementation techniques
- Support infrastructure

### Non-UIMS Terms
- UI development system (UIDS)
- UI development environment (UIDE)
  - e.g. Visual Basic

---

## 13. UIMS AS CONCEPTUAL ARCHITECTURE

### Separation Principle
- **Separation** between application semantics and presentation

### Improves:
- **Portability** – runs on different systems
- **Reusability** – components reused cutting costs
- **Multiple interfaces** – accessing same functionality
- **Customizability** – by designer and user

---

## 14. UIMS TRADITION – INTERFACE LAYERS

### Linguistic Levels: Lexical/Syntactic/Semantic

### Seeheim Model
- Presentation ↔ Dialogue Control ↔ Functionality (application interface)
- Switch connects presentation and functionality

### Arch/Slinky Model
- Physical → Lexical → Dialogue → Func. core adaptor → Functional core
- Like a 'slinky' spring – different layers may be thicker in different systems

---

## 15. SEEHEIM MODEL

### Three Layers
1. **Presentation** (lexical)
2. **Dialogue Control** (syntactic)
3. **Functionality** (semantic) – application interface

### Key Component
- **Switch**: Connects presentation and functionality
  - Needed for implementation
  - But not conceptual

---

## 16. CONCEPTUAL VS. IMPLEMENTATION

### Seeheim's Contribution
- Arose out of implementation experience
- But principal contribution is conceptual
- Concepts part of 'normal' UI language
- **Because of Seeheim... we think differently!**

---

## 17. SEMANTIC FEEDBACK

### Different Kinds of Feedback
- **Lexical** – movement of mouse
- **Syntactic** – menu highlights
- **Semantic** – sum of numbers changes

### Semantic Feedback Often Slower
- Use rapid lexical/syntactic feedback

### But May Need Rapid Semantic Feedback
- Freehand drawing
- Highlight trash can or folder when file dragged

---

## 18. THE BYPASS/SWITCH

### Rapid Semantic Feedback
- Direct communication between application and presentation
- But regulated by dialogue control
- Allows fast response for certain operations

---

## 19. ARCH/SLINKY – MORE LAYERS

### Layer Structure
- Physical → Lexical → Dialogue → Func. core adaptor → Functional core
- More layers distinguish lexical/physical

### Key Insight
- Like a 'slinky' spring – different layers may be thicker (more important) in different systems or in different components

---

## 20. MONOLITHIC VS. COMPONENTS

### Seeheim Has Big Components
- Often easier to use smaller ones
- Especially if using object-oriented toolkits

### Smalltalk Used MVC – Model-View-Controller
- **Model** – internal logical state of component
- **View** – how it is rendered on screen
- **Controller** – processes user input

---

## 21. MVC – MODEL-VIEW-CONTROLLER

### Components
- **Model**: Internal state (data/logic)
- **View**: Screen rendering (output)
- **Controller**: Input processing

### Data Flow
- Model → View (display)
- Controller → Model (update)
- View ↔ Controller (coordinate)

---

## 22. MVC ISSUES

### Pipeline Model
- Input → Control → Model → View → Output

### Problem in Graphical Interface
- Input only has meaning in relation to output
- e.g. mouse click:
  - Need to know *what* was clicked
  - Controller has to decide what to do with click
  - But view knows what is shown where!
- **In practice controller 'talks' to view**
  - Separation not complete

---

## 23. PAC MODEL

### Definition
- PAC model closer to Seeheim
- **Abstraction** – logical state of component
- **Presentation** – manages input and output
- **Control** – mediates between them

### Key Features
- Manages hierarchy and multiple views
- Control part of PAC objects communicate

### Comparison
- PAC cleaner in many ways...
- But MVC used more in practice (e.g. Java Swing)

---

## 24. IMPLEMENTATION OF UIMS

### Techniques for Dialogue Controller
- Menu networks
- State transition diagrams
- Grammar notations
- Event languages
- Declarative languages
- Constraints
- Graphical specification

### N.B. Constraints
- Instead of what *happens* say what should be *true*
- Used in groupware as well as single user interfaces
- ALV – abstraction-link-view

---

## 25. GRAPHICAL SPECIFICATION

### What It Is
- Draw components on screen
- Set actions with script or links to program

### In Use
- With raw programming most popular technique
- e.g. Visual Basic, Dreamweaver, Flash

### Local vs. Global
- Hard to 'see' the paths through system
- Focus on what can be seen on one screen

---

## 26. THE DRIFT OF DIALOGUE CONTROL

### Three Levels
1. **Internal control** – e.g., read-evaluation loop
2. **External control** – independent of application semantics or presentation
3. **Presentation control** – e.g., graphical specification

---

## KEY CONCEPTS FOR EXAM
1. **Windowing systems**: device independence + resource sharing for multiple applications
2. **Three architectures**: app manages processes, OS kernel manages, separate app manages (most portable)
3. **Client-server architecture**: clients (apps) ↔ abstract terminals ↔ server (resource manager) ↔ device drivers
4. **X Windows**: client-server, separate window manager, pixel-based, X protocol
5. **Read-evaluation loop**: repeat → read event → case on type → process → end repeat
6. **Notification-based**: register callbacks, notifier dispatches to appropriate handler
7. **Going with grain**: system style affects what's easy/hard – implementation shouldn't drive design
8. **Toolkits**: interaction objects (widgets), consistency, OO programming
9. **Java AWT**: Abstract Windowing Toolkit, notification-based (1.0 subclass, 1.1 callbacks)
10. **Java Swing**: built on AWT, higher level, uses MVC
11. **UIMS**: separation of presentation and application semantics
12. **Seeheim model**: Presentation → Dialogue Control → Functionality (+ switch)
13. **Lexical/Syntactic/Semantic**: feedback levels (mouse movement, menu highlights, data changes)
14. **Arch/Slinky**: more layers, different thickness = different importance
15. **MVC**: Model (state), View (rendering), Controller (input) – pipeline but controller talks to view
16. **PAC**: Abstraction, Presentation, Control – closer to Seeheim, manages hierarchy
17. **Dialogue control drift**: Internal → External → Presentation control
18. **Graphical specification**: draw components, set actions (Visual Basic, Dreamweaver)
19. **Constraints**: say what should be true, not what happens
20. **ALV**: Abstraction-Link-View for groupware
