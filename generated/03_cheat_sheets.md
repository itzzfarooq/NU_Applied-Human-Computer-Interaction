# HCI Cheat Sheets — Chapters 1–9

---

## Ch1: The Human

### Perception
- **Vision**: 2 stages (reception → interpretation). Retina: rods (low light), cones (colour). Images focus upside-down. Blue acuity lowest. 8% males / 1% females colour blind.
- **Reading**: Saccades (movement) + fixations (pauses). Perception during fixations. Word shape matters. Negative contrast better for screens.
- **Hearing**: 20 Hz–15 kHz. Pitch/loudness/timbre. Cocktail party phenomenon (focus one voice in noise).
- **Touch**: Thermoreceptors (heat/cold), nociceptors (pain), mechanoreceptors (pressure). Kinesthesia = body position awareness.

### Movement
- **Response time** = reaction time + movement time
- Reaction times: visual ~200 ms, auditory ~150 ms, pain ~700 ms
- **Fitts' Law**: `Mt = a + b log₂(D/S + 1)`
  - D = distance to target, S = size of target
  - Implication: **large targets, short distances**

### Memory
| Type | Capacity | Access | Decay |
|------|----------|--------|-------|
| Sensory | Unlimited | Instant | Milliseconds |
| STM | **7 ± 2 chunks** | ~70 ms | ~200 ms |
| LTM | Unlimited | ~100 ms | Minimal |

- **Chunking**: group items into meaningful units to extend STM
- **LTM types**: Episodic (events, serial) vs Semantic (facts, structured)
- **Semantic memory models**:
  - *Networks*: inheritance (DOG inherits from ANIMAL)
  - *Frames*: slots with fixed/default/variable values
  - *Scripts*: stereotypical situations (props, roles, scenes, tracks)
  - *Production rules*: IF condition THEN action

### Thinking
- **Deduction**: premises → necessary conclusion (not necessarily true)
- **Induction**: generalize from seen → unseen (unreliable but useful)
- **Abduction**: event → cause (unreliable)
- **Wason's cards**: poor at using negative evidence

### Errors
- **Slips**: right intention, wrong action → fix: better interface design
- **Mistakes**: wrong intention → fix: better understanding

### Emotion & Affect
- Positive affect → creative problem solving; negative → narrow thinking
- Aesthetically pleasing interfaces increase positive affect
- Stressed users find tasks harder; relaxed users more forgiving

---

## Ch2: The Computer

### Displays
- **Resolution**: pixels (H × V). **Colour depth**: bits/pixel (1-bit B&W, 8-bit 256 colours, 24-bit true colour)
- CRT, LCD, OLED. Refresh rate, luminance, contrast, gamma.

### Colour Models
| Model | Type | Use |
|-------|------|-----|
| **RGB** | Additive | Displays (0–255 per channel, 24-bit = 16.7M colours) |
| **HSB** | Intuitive | Design (Hue 0–360°, Saturation, Brightness) |
| **CMYK** | Subtractive | Printing (pigments absorb light) |

- Colour design: red=warning, green=go, blue=info. Don't rely on colour alone (colour blindness).

### Input Devices
- **Keyboard**: QWERTY (prevent jamming), Dvorak (efficiency), chord, soft
- **Mouse**: relative positioning, mechanical/optical/laser
- **Trackball**: stationary mouse variant
- **Touchpad**: finger position, laptops
- **Joystick**: 2D/3D, gaming/CAD
- **Pen/Stylus**: direct input, natural writing

### Other Modalities
- **Audio**: speech synthesis, earcons, auditory icons
- **Haptic**: vibration, force feedback, texture
- **Speech recognition**: speaker-dependent vs independent, discrete vs continuous
- **Eye tracking**: fixations, saccades, scan paths

### Screen Design
- Grouping (Gestalt), alignment, white space, consistency
- Sans-serif for screens, 50–75 char line length, min 12pt

---

## Ch3: The Interaction

### Norman's 7 Stages
1. Goal → 2. Intention → 3. Specify actions → 4. Execute → 5. Perceive → 6. Interpret → 7. Evaluate

### Gulfs
- **Gulf of Execution**: user's formulation ≠ system's allowed actions
- **Gulf of Evaluation**: user's expectation ≠ actual system state

### Abowd & Beale Framework
- **U** (User) → **I** (Input) → **S** (System) → **O** (Output)
- Each has own language; interaction = translation between languages

### Ergonomics
- Physical characteristics of interaction (human factors)
- Office (text/slow/clean) vs Industrial (numeric/fast/dirty)
- Glass interfaces: cheaper, flexible, but loss of context

### Interaction Styles
| Style | Best For |
|-------|----------|
| Command line | Experts, repetitive tasks |
| Menus | Novices, visible options |
| Natural language | Familiar, but vague |
| Form-fills | Data entry/retrieval |
| **WIMP** | Default for most systems |

### WIMP Elements
- **W**indows: independent screen areas, scrollbars, overlapping/tiled
- **I**cons: small pictures representing objects/actions
- **M**enus: pull-down, drop-down, pop-up, pie, cascading
- **P**ointers: mouse/trackpad/joystick, graphical cursors
- **Buttons**: radio (mutually exclusive), checkboxes (non-exclusive)
- **Toolbars/Palettes**: fast access to common actions

### Key Concepts
- **Look and feel** = appearance + behaviour
- **Modal dialogs**: pre-emptive (errors, essential steps)
- **Flow** (Csikszentmihalyi): balance anxiety ↔ boredom
- **Value equation**: use IF perceived value > cost
- People discount future value → resistance to learning

---

## Ch4: Paradigms

### Timeline of Shifts
| Era | Paradigm | Key Feature |
|-----|----------|-------------|
| 1950s–60s | **Batch processing** | No direct interaction |
| 1960s | **Time-sharing** | Multiple users, interactive computing |
| 1960s–70s | **Networking** | Community, email, file sharing |
| 1962 | **Graphical displays** | Sketchpad (Sutherland) |
| 1970s | **Microprocessor** | LOGO (Papert), Dynabook (Kay), personal computing |
| 1981 | **WIMP/Windowing** | Xerox Star — first commercial windowing system |
| 1982 | **Direct manipulation** | Shneiderman: visibility, feedback, reversibility |
| 1990s | **WWW** | Hypertext on global network, HTTP/HTML |
| 1991+ | **Ubiquitous computing** | Weiser: "technologies that disappear" |

### Key Inventions
- **Sketchpad** (Sutherland, 1962): first graphical interaction
- **LOGO** (Papert, 1970s): children programming with turtle graphics
- **Xerox Star** (1981): first commercial WIMP system
- **Hypertext**: Bush memex (1945) → Nelson (1960s) → WWW

### Concepts
- **Metaphor**: relating computing to real-world (file/folder, desktop). Problems: cultural bias, task mismatch.
- **Direct Manipulation**: WYSIWYG, incremental action, rapid feedback, reversibility
- **CSCW**: Computer Supported Cooperative Work — multi-user focus
- **Agent-based interfaces**: proactive, intelligent, return to language paradigm
- **Context-aware**: sensing physical phenomena, making systems "aware"

---

## Ch5: Design Basics

### User Focus
- **Personas**: fictional users representing real categories — help argue for features
- **Cultural probes**: materials sent to participants to document own lives
- **Contextual inquiry**: observe + interview users in natural environment
- **Scenarios**: stories about users & systems (concrete vs abstract)

### Navigation Design — 4 Golden Rules
1. **Landmarks** — help users know where they are
2. **Routes** — clear paths through information
3. **Overviews** — show overall structure
4. **Context** — relationship to other parts

- Breadcrumbs show path taken. Modes = different interface states.

### Screen Design (Gestalt Principles)
| Principle | Description |
|-----------|-------------|
| **Proximity** | Close items → perceived as group |
| **Similarity** | Similar-looking items → perceived as group |
| **Closure** | Mind completes incomplete shapes |
| **Continuity** | Eye follows smooth paths |

- **Alignment**: visual consistency, grid-based
- **White space**: reduces cognitive load

### Affordances
- Properties that suggest how an object can be used (button affords pressing, slider affords sliding)
- Real-world: physical affordances. Interface: perceived affordances.

### Aesthetics
- Aesthetic-usability effect: attractive things work better
- Emotional response matters

### Localisation
- **Internationalisation**: design for multiple cultures from start
- **Localisation**: adapt for specific locale (text direction, dates, currency, symbols)

### Prototyping
- Low-fidelity (paper) vs high-fidelity (electronic)
- Throwaway / incremental / evolutionary
- **Wizard of Oz**: human simulates computer response
- Iteration: test → learn → improve (don't expect right first time)

---

## Ch6: Software Process

### Waterfall Model
1. Requirements → 2. Architectural design → 3. Detailed design → 4. Coding & unit test → 5. Integration & test → 6. Operation & maintenance
- Interactive systems need **feedback loops** between all stages

### Verification vs Validation
- **Verification**: designing the product right
- **Validation**: designing the right product
- **Formality gap**: validation always relies partly on subjective proof

### Usability Engineering
- Specific usability measures as explicit requirements
- Usability spec: attribute → measuring concept → method → now/worst/planned/best levels

### ISO 9241
| Dimension | Question |
|-----------|----------|
| **Effectiveness** | Can you achieve what you want? |
| **Efficiency** | Can you do it without wasting effort? |
| **Satisfaction** | Do you enjoy the process? |

### Prototyping Types
| Type | Description |
|------|-------------|
| **Throwaway** | Built quickly, discarded after use |
| **Incremental** | Built piece by piece, added to system |
| **Evolutionary** | Evolves into final system |

- Storyboards: visual interaction flow
- Wizard of Oz: human simulates system

### Design Rationale
- Explains **why** a system is the way it is
- **IBIS** (process-oriented): Issues → Positions → Arguments
- **QOC** (structure-oriented): Questions → Options → Criteria
- **DRL**: more formal version of QOC

---

## Ch7: Design Rules

### Three Types
| Type | Authority | Generality |
|------|-----------|------------|
| **Principles** | Low | High |
| **Standards** | High | Low |
| **Guidelines** | Medium | Medium |

### Principles of Usability
- **Learnability**: new users become effective quickly
- **Flexibility**: multiplicity of ways to exchange information
- **Robustness**: support for goal achievement & assessment

### Sub-principles
| Category | Principle | Meaning |
|----------|-----------|---------|
| Learnability | Predictability | Future actions predictable from past |
| | Synthesizability | Assess effect of past actions |
| | Familiarity | Prior knowledge applies |
| | Generalizability | Extend knowledge to new situations |
| | Consistency | Similar situations → similar behaviour |
| Flexibility | Dialogue initiative | User vs system pre-emptiveness |
| | Multithreading | Support multiple tasks simultaneously |
| | Task migratability | Pass responsibility between user & system |
| | Substitutivity | Equivalent values for input/output |
| | Customizability | Adaptability (user) vs adaptivity (system) |
| Robustness | Observability | Evaluate internal state from display |
| | Recoverability | Corrective action after error |
| | Responsiveness | Perceived rate of communication |
| | Task conformance | System supports all user tasks |

### Shneiderman's 8 Golden Rules
1. Consistency
2. Shortcuts for frequent users
3. Informative feedback
4. Dialogues yield closure
5. Error prevention & simple handling
6. Easy reversal of actions
7. Internal locus of control
8. Reduce short-term memory load

### Norman's 7 Principles
1. Knowledge in world + head
2. Simplify task structure
3. Make things visible (bridge gulfs)
4. Get mappings right
5. Exploit constraints
6. Design for error
7. Standardize when all else fails

### HCI Patterns
- Invariant solution to recurrent problem in specific context
- Pattern languages link patterns → complete designs
- Capture design **practice** not theory

---

## Ch8: Implementation

### Windowing Systems
- **Device independence**: abstract terminal drivers
- **Resource sharing**: multiple applications simultaneously
- **3 architectures**: app manages, OS manages, separate app manages (most portable)

### Client-Server
- Clients (apps) ↔ Abstract terminals ↔ Server (resource manager) ↔ Device drivers
- **X Windows**: client-server, separate window manager, X protocol

### Programming Paradigms
| Paradigm | Flow |
|----------|------|
| **Read-evaluation loop** | repeat → read event → case → process → end |
| **Notification-based** | register callbacks → notifier dispatches |

- Modal dialogs: easy with event-loop, hard with notification
- Non-modal dialogs: hard with event-loop, easy with notification
- **Warning**: implementation should not drive design

### Toolkits
- Interaction objects (widgets): button, menu, slider
- Promote consistency. Amenable to OO programming.
- **Java AWT**: notification-based. **Swing**: built on AWT, uses MVC.

### UIMS
- Separates presentation from application semantics
- Improves: portability, reusability, multiple interfaces, customizability

### Seeheim Model (3 layers)
| Layer | Level |
|-------|-------|
| **Presentation** | Lexical |
| **Dialogue Control** | Syntactic |
| **Functionality** | Semantic |

- Switch connects presentation ↔ functionality
- Semantic feedback often slower → use rapid lexical/syntactic feedback

### MVC
| Component | Role |
|-----------|------|
| **Model** | Internal state / data / logic |
| **View** | Screen rendering (output) |
| **Controller** | Input processing |

- Pipeline: Controller → Model → View. In practice, controller "talks" to view (separation not complete).

### PAC
- **Abstraction** (logical state), **Presentation** (I/O), **Control** (mediator)
- Closer to Seeheim. Manages hierarchy & multiple views.
- MVC more widely used (e.g. Java Swing)

---

## Ch9: Evaluation

### Expert Evaluation
| Method | Who | Focus |
|--------|-----|-------|
| **Cognitive walkthrough** | Psychology expert | How well design supports learning |
| **Heuristic evaluation** | Design experts | Violations of usability heuristics |
| **Review-based** | Any expert | Literature/model-based support |

### Heuristic Evaluation (Nielsen & Molich)
- Experts check design against heuristics (predictable behaviour, consistency, feedback, etc.)
- "Debugs" design without users

### User-Based Evaluation
| Setting | Pros | Cons |
|---------|------|------|
| **Lab** | Controlled, specialist equipment | Lack of context |
| **Field** | Natural, context retained | Distractions, noise |

### Observational Methods
| Method | Description |
|--------|-------------|
| **Think aloud** | User narrates thoughts while performing tasks |
| **Cooperative evaluation** | User + evaluator collaborate, both ask questions |
| **Protocol analysis** | Paper/audio/video/logging of actions |
| **Post-task walkthrough** | Transcript played back, immediate or delayed |

### Experimental Evaluation
- **IV (Independent Variable)**: what you change (e.g. interface style)
- **DV (Dependent Variable)**: what you measure (e.g. time, errors)
- **Null hypothesis**: no difference — aim is to disprove
- **Within groups**: each subject does all conditions (less costly, learning transfer possible)
- **Between groups**: each subject does one condition (no transfer, more users needed)
- **Parametric tests**: assume normal distribution, powerful
- **Non-parametric tests**: no normal assumption, less powerful, more reliable

### Eye Tracking
- **Fixations**: stable position → duration indicates difficulty
- **Saccades**: rapid movement between points of interest
- **Scan paths**: straight to target + short fixation = optimal

### Choosing a Method — 7 Dimensions
1. **When**: design vs implementation
2. **Style**: lab vs field
3. **Objectivity**: subjective vs objective
4. **Measures**: qualitative vs quantitative
5. **Info level**: high vs low
6. **Interference**: obtrusive vs unobtrusive
7. **Resources**: time, subjects, equipment, expertise

### Query Techniques
- **Interviews**: one-to-one, informal, subjective, flexible
- **Questionnaires**: fixed questions, quick, large groups, rigorous analysis
- Question styles: general, open-ended, scalar (Likert), multi-choice, ranked
