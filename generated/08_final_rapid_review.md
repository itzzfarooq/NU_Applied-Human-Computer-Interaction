# FINAL RAPID REVIEW — Last 30-60 Minutes Before Exam

## Chapter 1: The Human
**Top 3 Concepts:**
1. Human info processing: Input → Memory → Processing → Output (emotion modulates)
2. Fitts' Law: Mt = a + b log₂(D/S + 1) → large targets, short distances
3. Memory: Sensory → STM (7±2 chunks, ~200ms decay) → LTM (episodic/semantic)

**Key Models:**
- LTM structures: Semantic networks (inheritance), Frames (slots), Scripts (situations), Production rules (IF-THEN)
- Reasoning: Deduction (logical), Induction (generalize, unreliable), Abduction (event→cause)
- Errors: Slips (right intention, wrong action) vs Mistakes (wrong intention)

**Critical Facts:**
- Colour blindness: 8% males, 1% females — never rely on colour alone
- Vision: rods (low light) vs cones (colour); blue acuity lowest
- Reading: saccades + fixations; negative contrast better for screens

## Chapter 2: The Computer
**Top 3 Concepts:**
1. Display specs: resolution, colour depth (bits/pixel), refresh rate
2. Colour models: RGB (additive, displays), HSB (intuitive), CMYK (subtractive, printing)
3. Input devices: mouse (relative), trackball (stationary), touchpad, joystick, pen/stylus

**Key Comparisons:**
- Text vs Graphics displays: matrix characters vs individually addressable pixels
- Speech recognition: speaker-dependent vs independent; discrete vs continuous
- Audio output: speech synthesis, earcons, auditory icons

**Screen Design:**
- Gestalt: proximity, similarity, closure, continuity
- Text: sans-serif for screens, 50-75 char lines, high contrast
- Progressive disclosure: show detail on demand

## Chapter 3: The Interaction
**Top 3 Concepts:**
1. Norman's 7 stages: goal → intention → specify → execute → perceive → interpret → evaluate
2. Gulfs: Execution (user actions ≠ system allows) vs Evaluation (user expects ≠ system shows)
3. WIMP: Windows, Icons, Menus, Pointers — dominant paradigm

**Interaction Styles:**
- CLI, menus, natural language, Q&A, forms, spreadsheets, WIMP, 3D
- Modal dialogs: pre-emptive, use sparingly

**Key Principles:**
- Value equation: use IF perceived value > cost
- Flow (Csikszentmihalyi): balance anxiety and boredom
- Physical constraints: ergonomic, physical, legal/safety, context, aesthetic, economic

## Chapter 4: Paradigms
**Top 3 Concepts:**
1. Paradigm shifts: batch → time-sharing → networking → graphical → microprocessor → WWW → ubiquitous
2. Direct manipulation (Shneiderman): visibility, incremental action, rapid feedback, reversibility
3. Ubiquitous computing (Weiser): technology that disappears, embedded in physical world

**Key Developments:**
- Sketchpad (1962): first graphical interaction
- LOGO (1970s): programming for children
- Dynabook (Kay): ultimate personal computer vision
- Xerox Star (1981): first commercial windowing system
- Hypertext: Bush's memex → Nelson's Xanadu

## Chapter 5: Interaction Design
**Top 3 Concepts:**
1. User-centered design: involve users throughout
2. Scenarios: stories about use — concrete (specific) or abstract (general)
3. Navigation: 4 golden rules — landmarks, routes, overviews, context

**Design Techniques:**
- Personas: fictional users from research
- Cultural probes: self-documentation packages
- Contextual inquiry: observe + interview in natural environment

**Screen Design:**
- Gestalt: proximity, similarity, closure, continuity
- Affordances: perceived properties that suggest use
- Aesthetic-usability effect: attractive → works better (perception)
- Internationalisation vs Localisation

## Chapter 6: Software Process
**Top 3 Concepts:**
1. Waterfall model: sequential — doesn't fit interactive systems (need feedback)
2. Verification (product right) vs Validation (right product)
3. Prototypes: throwaway, incremental, evolutionary

**Usability Engineering:**
- ISO 9241: effectiveness, efficiency, satisfaction
- Usability spec: attribute, measuring concept, method, now/worst/planned/best

**Design Rationale:**
- IBIS: Issues, Positions, Arguments (process-oriented)
- QOC: Questions, Options, Criteria (structure-oriented)
- Wizard of Oz: human simulates computer response

## Chapter 7: Design Rules
**Top 3 Concepts:**
1. Nielsen's 10 Heuristics (compact list below)
2. Shneiderman's 8 Golden Rules (compact list below)
3. Norman's 7 Principles (compact list below)

**Three Pillars:**
- Learnability: predictability, synthesizability, familiarity, generalizability, consistency
- Flexibility: dialogue initiative, multithreading, task migratability, substitutivity, customizability
- Robustness: observability, recoverability, responsiveness, task conformance

**Nielsen's 10 Heuristics:**
1. Visibility of system status
2. Match system-real world
3. User control and freedom
4. Consistency and standards
5. Error prevention
6. Recognition over recall
7. Flexibility and efficiency
8. Aesthetic and minimalist design
9. Help recover from errors
10. Help and documentation

**Shneiderman's 8 Golden Rules:**
1. Strive for consistency
2. Enable shortcuts
3. Offer informative feedback
4. Design dialogs to yield closure
5. Error prevention and simple handling
6. Permit easy reversal
7. Support internal locus of control
8. Reduce short-term memory load

**Norman's 7 Principles:**
1. Use knowledge in world and head
2. Simplify structure of tasks
3. Make things visible
4. Get mappings right
5. Exploit constraints
6. Design for error
7. Standardize when all else fails

## Chapter 8: Implementation
**Top 3 Concepts:**
1. Windowing systems: device independence + resource sharing
2. MVC: Model (state), View (rendering), Controller (input) — pipeline but controller talks to view
3. UIMS: separation of presentation and application semantics

**Architectures:**
- Seeheim: Presentation ↔ Dialogue Control ↔ Functionality (+ switch)
- Arch/Slinky: 5 layers (Physical → Lexical → Dialogue → FCA → Functional Core)
- PAC: Abstraction, Presentation (unified I/O), Control (hierarchical)

**Key Terms:**
- Toolkits: interaction objects (widgets), consistency, OO programming
- Constraints: say what's true, not what happens
- Going with grain: modal (loop-easy) vs non-modal (callbacks-easy)

## Chapter 9: Evaluation
**Top 3 Concepts:**
1. Cognitive walkthrough: 4 questions (goal match, visibility, recognition, feedback)
2. Heuristic evaluation: 3-5 independent evaluators, 10 heuristics, severity 0-4
3. GOMS/KLM: predict user performance with operators

**Evaluation Methods Comparison:**

| Method | Type | Users? | Stage | Cost | Finds |
|--------|------|--------|-------|------|-------|
| Cognitive walkthrough | Expert | No | Any | Low | Learning problems |
| Heuristic evaluation | Expert | No | Any | Low | Usability violations |
| Think aloud | User | Yes | Implementation | Medium | Subjective insights |
| Questionnaire | User | Yes | Any | Low | Preferences, satisfaction |
| Experiment | User | Yes | Implementation | High | Causal relationships |
| Eye tracking | User | Yes | Implementation | High | Visual attention |

**KLM Operators & Times:**
- K (keystroke): ~0.2-0.3s
- P (pointing): ~1.1s
- Mh (mental): ~1.35s
- H (home to device): ~0.4s
- Total = Σ(operators) + mental preparation

**Statistical Tests:**
- Parametric: assume normal (t-test, ANOVA, regression)
- Non-parametric: rank-based (Wilcoxon, Spearman)
- 5 users find ~75% of usability problems (Nielsen & Landauer)

## COMMON EXAM TRAPS
1. Confusing slips (right intention) with mistakes (wrong intention)
2. Confusing verification (product right) with validation (right product)
3. Thinking evaluation is only at the end — should be continuous
4. Assuming expert evaluation replaces user testing — both needed
5. Confusing internationalisation (design for many) with localisation (adapt for one)
6. Thinking MVC is clean in practice — controller talks to view
7. Forgetting colour blindness: never rely on colour alone
8. Confusing modal (context-dependent) with modeless (consistent)
9. Thinking more users always better — need proper experimental design
10. Confusing statistical significance with practical significance

## QUICK SELF-TEST CHECKLIST
- [ ] Can I explain Fitts' Law and its design implication?
- [ ] Can I list the 3 types of memory and their key properties?
- [ ] Can I describe Norman's 7 stages and the two gulfs?
- [ ] Can I name 3 interaction styles besides WIMP?
- [ ] Can I list the 4 golden rules of navigation?
- [ ] Can I explain the difference between verification and validation?
- [ ] Can I name 3 prototyping types and when to use each?
- [ ] Can I list Nielsen's 10 heuristics from memory?
- [ ] Can I explain the difference between cognitive walkthrough and heuristic evaluation?
- [ ] Can I describe MVC and its practical limitation?
- [ ] Can I explain KLM operators and their typical times?
- [ ] Can I name 3 physiological measures and what they track?
- [ ] Can I explain the difference between parametric and non-parametric tests?
- [ ] Can I describe the value equation from Chapter 3?
- [ ] Can I explain the concept of ubiquitous computing?