# Chapter 3: The Interaction — Where Human Meets Computer

## The Big Picture

Chapters 1 and 2 established the human and the computer as separate systems. Chapter 3 is about what happens **between them** — the interaction itself. We explore:

1. **Conceptual models** of interaction (Norman, Abowd & Beale)
2. **Physical ergonomics** of interaction
3. **Interaction styles** — the many ways humans have communicated with computers
4. **WIMP** — the dominant style in detail
5. **Context, experience, and value** — the softer side of interaction

---

## 1. WHAT IS INTERACTION?

Interaction is communication between user and system. Three key terms:

- **Domain** — the area of work (e.g., graphic design)
- **Goal** — what you want to achieve (e.g., create a solid red triangle)
- **Task** — how you go about doing it (e.g., select fill tool, click over triangle)

> Note: These terms are used differently across the HCI literature — especially task vs. goal!

---

## 2. TWO FRAMEWORKS FOR UNDERSTANDING INTERACTION

### Norman's Model — The User's View

Norman describes interaction as **7 stages** in a cycle:

```
1. Establish goal
2. Form intention
3. Specify actions
4. Execute action
        ↓
5. Perceive system state
6. Interpret state
7. Evaluate state vs. goal
```

This is an **execution/evaluation loop** — three stages to act, three to assess.

**Two critical gaps** can break the loop:

| Gulf | Problem | Example |
|------|---------|---------|
| **Gulf of Execution** | User's intended actions ≠ what the system allows | You want to save, but can't find the save button |
| **Gulf of Evaluation** | User's expected feedback ≠ what the system shows | You hit save, but nothing on screen confirms it |

**Error connection**: A **slip** = correct goal, wrong action (bridge the execution gulf). A **mistake** = wrong goal (bridge the evaluation gulf).

### Abowd & Beale Framework — The System's View

An extension of Norman that models interaction as **translation between four languages**:

```
User (U) ↔ Input (I) ↔ System (S) ↔ Output (O)
```

Each component has its **own language**. Interaction is a **translation** between them. Problems in interaction = breakdowns in translation.

Example: You want to delete a file (U-language) → you drag it to the trash (I-language) → the OS updates its file table (S-language) → the icon disappears (O-language) → you see it's gone (back to U).

**Benefits**: General (not just computers), identifies all major components, allows comparing different systems.

---

## 3. ERGONOMICS — The Physical Side

**Ergonomics (human factors)** studies the physical characteristics of interaction.

### Key Concerns

- **Arrangement of controls** — grouped by function or frequency
- **Environment** — seating, lighting, temperature, noise
- **Health** — physical position, environmental conditions
- **Colour** — red = warning, green = okay, remember colour blindness

### Office vs. Industrial Interfaces

| | Office | Industrial |
|--|--------|------------|
| Data type | Textual | Numeric |
| Rate of change | Slow | Fast |
| Environment | Clean | Dirty |
| Manipulation | Direct (user interacts with artificial world) | Indirect (user interacts with real world *through* interface) |

### Glass Interfaces

Traditional industrial interfaces (dials, knobs) → modern screens and keypads.

| Pros | Cons |
|------|------|
| Cheaper, more flexible | Not physically located |
| Multiple representations | Loss of context |
| Precise values | Complex interfaces |

Sometimes you need **both** traditional and glass interfaces.

---

## 4. INTERACTION STYLES — The Many Ways to Talk to a Computer

Eight major styles, roughly ordered from oldest to newest:

| Style | How It Works | Best For | Weakness |
|-------|-------------|----------|----------|
| **Command Line** | Type instructions directly | Experts, repetitive tasks | Steep learning curve |
| **Menus** | Choose from visible options | Novices (recognition > recall) | Screen space, hierarchy depth |
| **Natural Language** | Speak or type naturally | Everyone (familiar) | Ambiguous, hard to implement |
| **Q&A / Query** | System asks, user answers | Novices, database queries | Restricted functionality |
| **Form-fills** | Fill in fields like paper forms | Data entry | Needs good design |
| **Spreadsheets** | Grid of cells with values/formulas | Financial modeling | Specialized use |
| **WIMP** | Windows, Icons, Menus, Pointers | General-purpose | Complex to implement |
| **3D Interfaces** | Navigate virtual spaces | Gaming, simulation | Hard to use for productivity |

---

## 5. WIMP — The Dominant Paradigm

### The Big Four

- **W**indows — independent screen areas that can move, resize, overlap, or tile
- **I**cons — small pictures representing objects or actions
- **M**enus — lists of operations to select from
- **P**ointers — graphical cursors controlled by mouse/trackpad/keys

Plus: buttons, toolbars, palettes, dialog boxes.

### Windows in Detail
- Can contain text or graphics
- **Scrollbars** move contents
- **Title bars** name the window
- Two layouts: **overlapping** (modern) or **tiled** (side by side)

### Menus in Detail

**How menus appear:**
- **Menu bar** at top → drags down
  - Pull-down: hold and drag
  - Drop-down: click reveals
  - Fall-down: mouse over bar
- **Contextual menu** (pop-up): appears where you click
- **Pie menu**: arranged in a circle (larger targets, equal distance — but not widely used)

**Menu extras:**
- **Cascading**: sub-menus within menus
- **Keyboard accelerators**: Ctrl+letter shortcuts
- **Tear-off menus**: menu detaches to become a floating palette

### Buttons
- **Radio buttons**: mutually exclusive (choose one)
- **Check boxes**: non-exclusive (choose many)

### Dialog Boxes
Pop-up windows that demand information or announce events (e.g., "Save As..." dialog).

---

## 6. INTERACTIVITY — Look, Feel, and Control

### Look and Feel
Two systems can have the same WIMP elements but behave differently (e.g., Mac vs. Windows menus). **Appearance + behaviour = look and feel.**

### Initiative — Who's in Charge?

| Style | Who Leads |
|-------|-----------|
| Old Q&A systems | Computer |
| WIMP | **User** (mostly) |
| **Modal dialog boxes** | Computer (temporarily) — "won't go away!" |

Modal dialogs are **pre-emptive** — good for errors and essential steps, but use with care.

### Error and Repair
Errors are inevitable. Make them easy to **detect**, then easy to **repair**.

---

## 7. CONTEXT — Interaction Doesn't Happen in a Vacuum

People are affected by:
- **Other people** — competition, fear of failure, desire to impress
- **Motivation** — fear, allegiance, ambition, self-satisfaction
- **Inadequate systems** — cause frustration and kill motivation

---

## 8. EXPERIENCE, ENGAGEMENT, AND FUN

Not enough that people *can* use a system — they must *want* to.

**Flow** (Csikszentmihalyi): the optimal experience between anxiety and boredom. Related to **zone of proximal development** (education) — things you can just do with help.

**Christmas cracker example**: A virtual cracker must reproduce the experience — sharedness, co-experience, excitement, hiddenness, suspense, surprise. The surface elements (design, play, dressing up) must produce the right *experienced effects*.

---

## 9. PHYSICAL DESIGN — Real-World Constraints

### Six Types of Constraints (Often Contradictory)

1. **Ergonomic** — minimum button size
2. **Physical** — high-voltage switches are big
3. **Legal & safety** — cooker controls placement
4. **Context & environment** — easy to clean
5. **Aesthetic** — must look good
6. **Economic** — ...and not cost too much

Trade-offs exist **within** categories (front vs. rear cooker controls: both have different safety profiles) and **between** categories (ergonomics vs. physical: MiniDisc remote controls need to be bigger, but there's no room → multifunction controls).

### Fluidity — Does Physical Reflect Logical?
- Does the controller's physical state match the system's logical state? (e.g., toggle switch up = on)
- Inverse actions → inverse effects? (arrow buttons, twist controls)
- **Spring-back controls** (one-shot buttons, joysticks) — good for large selection sets, bad because they hide state.

### Compliant Interaction
- Mechanical buttons reveal their state visually
- Rotary knobs can be controlled by both user and machine — the state is evident

---

## 10. MANAGING VALUE — Why People Actually Use Things

### The Value Equation

People use something **ONLY IF**:
- It has **perceived value**
- **AND** value exceeds cost

**Value**: helps work, fun, good for others
**Cost**: download time, money, learning effort

### The Discounted Future Problem
People heavily discount future value and future cost. This is why there's resistance to learning — the short-term cost looms larger than the long-term benefit. **Solution**: low barriers + high perceived present value.

### Making People Do Things (Organizational Design)

| Strategy | How It Works |
|----------|-------------|
| **Coercion** | "Do it or you're fired" — value = keeping your job |
| **Enculturation** | Explain corporate values, share options — align individual with organization |
| **Emergence** | Design the process so individual value → organizational value naturally |

### General Lesson
If you want someone to do something: **make it easy for them** and **understand their values**.

---

## KEY CONCEPTS FOR EXAM

1. **Interaction terms**: domain (work area), goal (what to achieve), task (how to do it)
2. **Norman's 7 stages**: goal → intention → specify → execute → perceive → interpret → evaluate
3. **Gulfs**: Execution (user actions ≠ system allows) and Evaluation (user expects ≠ system shows)
4. **Slips** (right intention, wrong action) vs **Mistakes** (wrong intention)
5. **Abowd & Beale**: User, Input, System, Output — each with own language; interaction = translation
6. **Ergonomics**: physical characteristics, human factors, health, colour use
7. **Office vs Industrial**: text vs numeric, slow vs fast, clean vs dirty, direct vs indirect manipulation
8. **Glass interfaces**: cheaper, flexible, but loss of context
9. **Interaction styles**: CLI, menus, NL, Q&A, forms, spreadsheets, WIMP, 3D
10. **WIMP**: Windows, Icons, Menus, Pointers — default desktop paradigm
11. **Windows**: independent areas, scrollbars, title bars, overlapping/tiled
12. **Icons**: small pictures representing objects/actions
13. **Menu types**: pull-down, drop-down, fall-down, pop-up, pie, cascading
14. **Buttons**: radio (exclusive) vs check boxes (non-exclusive)
15. **Look and feel**: appearance + behaviour
16. **Modal dialog boxes**: pre-emptive, use sparingly
17. **Flow** (Csikszentmihalyi): balance anxiety and boredom
18. **Physical constraints**: ergonomic, physical, legal/safety, context, aesthetic, economic
19. **Fluidity**: physical state reflects logical state
20. **Value equation**: use IF perceived value > cost
21. **Discounted future**: high learning barrier → low adoption → need low barriers
22. **Organizational design**: coercion, enculturation, emergence
