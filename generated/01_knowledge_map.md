# Knowledge Map — Applied HCI (Chapters 1–9)

## Chapter 1: The Human — The User We Design For

- **Human as Information Processing System**
  - Input → Memory → Processing → Output (modulated by Emotion, prone to Errors)

- **Perception (Input)**
  - Vision
    - Two stages: physical reception + processing/interpretation
    - Retina: rods (low light) vs cones (colour)
    - Ganglion cells (pattern/movement detection)
    - Visual angle, visual acuity, size constancy
    - Brightness: subjective reaction to luminance, just noticeable difference
    - Colour: hue / intensity / saturation; blue acuity lowest; colour blindness (8% males, 1% females)
    - Optical illusions (Ponzo, Muller-Lyer)
  - Reading
    - Multi-stage: perceive → decode → interpret
    - Saccades (fast eye jumps) + fixations (perception pauses)
    - Word shape matters
    - Negative contrast (dark on light) preferred for screens
  - Hearing
    - Three parts: outer / middle / inner
    - Properties: pitch (frequency) / loudness (amplitude) / timbre (quality)
    - Range: 20Hz–15kHz
    - Cocktail party phenomenon (selective attention)
  - Touch
    - Thermoreceptors (heat/cold), Nociceptors (pain), Mechanoreceptors (pressure)
    - Kinesthesia (body position awareness)
  - Movement (Output)
    - Reaction time: visual ~200ms, auditory ~150ms, pain ~700ms
    - Fitts' Law: Mt = a + b log₂(D/S + 1) → large targets, short distances

- **Memory (Storage) — Three Systems**
  - Sensory Memory (ultra-short buffers)
    - Iconic (visual), Echoic (aural), Haptic (tactile)
    - Continuously overwritten
  - Short-Term Memory (STM)
    - Rapid access (~70ms), rapid decay (~200ms)
    - Capacity: 7 ± 2 chunks
    - Chunking increases effective capacity
  - Long-Term Memory (LTM)
    - Slow access (~100ms), practically permanent, unlimited capacity
    - Episodic (events/autobiographical) vs Semantic (facts/concepts)
    - LTM structure models:
      - Semantic Networks (nodes with inheritance)
      - Frames (slots: fixed / default / variable values)
      - Scripts (stereotypical situations: entry conditions, props, roles, scenes, tracks)
      - Production Rules (IF condition THEN action)
    - Forgetting: decay + interference (retroactive, proactive)
    - Retrieval: Recall (reproduce with cues) vs Recognition (identify as seen before)

- **Processing (Thinking)**
  - Reasoning types: Deduction / Induction / Abduction
  - Wason's Cards: humans poor at negative evidence
  - Problem Solving theories
    - Gestalt: reproductive + productive (insight/restructuring)
    - Problem Space Theory: states + operators + heuristics (means-ends analysis)
    - Analogy: transfer from similar domains
  - Skill Acquisition: expert chunking (conceptual grouping)

- **Errors (Output)**
  - Slips: right intention, wrong action → fix with better interface design
  - Mistakes: wrong intention → fix with better understanding
  - Mental models explain how users understand systems

- **Emotion (Modulator)**
  - Theories: James-Lange / Cannon / Schacter-Singer
  - Positive affect → creative problem solving, forgiving of flaws
  - Negative affect → narrow thinking, harder tasks
  - Aesthetically pleasing interfaces increase positive affect

- **Variation (Individual Differences)**
  - Long-term: sex, physical/intellectual abilities
  - Short-term: stress, fatigue
  - Changing: age
  - Design must not exclude user population segments

---

## Chapter 2: The Computer — The Other Half of the Dialogue

- **Output Devices**
  - Displays
    - Specs: resolution (pixels), colour depth (bits/pixel), refresh rate
    - Text vs Graphics displays
    - Anti-aliasing smooths jagged edges
    - Luminance, contrast, gamma correction
  - Audio Output
    - Speech synthesis (text-to-speech)
    - Earcons (musical representations)
    - Auditory icons (real-world sounds)
  - Haptic Output
    - Vibration, force feedback, texture simulation

- **Input Devices**
  - Keyboards: QWERTY (anti-jam), Dvorak (efficient), chord keyboards, soft keyboards
  - Pointing devices
    - Mouse: relative movement (mechanical / optical / laser)
    - Trackball: stationary, compact
    - Touchpad: laptop standard, finger position sensing
    - Joystick: 2D/3D, gaming/CAD
    - Pen/Stylus: direct input, occlusion problem
  - Speech Recognition: speaker-dependent vs independent; discrete vs continuous
  - Gesture Recognition: cameras, gloves, accelerometers
  - Eye Tracking: fixations, saccades, scan paths
  - Brain-Computer Interface (BCI): EEG-based, experimental

- **Colour (Bridge between Human and Computer)**
  - RGB (additive, displays), HSB/HSV (intuitive, design), CMYK (subtractive, printing)
  - Colour in UI: red=warning, green=okay, blue=information
  - Never rely on colour alone (colour blindness)
  - Redundant cues: shapes, patterns, text labels
  - Metamerism, gamma correction, calibration

- **Screen Design Principles**
  - Gestalt: grouping (proximity, similarity), alignment, white space, consistency
  - Text: sans-serif for screens, 12pt min, 50-75 char lines, 1.2-1.5× spacing, high contrast
  - Progressive disclosure (show detail on demand)

---

## Chapter 3: The Interaction — Where Human Meets Computer

- **Key Terms**: domain (work area), goal (what to achieve), task (how to do it)

- **Norman's Model (7 Stages)**
  - Goal → Intention → Specify → Execute → Perceive → Interpret → Evaluate
  - Execution/evaluation loop (3 to act, 3 to assess)
  - Gulf of Execution: user's intended actions ≠ system allows
  - Gulf of Evaluation: user's expected feedback ≠ system shows
  - Slips bridge execution gulf; mistakes bridge evaluation gulf

- **Abowd & Beale Framework**
  - User (U) ↔ Input (I) ↔ System (S) ↔ Output (O)
  - Each has own "language"; interaction = translation between languages

- **Ergonomics (Human Factors)**
  - Arrangement of controls, environment, health, colour use
  - Office vs Industrial interfaces
  - Glass interfaces: cheaper/flexible but loss of context

- **Interaction Styles (8 types)**
  - Command Line, Menus, Natural Language, Q&A/Query, Form-fills, Spreadsheets, WIMP, 3D

- **WIMP (Dominant Paradigm)**
  - Windows (independent areas, scrollbars, overlapping/tiled)
  - Icons (small pictures representing objects/actions)
  - Menus (pull-down, drop-down, fall-down, pop-up, pie, cascading; tear-off; keyboard accelerators)
  - Pointers (graphical cursors)
  - Buttons: radio (exclusive) vs check boxes (non-exclusive)
  - Dialog boxes: modal (pre-emptive, use sparingly) vs modeless

- **Look and Feel**: appearance + behaviour

- **Flow** (Csikszentmihalyi): optimal experience between anxiety and boredom

- **Physical Design Constraints**
  - Six types: ergonomic, physical, legal/safety, context/environment, aesthetic, economic
  - Trade-offs within and between categories
  - Fluidity: physical state reflects logical state
  - Compliant interaction: mechanical buttons reveal state visually

- **Value Equation**: use IF perceived value > cost
  - Discounted future: people discount future value → resistance to learning
  - Organizational design: coercion / enculturation / emergence

---

## Chapter 4: Paradigms — The Big Ideas That Shaped HCI

- **Paradigm Shifts Timeline**
  - Batch Processing (1940s-50s): impersonal, no direct interaction
  - Time-Sharing (1960s): one computer, many users → interactive computing
  - Networking (1960s-70s): community computing, email, file sharing
  - Graphical Displays (1962): Sutherland's Sketchpad → direct manipulation
  - Microprocessor (1970s): personal computing; Papert's LOGO; Kay's Dynabook
  - WWW (1990s): hypertext on global network; HTTP/HTML; critical mass
  - Ubiquitous Computing (1991+): Weiser — technology that disappears; symbiosis

- **Window Systems & WIMP**: Xerox Star (1981) first commercial windowing system

- **Metaphor**: relating computing to real life (turtle, desktop, spreadsheets, VR)
  - Problems: cultural bias, task mismatch

- **Direct Manipulation** (Shneiderman, 1982)
  - Visibility, incremental action, rapid feedback, reversibility, syntactic correctness
  - Replace language with action
  - Apple Mac (1984) brought to mainstream; WYSIWYG

- **Language vs Action Tension**
  - DM: interface as "world"; Language: interface as mediator; Programming by example: both

- **Hypertext**: Bush's memex (1945) → Nelson's non-linear browsing → Xanadu

- **Multimodality**: simultaneous use of multiple communication channels

- **CSCW**: Computer Supported Cooperative Work — work is social

- **Agent-Based Interfaces**: return to language with proactivity and intelligence

- **Sensor-Based & Context-Aware Interaction**: from sensed measures to "aware" behavior

---

## Chapter 5: Interaction Design Basics

- **Design Process**
  - Design = plan for making usable interactive systems
  - Collaborative: customers, users, other designers
  - User-Centered Design (UCD): involve users throughout

- **Understanding Users**
  - Personas: fictional users from research, represent real categories
  - Cultural probes: self-documentation packages for context/culture (NOT for requirements)
  - Contextual inquiry: observe + interview in natural work environment

- **Scenarios**: stories about use — concrete (specific) vs abstract (general)

- **Navigation Design**
  - 4 Golden Rules: landmarks, routes, overviews, context
  - Breadcrumbs: path shown, enables return, gives orientation
  - Modes: modal (context-dependent) vs modeless (consistent)
  - Information structures: hierarchical vs network

- **Screen Design**
  - Gestalt: proximity, similarity, closure, continuity
  - Alignment: grid-based consistency
  - White space: reduces cognitive load
  - Affordances: perceived properties that suggest use
  - Aesthetic-usability effect: attractive → perceived as working better
  - Colour: never rely on colour alone

- **Internationalisation & Localisation**
  - Internationalisation: design for multiple cultures upfront
  - Localisation: adapt per locale (dates, currency, symbols, text direction)

- **Prototyping & Iteration**
  - Fidelity: low (paper sketches) vs high (interactive)
  - Strategy: throwaway / evolutionary / incremental
  - Iteration: test → learn → improve → repeat

---

## Chapter 6: HCI in the Software Process

- **Software Lifecycle**: Requirements → Architecture → Detailed Design → Coding → Integration → Maintenance
  - Waterfall model: sequential — doesn't fit interactive systems (need feedback)

- **Verification vs Validation**
  - Verification: product right ("does it meet spec?")
  - Validation: right product ("does it solve user's problem?")
  - Formality gap: validation needs subjective judgement

- **Usability Engineering**
  - Usability specification: attribute, measuring concept, method, now/worst/planned/best levels
  - ISO 9241: effectiveness + efficiency + satisfaction

- **Iterative Design & Prototyping**
  - Why iterate: requirements always incomplete initially
  - Types: throwaway / incremental / evolutionary
  - Storyboards: visual interaction flow
  - Wizard of Oz: human simulates computer response

- **Design Rationale**: why the system is the way it is
  - Benefits: communication, reuse, discipline, trade-off analysis, organization, context
  - Process-oriented vs Structure-oriented

- **IBIS (Issue-Based Information System)**
  - Issues → Positions → Arguments (+ sub-issues)
  - gIBIS: graphical version

- **Design Space Analysis**
  - QOC: Questions, Options, Criteria (structure-oriented)
  - DRL: Design Rationale Language (formal QOC)

- **Psychological Design Rationale**: make consequences for users explicit
  - Task-artefact cycle

---

## Chapter 7: Design Rules — Principles, Standards, Heuristics

- **Spectrum of Design Rules**
  - Principles (abstract, low authority) → Guidelines → Standards (specific, high authority)

- **Three High-Level Principles**
  - Learnability, Flexibility, Robustness

- **Learnability** (5 sub-principles)
  - Predictability, Synthesizability, Familiarity, Generalizability, Consistency

- **Flexibility** (5 sub-principles)
  - Dialogue Initiative, Multithreading, Task Migratability, Substitutivity, Customizability
  - Adaptability (user changes) vs Adaptivity (system auto-adapts)

- **Robustness** (4 sub-principles)
  - Observability, Recoverability, Responsiveness, Task Conformance

- **Memory & Guidelines**
  - Lamming's "Memory Noters": external representations needed

- **Standards**: ISO 9241 (effectiveness, efficiency, satisfaction)

- **Golden Rules & Heuristics**
  - Nielsen's 10 Heuristics: visibility, real world match, user control, consistency, error prevention, recognition over recall, flexibility/efficiency, aesthetics, error recovery, help/documentation
  - Shneiderman's 8 Golden Rules: consistency, shortcuts, feedback, closure, error prevention, reversal, locus of control, reduce memory load
  - Norman's 7 Principles: knowledge in world/head, simplify tasks, visibility, mappings, constraints, design for error, standardize

- **HCI Design Patterns**
  - Originated in architecture (Christopher Alexander)
  - Pattern: invariant solution to recurrent problem within context
  - Pattern languages: link patterns for complete designs

---

## Chapter 8: Implementation Support

- **Windowing Systems**
  - Device independence + resource sharing
  - Three architectures: app-manages / kernel-manages / separate-process-manages (best portability)
  - Client-server model: clients ↔ abstract terminals ↔ server ↔ device drivers
  - X Windows (X11): client-server, separate window manager, pixel-based, X protocol

- **Programming Paradigms for Input**
  - Read-evaluation loop: modal dialogs easy, non-modal hard
  - Notification-based (callbacks): non-modal easy, modal hard
  - "Going with the grain": don't let implementation drive design

- **Interaction Toolkits**
  - Provide interaction objects (widgets/gadgets)
  - Consistency, generalizability, OO programming
  - Java AWT (native, notification-based) → Swing (on AWT, MVC)

- **UIMS (User Interface Management Systems)**
  - Separation of presentation and application semantics
  - Benefits: portability, reusability, multiple interfaces, customizability

- **Seeheim Model**
  - 3 layers: Presentation (lexical) ↔ Dialogue Control (syntactic) ↔ Functionality (semantic)
  - Switch: direct Presentation–Functionality path for rapid semantic feedback
  - Feedback levels: lexical (fast) → syntactic (medium) → semantic (slow)

- **Arch/Slinky**: 5 layers (Physical → Lexical → Dialogue → FCA → Functional Core)
  - Slinky analogy: any layer can be thicker depending on system type

- **MVC (Model-View-Controller)**
  - Model (state/data/logic), View (rendering), Controller (input)
  - Pipeline: Input → Controller → Model → View → Output
  - Problem: Controller talks to View in practice (violates clean separation)

- **PAC (Presentation-Abstraction-Control)**
  - Abstraction (like Model), Presentation (unified I/O), Control (mediates)
  - Hierarchical (vs MVC's flat); cleaner separation but less common

- **Implementation Techniques**: state diagrams, grammars, events, declarations, constraints, graphical specification
  - Constraints: declare what's true, not what happens
  - ALV: Abstraction-Link-View for groupware

- **Dialogue Control Drift**: internal → external → presentation

---

## Chapter 9: Evaluation Techniques

- **Evaluation Goals**: assess functionality, user experience, identify specific problems
- **Evaluation Throughout Lifecycle**: cheapest to fix early, most expensive late

- **Expert Evaluation (Without Users)**
  - Cognitive Walkthrough (Polson et al.)
    - 4 questions per action: goal match, visibility, recognition, feedback
    - Needs: specification/prototype, task description, action list, user description
    - Documentation: evaluation forms → usability problem reports with severity
  - Heuristic Evaluation (Nielsen & Molich)
    - 3–5 independent evaluators, severity 0–4
    - 5 evaluators find ~75% of problems
    - Nielsen's 10 Heuristics (see Ch7)
  - Model-Based Evaluation
    - GOMS: Goals, Operators, Methods, Selection
    - KLM: keystroke-level predictions (K, P, Mh, H, D, Rc, Wb, Bb operators)
  - Review-Based Evaluation: literature review supports/refutes design decisions

- **User-Based Evaluation**
  - Laboratory vs Field Studies
    - Lab: controlled, lacks context; Field: natural context, observer effect
  - Experimental Evaluation
    - Variables: IV (manipulated) vs DV (measured)
    - Null hypothesis: no difference — aim to disprove
    - Designs: between-subjects / within-subjects / mixed
    - Counterbalancing, transfer effects
    - Statistical analysis: parametric (normal) vs non-parametric (rank-based)
    - Tests: Student's t, ANOVA, regression, Wilcoxon, Spearman
    - Nielsen & Landauer: 1 user → ~33%, 5 users → ~75% of problems

- **Observational Techniques**
  - Think Aloud: user talks through actions — simple but subjective, affects performance
  - Cooperative Evaluation: user + evaluator collaborate, user encouraged to criticize
  - Protocol Analysis: paper/audio/video/logging/notebooks (mixed methods)
  - EVA: Experimental Video Annotator
  - Post-Task Walkthroughs: transcript replay (immediate or delayed)

- **Query Techniques**
  - Interviews: flexible, probe deeply, subjective, time-consuming
  - Questionnaires: quick, large groups, 5 styles (general, open-ended, scalar, multi-choice, ranked)
  - Scalar scales: 1–5 or 1–7 most effective; pilot study first
  - Validated instruments: QUIS, SUS, NASA-TLX

- **Physiological Measures**
  - Eye tracking: fixations (difficulty), saccades (movement), scan path (cognitive load)
  - GSR (arousal), EMG (task involvement), EEG (decision/attention), heart activity (stress)
  - Limitation: unclear relationship between changes and specific interaction events

- **Choosing Evaluation Methods: 8 Dimensions**
  - Stage, style, objectivity, measures, information level, immediacy, intrusiveness, resources

- **GOMS & KLM**
  - GOMS: Goals, Operators, Methods, Selection — predicts user performance
  - KLM: low-level physical task time predictions (K, P, Mh, H, D, Rc, Wb, Bb)
