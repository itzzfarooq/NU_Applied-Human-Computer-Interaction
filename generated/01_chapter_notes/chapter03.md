# Chapter 3: The Interaction - HCI Notes

## Overview
Chapter 3 covers the interaction between humans and computers: interaction models (Norman's model, Abowd & Beale framework), ergonomics, interaction styles (command line, menus, natural language, WIMP, etc.), WIMP elements, interactivity, context, experience design, physical design, and managing value.

---

## 1. WHAT IS INTERACTION?

Interaction = communication between user and system

But is that all? See "language and action" in Chapter 4...

### Terms of Interaction
- **Domain** – the area of work under study (e.g. graphic design)
- **Goal** – what you want to achieve (e.g. create a solid red triangle)
- **Task** – how you go about doing it (ultimately in terms of operations or actions)
  - Example: select fill tool, click over triangle

**Note**: Traditional interaction – use of terms differs a lot, especially task/goal!

---

## 2. NORMAN'S MODEL

### Seven Stages
1. User establishes the **goal**
2. Formulates **intention**
3. **Specifies actions** at interface
4. **Executes action**
5. **Perceives** system state
6. **Interprets** system state
7. **Evaluates** system state with respect to goal

### Key Insight
Norman's model concentrates on **user's view** of the interface.

### Execution/Evaluation Loop
- Circular flow: goal → execution → system → evaluation → goal
- Three execution stages: formulate intention, specify actions, execute action
- Three evaluation stages: perceive state, interpret state, evaluate state

### Gulfs
- **Gulf of Execution**: user's formulation of actions ≠ actions allowed by the system
- **Gulf of Evaluation**: user's expectation of changed system state ≠ actual presentation of this state

### Human Error - Slips and Mistakes
- **Slip**: understand system and goal, correct formulation of action, but incorrect action
- **Mistake**: may not even have right goal!
- **Fixing**: slip → better interface design; mistake → better understanding of system

---

## 3. ABOWD AND BEALE FRAMEWORK

### Extension of Norman's Model
Their interaction framework has 4 parts:
- **User** (U)
- **Input** (I)
- **System** (S)
- **Output** (O)

Each has its own unique language. Interaction = translation between languages. Problems in interaction = problems in translation.

### Translation Process
User intentions → translated into actions at the interface → translated into alterations of system state → reflected in the output display → interpreted by the user

### Benefits
- General framework for understanding interaction
- Not restricted to electronic computer systems
- Identifies all major components involved in interaction
- Allows comparative assessment of systems
- An abstraction

---

## 4. ERGONOMICS

### Definition
Study of the physical characteristics of interaction. Also known as **human factors**.

### Examples
- **Arrangement of controls and displays** – grouped according to function or frequency of use
- **Surrounding environment** – seating arrangements adaptable to all sizes
- **Health issues** – physical position, environmental conditions (temperature, humidity), lighting, noise
- **Use of colour** – red for warning, green for okay, awareness of colour-blindness

### Office vs Industrial Interfaces
| | Office | Industrial |
|---|---|---|
| Type of data | Textual | Numeric |
| Rate of change | Slow | Fast |
| Environment | Clean | Dirty |

### Glass Interfaces
- Industrial interface: traditional (dials and knobs) → now (screens and keypads)
- **Glass interface advantages**: cheaper, more flexible, multiple representations, precise values
- **Glass interface disadvantages**: not physically located, loss of context, complex interfaces
- May need both traditional and glass interfaces

### Indirect Manipulation
- **Office**: direct manipulation – user interacts with artificial world
- **Industrial**: indirect manipulation – user interacts *with* real world *through* interface
- Issues: feedback, delays

---

## 5. INTERACTION STYLES

### Common Styles
1. Command line interface
2. Menus
3. Natural language
4. Question/answer and query dialogue
5. Form-fills and spreadsheets
6. WIMP
7. Point and click
8. Three-dimensional interfaces

### Command Line Interface
- Way of expressing instructions directly (function keys, characters, abbreviations, words)
- Suitable for repetitive tasks
- Better for expert users than novices
- Offers direct access to system functionality
- Command names/abbreviations should be meaningful
- **Typical example**: Unix system

### Menus
- Set of options displayed on screen
- Options visible → less recall → easier to use
- Rely on recognition → names should be meaningful
- Selection by: numbers, letters, arrow keys, mouse, combinations
- Often hierarchically grouped → sensible grouping needed
- Restricted form of full WIMP system

### Natural Language
- Familiar to user
- Speech recognition or typed natural language
- **Problems**: vague, ambiguous, hard to do well
- **Solutions**: try to understand a subset, pick on key words

### Query Interfaces
- **Question/answer**: user led through interaction via series of questions, suitable for novice users but restricted functionality
- **Query languages** (e.g. SQL): used to retrieve information from database, requires understanding of database structure and language syntax

### Form-fills
- Primarily for data entry or data retrieval
- Screen like paper form
- Data put in relevant place
- Requires good design and obvious correction facilities

### Spreadsheets
- First spreadsheet: VisiCalc, followed by Lotus 1-2-3, MS Excel most common today
- Sophisticated variation of form-filling
- Grid of cells contain a value or a formula
- Formula can involve values of other cells
- User can enter and alter data; spreadsheet maintains consistency

---

## 6. WIMP INTERFACE

### Components
- **W**indows
- **I**cons
- **M**enus
- **P**ointers

Or: windows, icons, mice, and pull-down menus!

### Default Style
Default style for majority of interactive computer systems, especially PCs and desktop machines.

### Additional Elements
- Buttons, toolbars, palettes, dialog boxes

---

## 7. WIMP ELEMENTS IN DETAIL

### Windows
- Areas of the screen that behave as if they were independent
- Can contain text or graphics
- Can be moved or resized
- Can overlap (overlapping) or be laid out next to one another (tiled)
- **Scrollbars** – allow user to move contents up/down or side to side
- **Title bars** – describe the name of the window

### Icons
- Small picture or image
- Represents some object in the interface (often a window or action)
- Windows can be closed down (iconised) → small representation for many accessible windows
- Can be highly stylized or realistic representations

### Pointers
- Important component – WIMP style relies on pointing and selecting things
- Uses mouse, trackpad, joystick, trackball, cursor keys or keyboard shortcuts
- Wide variety of graphical images (arrow, crosshair, target, etc.)

### Menus
- Choice of operations or services offered on the screen
- Required option selected with pointer
- **Problem**: take a lot of screen space
- **Solution**: pop-up – menu appears when needed

### Kinds of Menus
- **Menu Bar** at top of screen, menu drags down
  - **Pull-down menu** – mouse hold and drag down
  - **Drop-down menu** – mouse click reveals menu
  - **Fall-down menus** – mouse just moves over bar!
- **Contextual menu** appears where you are
  - **Pop-up menus** – actions for selected object
  - **Pie menus** – arranged in a circle
    - Easier to select item (larger target area)
    - Quicker (same distance to any option)
    - ... but not widely used!

### Menu Extras
- **Cascading menus** – hierarchical menu structure, selection opens new menu
- **Keyboard accelerators** – key combinations, same effect as menu item
  - Active when menu open – usually first letter
  - Active when menu closed – usually Ctrl + letter (usually different!)

### Menu Design Issues
- Which kind to use
- What to include in menus at all
- Words to use (action or description)
- How to group items
- Choice of keyboard accelerators

### Buttons
- Individual and isolated regions within a display that can be selected to invoke an action
- **Radio buttons** – set of mutually exclusive choices
- **Check boxes** – set of non-exclusive choices

### Toolbars
- Long lines of icons for fast access to common actions
- Often customizable: choose which toolbars to see, what options on it

### Palettes and Tear-off Menus
- **Problem**: menu not there when you want it
- **Solution**: 
  - Palettes – little windows of actions, shown/hidden via menu option
  - Tear-off and pin-up menus – menu 'tears off' to become palette

### Dialogue Boxes
- Information windows that pop up to inform of an important event or request information
- Example: saving a file → dialogue box for filename and location → disappears after save

---

## 8. INTERACTIVITY

### Look and Feel
- WIMP systems have the same elements: windows, icons, menus, pointers, buttons, etc.
- But different window systems *behave* differently
- Example: MacOS vs Windows menus
- **Appearance + behaviour = look and feel**

### Initiative
- Who has the initiative?
  - Old question-answer → computer
  - WIMP interface → user
- WIMP exceptions: **pre-emptive** parts of the interface
  - **Modal dialog boxes** – come and won't go away!
  - Good for errors, essential steps
  - But use with care

### Error and Repair
- Can't always avoid errors... but we can put them right
- Make it easy to *detect* errors → then the user can *repair* them

---

## 9. CONTEXT

Interaction affected by social and organizational context:
- **Other people** – desire to impress, competition, fear of failure
- **Motivation** – fear, allegiance, ambition, self-satisfaction
- **Inadequate systems** – cause frustration and lack of motivation

---

## 10. EXPERIENCE, ENGAGEMENT AND FUN

### Experience
- Home, entertainment, shopping – not enough that people *can* use a system, they must *want* to use it!
- Psychology of experience: **flow** (Csikszentmihalyi) – balance between anxiety and boredom
- Education: **zone of proximal development** – things you can just do with help
- Wider: literary analysis, film studies, drama

### Designing Experience (Christmas Cracker Example)
| | Real cracker | Virtual cracker |
|---|---|---|
| **Surface elements** | | |
| Design | cheap and cheerful | simple page/graphics |
| Play | plastic toy and joke | web toy and joke |
| Dressing up | paper hat | mask to cut out |
| **Experienced effects** | | |
| Shared | offered to another | sent by email message |
| Co-experience | pulled together | sender can't see content until opened |
| Excitement | cultural connotations | recruited expectation |
| Hiddenness | contents inside | first page - no contents |
| Suspense | pulling cracker | slow... page change |
| Surprise | bang (when it works) | WAV file (when it works) |

---

## 11. PHYSICAL DESIGN

### Constraints
- **Ergonomic** – minimum button size
- **Physical** – high-voltage switches are big
- **Legal and safety** – high cooker controls
- **Context and environment** – easy to clean
- **Aesthetic** – must look good
- **Economic** – ... and not cost too much!

### Design Trade-offs
Constraints are contradictory → need trade-offs

**Within categories**: e.g. safety – cooker controls: front panel safer for adult, rear panel safer for child

**Between categories**: e.g. ergonomics vs. physical – MiniDisc remote: controls need to be bigger, no room → solution: multifunction controls & reduced functionality

### Fluidity
- Do external physical aspects reflect logical effect?
- Related to affordance (Chapter 5)
- Logical state revealed in physical state? (e.g. on/off buttons)
- Inverse actions → inverse effects? (e.g. arrow buttons, twist controls)

### Spring-back Controls
- One-shot buttons, joystick, some sliders
- Good: large selection sets
- Bad: hidden state

### Physical Layout
- Controls: logical relationship ≈ spatial grouping
- Example: Microwave control panel – grouped controls for different functions

### Compliant Interaction
- State evident in mechanical buttons
- Rotary knobs reveal internal state and can be controlled by both user and machine

---

## 12. MANAGING VALUE

### The Value Equation
People use something **ONLY IF**:
- It has **perceived value**
- **AND** value exceeds cost

**BUT NOTE**: exceptions (e.g. habit), value NOT necessarily personal gain or money

### Weighing Up Value
**Value**:
- Helps me get my work done
- Fun
- Good for others

**Cost**:
- Download time
- Money
- Learning effort

### Discounted Future
- In economics: Net Present Value, discount by (1+rate)^years to wait
- In life: people heavily discount future value and future cost
- Hence resistance to learning
- Need low barriers and high perceived present value

### Value and Organisational Design
- **Coercion** – tell people what to do! Value = keep your job
- **Enculturation** – explain corporate values, establish support (e.g. share options)
- **Emergence** – design process so that individuals value → organisational value

### General Lesson
If you want someone to do something:
- Make it easy for them!
- Understand their values

---

## KEY CONCEPTS FOR EXAM
1. **Terms of interaction**: domain (area of work), goal (what to achieve), task (how to do it)
2. **Norman's model**: 7 stages – goal, intention, specify actions, execute, perceive, interpret, evaluate
3. **Execution/evaluation loop**: circular flow between user's goals and system state
4. **Gulf of Execution**: user's formulation ≠ system's allowed actions
5. **Gulf of Evaluation**: user's expectation ≠ actual system state
6. **Slips**: right intention, wrong action; **Mistakes**: wrong intention
7. **Abowd & Beale framework**: User, Input, System, Output – each with own language, interaction = translation
8. **Ergonomics**: physical characteristics, human factors, health issues, colour use
9. **Office vs Industrial**: text vs numeric, slow vs fast, clean vs dirty
10. **Glass interfaces**: cheaper, more flexible, but loss of context
11. **Indirect manipulation**: industrial – user interacts with real world through interface
12. **Command line**: direct access, better for experts, repetitive tasks
13. **Menus**: visible options, less recall, recognition-based, hierarchical grouping
14. **WIMP**: Windows, Icons, Menus, Pointers – default style for most systems
15. **Windows**: independent areas, scrollbars, title bars, overlapping/tiled
16. **Icons**: small pictures representing objects/actions
17. **Pointers**: mouse/trackpad/joystick, graphical images for pointing
18. **Menu types**: pull-down, drop-down, fall-down, pop-up, pie, cascading
19. **Buttons**: radio buttons (mutually exclusive), check boxes (non-exclusive)
20. **Look and feel**: appearance + behaviour
21. **Modal dialog boxes**: pre-emptive, good for errors/essential steps
22. **Flow** (Csikszentmihalyi): balance between anxiety and boredom
23. **Physical design constraints**: ergonomic, physical, legal/safety, context, aesthetic, economic
24. **Fluidity**: external physical aspects reflect logical effect
25. **Value equation**: use something IF perceived value > cost
26. **Discounted future**: people discount future value → resistance to learning → need low barriers
27. **Organisational design**: coercion, enculturation, emergence
