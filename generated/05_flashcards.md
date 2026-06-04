# HCI Flashcards – Chapters 1–9

---

## Chapter 1: The Human

**Q:** What is Fitts' Law and what does it predict?
**A:** Mt = a + b log₂(D/S + 1), where Mt is movement time, D is distance to target, S is size of target. It predicts the time to hit a screen target; design implications are to make targets large and distances small.

**Q:** What is the capacity of short-term memory (STM)?
**A:** 7 ± 2 chunks. STM has rapid access (~70ms) and rapid decay (~200ms).

**Q:** What are the two types of long-term memory (LTM)?
**A:** Episodic (serial memory of events) and Semantic (structured memory of facts, concepts, skills). Semantic LTM is derived from episodic LTM.

**Q:** Define slips and mistakes in human error.
**A:** Slips: right intention, wrong action (fix: better interface design). Mistakes: wrong intention due to incorrect understanding (fix: better understanding of the system).

**Q:** What is the Ponzo illusion?
**A:** Two horizontal bars of equal length placed on converging lines (like railroad tracks) make the upper bar appear longer due to depth cues.

**Q:** What is the Muller-Lyer illusion?
**A:** Two lines of equal length with different arrowhead configurations (inward vs outward) make them appear different lengths.

**Q:** What was Wason's card task designed to test?
**A:** It tests people's ability to use negative evidence in inductive reasoning. Given cards 7, E, 4, K and rule "if vowel → even number", people must turn E (check even) and 7 (check consonant), but most get it wrong.

**Q:** What is a semantic network?
**A:** A knowledge representation where concepts are nodes connected by labeled relationships. Child nodes inherit properties of parent nodes (inheritance), supporting inference.

**Q:** What is a frame in memory representation?
**A:** A data structure with slots that can be instantiated with values. Slots have fixed values (always true), default values (usually true), and variable values (change).

**Q:** What is a script?
**A:** A model of stereotypical information required to interpret a situation. Scripts have entry conditions, results, props, roles, scenes, and tracks (e.g., visiting a vet).

**Q:** What is the cocktail party phenomenon?
**A:** The ability to focus on one voice in a noisy environment, demonstrating auditory filtering.

**Q:** What are saccades and fixations in reading?
**A:** Saccades are rapid eye movements between points; fixations are pauses where perception occurs. Reading involves alternating saccades and fixations.

**Q:** What are the three types of reasoning?
**A:** Deduction (logically necessary conclusion), Induction (generalize from cases seen to unseen), Abduction (reasoning from event to cause).

**Q:** Why is negative contrast better for computer screen reading?
**A:** It improves readability and reduces eye strain compared to positive contrast (dark text on light background).

**Q:** What are the three types of sensory memory?
**A:** Iconic (visual), Echoic (aural), Haptic (tactile). They are continuously overwritten buffers for stimuli.

**Q:** What is chunking in STM?
**A:** Grouping information into meaningful units to overcome STM's 7±2 limit. Example: 0121 414 2626 is easier than 212348278493202.

**Q:** How does emotion affect problem solving?
**A:** Positive affect enables creative problem solving; negative affect narrows thinking and makes even easy tasks harder (Donald Norman).

**Q:** What is retroactive interference in LTM?
**A:** New information replaces old information, causing forgetting of the old.

**Q:** What is proactive inhibition?
**A:** Old information interferes with learning new information.

**Q:** What is the distribution of practice effect?
**A:** Learning is optimized by spreading practice over time rather than massing it together.

---

## Chapter 2: The Computer

**Q:** What is the difference between RGB and CMYK color models?
**A:** RGB (Red, Green, Blue) is additive, used in displays. CMYK (Cyan, Magenta, Yellow, Key/Black) is subtractive, used in printing where pigments absorb light.

**Q:** What is the HSB color model?
**A:** Hue (color type, 0-360°), Saturation (purity/intensity), Brightness/Value (lightness). More intuitive for users than RGB.

**Q:** What percentage of males and females are color blind?
**A:** 8% of males and 1% of females.

**Q:** What is color depth?
**A:** The number of bits per pixel. 1-bit = black & white, 8-bit = 256 colors, 24-bit = true color (16.7 million colors).

**Q:** What is gamma correction?
**A:** Compensation for the nonlinear relationship between pixel value and luminance in displays.

**Q:** What is metamerism?
**A:** Different spectral compositions can appear as the same color to the human eye.

**Q:** Why shouldn't blue be used for important detail?
**A:** Blue acuity is the lowest among color channels in human vision.

**Q:** What is anti-aliasing?
**A:** Smoothing jagged edges in graphics displays by using intermediate color values at boundaries.

**Q:** What are earcons and auditory icons?
**A:** Earcons are musical sounds representing actions/objects. Auditory icons are real-world sounds (e.g., trash can crumple sound).

**Q:** What are the four types of pointing devices compared to mouse?
**A:** Trackball (stationary, compact), Touchpad (no moving parts, laptop), Joystick (2D/3D, gaming), Pen/Stylus (direct input, natural writing).

**Q:** Why was the QWERTY keyboard layout designed?
**A:** Originally designed to prevent mechanical jamming of typewriter keys, not for typing speed optimization.

**Q:** What is the difference between speaker-dependent and speaker-independent speech recognition?
**A:** Speaker-dependent requires training to a specific voice; speaker-independent works with any voice.

**Q:** What is discrete vs continuous speech recognition?
**A:** Discrete requires one word at a time; continuous allows natural speech flow.

**Q:** What are the screen design principles for text display?
**A:** Sans-serif for screens, minimum 12pt, 50-75 characters per line, 1.2-1.5× line spacing, high contrast.

**Q:** What is progressive disclosure?
**A:** Showing detail on demand to balance information density between completeness and clutter.

---

## Chapter 3: The Interaction

**Q:** What are Norman's 7 stages of interaction?
**A:** 1) Establish goal, 2) Formulate intention, 3) Specify actions, 4) Execute action, 5) Perceive system state, 6) Interpret state, 7) Evaluate state against goal.

**Q:** Define the Gulf of Execution.
**A:** The gap between the user's formulation of actions and the actions allowed by the system.

**Q:** Define the Gulf of Evaluation.
**A:** The gap between the user's expectation of changed system state and the actual presentation of that state.

**Q:** What are the 4 components of the Abowd & Beale framework?
**A:** User (U), Input (I), System (S), Output (O). Each has its own language; interaction is translation between languages; problems = problems in translation.

**Q:** What is WIMP?
**A:** Windows, Icons, Menus, Pointers – the default interaction style for most desktop computer systems.

**Q:** Compare command line and menu-based interfaces.
**A:** Command line: direct access, better for experts, repetitive tasks, requires memorization. Menus: visible options, recognition-based, less recall, easier for novices.

**Q:** What are the two types of mutually exclusive controls?
**A:** Radio buttons (mutually exclusive choices) and Check boxes (non-exclusive choices).

**Q:** What is the difference between pull-down, drop-down, and fall-down menus?
**A:** Pull-down: mouse hold and drag. Drop-down: mouse click reveals menu. Fall-down: mouse just moves over bar.

**Q:** What are pie menus and why are they faster?
**A:** Circular menus where items are arranged around a center point. Faster because all items are equidistant from the cursor and have larger target areas.

**Q:** What are modal vs non-modal dialog boxes?
**A:** Modal: come up and won't go away until addressed (good for errors, essential steps). Non-modal: can be ignored or dismissed freely.

**Q:** What is the value equation in HCI?
**A:** People use something ONLY IF perceived value exceeds cost. Cost includes download time, money, learning effort. Future value is heavily discounted.

**Q:** What are the three types of organizational design for adoption?
**A:** Coercion (tell people what to do), Enculturation (explain values, establish support), Emergence (design process so individual value → organizational value).

**Q:** What is flow in experience design?
**A:** A state of optimal experience (Csikszentmihalyi) balancing anxiety and boredom, where the challenge matches skill level.

**Q:** What are the physical design constraints for interfaces?
**A:** Ergonomic, physical, legal/safety, context/environment, aesthetic, and economic constraints.

**Q:** What is fluidity in physical design?
**A:** Whether external physical aspects reflect logical effects – e.g., inverse actions should have inverse effects, logical state should be visible in physical state.

**Q:** What are spring-back controls?
**A:** One-shot buttons, joysticks, or sliders that return to a neutral position. Good for large selection sets but hide state.

---

## Chapter 4: Paradigms

**Q:** What is the sequence of paradigm shifts in computing?
**A:** Batch processing → Time-sharing → Networking → Graphical displays → Microprocessor → WWW → Ubiquitous computing.

**Q:** Who is credited with time-sharing and what did it enable?
**A:** J.C.R. Licklider at ARPA in the 1960s. It enabled a single computer to support multiple users with interactive computing.

**Q:** What was Sketchpad and who created it?
**A:** Created by Ivan Sutherland in 1962, it was the first graphical interaction system, demonstrating direct manipulation of visual objects on a computer.

**Q:** What was LOGO and who developed it?
**A:** Developed by Seymour Papert in the 1970s, LOGO was a programming language allowing children to create simple graphics by commanding a "turtle" to move.

**Q:** What was the Dynabook concept?
**A:** Alan Kay's vision at Xerox PARC of the ultimate personal computer – small, powerful machines dedicated to the individual.

**Q:** What was the Xerox Star and why is it significant?
**A:** Released in 1981, it was the first commercial windowing system, introducing the WIMP interface (Windows, Icons, Menus, Pointers).

**Q:** What is direct manipulation according to Shneiderman?
**A:** Defined in 1982: visibility of objects, incremental action and rapid feedback, reversibility, syntactic correctness of all actions, replacing language with action.

**Q:** What is WYSIWYG?
**A:** What You See Is What You Get – the display shows exactly what will be printed or output.

**Q:** Who proposed hypertext and when?
**A:** Vannevar Bush proposed the memex in 1945; Ted Nelson described hypertext in the mid-1960s as a non-linear browsing structure.

**Q:** What is CSCW?
**A:** Computer Supported Cooperative Work – removes the bias of single user/single computer systems, addressing social aspects of computing.

**Q:** What is ubiquitous computing according to Weiser?
**A:** "The most profound technologies are those that disappear." (Mark Weiser, 1991) – embedding computers in the physical world so they don't demand attention.

**Q:** What are agent-based interfaces?
**A:** Return to language-based interaction by instilling proactivity and intelligence in the command processor, using avatars and natural language processing.

**Q:** What is multimodality in HCI?
**A:** The simultaneous use of multiple human communication channels (modes) for input and output.

**Q:** What is context-aware interaction?
**A:** Systems that automatically sense physical phenomena (light, temperature, location, identity) and behave as if "aware" of surroundings.

**Q:** What is the difference between the direct manipulation and language paradigms?
**A:** DM: interface replaces underlying system, action-based. Language: interface as mediator, language-based. Programming by example combines both.

---

## Chapter 5: Design Basics

**Q:** What is user-centered design?
**A:** Involving users throughout the design process, understanding their tasks and requirements using multiple methods.

**Q:** What are personas?
**A:** Fictional users representing categories of real users. They give designers understanding of goals and capabilities, and help argue for design features.

**Q:** What are cultural probes?
**A:** Packages of materials sent to participants who document their own lives, helping designers understand context and culture. Not for direct requirements gathering.

**Q:** What is contextual inquiry?
**A:** Observing and interviewing users in their natural work environment to understand work practices, tools, and environment while building rapport.

**Q:** What are scenarios?
**A:** Stories about users and systems that capture what a user might do and illustrate how interaction takes place without specifying exact interface details.

**Q:** What is the difference between concrete and abstract scenarios?
**A:** Concrete scenarios: specific instances with particular users and tasks. Abstract scenarios: general patterns not tied to specific instances.

**Q:** What are the four golden rules of navigation design?
**A:** 1) Provide landmarks, 2) Provide routes, 3) Provide overviews, 4) Provide context.

**Q:** What are breadcrumbs?
**A:** Navigation elements showing the path the user has taken, allowing return to previous locations and providing context and orientation.

**Q:** What are modal vs modeless interfaces?
**A:** Modal: interface behaves differently depending on mode. Modeless: same behavior regardless of state.

**Q:** What are the Gestalt principles?
**A:** Proximity (items close = group), Similarity (items alike = group), Closure (mind completes shapes), Continuity (eye follows smooth paths).

**Q:** What is white space in screen design?
**A:** Space between elements that gives room to breathe, reduces cognitive load, improves readability and comprehension – don't fill every pixel.

**Q:** What are affordances?
**A:** Properties of an object that suggest how it can be used. A button "affords" pressing; a slider "affords" sliding. Physical objects have physical affordances; interface objects have perceived affordances.

**Q:** What is the aesthetic-usability effect?
**A:** Attractive things appear to work better – users are more tolerant of minor usability issues in aesthetically pleasing designs.

**Q:** What is the difference between internationalisation and localisation?
**A:** Internationalisation: designing for multiple cultures from the start. Localisation: adapting a product for a specific locale.

**Q:** What are the three types of prototyping?
**A:** Throwaway (built quickly, discarded), Incremental (built piece by piece), Evolutionary (evolves into final system).

**Q:** What is the Wizard of Oz technique?
**A:** A prototyping method where a human simulates the computer's response to test an interface before implementation.

**Q:** What is the advantage of storyboards?
**A:** Visual representation of user interaction flow that need not be computer-based and can be animated to explore design alternatives.

---

## Chapter 6: Software Process

**Q:** What are the 6 stages of the waterfall model?
**A:** 1) Requirements specification, 2) Architectural design, 3) Detailed design, 4) Coding and unit testing, 5) Integration and testing, 6) Operation and maintenance.

**Q:** What is the difference between verification and validation?
**A:** Verification: designing the product right (meeting specifications). Validation: designing the right product (meeting user needs).

**Q:** What is the formality gap?
**A:** Validation will always rely to some extent on subjective means of proof because it's difficult to formally specify all usability requirements.

**Q:** What is usability engineering?
**A:** The ultimate test of usability based on measurement of user experience, demanding that specific usability measures be made explicit as requirements.

**Q:** What are the four levels in a usability specification?
**A:** Now level (current state), Worst case, Planned level (target), Best case.

**Q:** What are the three categories of ISO 9241 usability?
**A:** Effectiveness (can you achieve what you want?), Efficiency (can you do it without wasting effort?), Satisfaction (do you enjoy the process?).

**Q:** Why is iterative design necessary?
**A:** It overcomes inherent problems of incomplete requirements – you don't get it right first time, so refine based on feedback.

**Q:** What is design rationale?
**A:** Information that explains why a computer system is the way it is. Benefits include communication, reuse, design discipline, and capturing trade-offs.

**Q:** What are the main elements of IBIS?
**A:** Issues (hierarchical problems), Positions (potential resolutions), Arguments (modify relationship between positions and issues). Process-oriented approach.

**Q:** What is QOC?
**A:** Questions-Options-Criteria – a structure-oriented design space analysis approach where Questions represent major issues, Options provide alternatives, and Criteria assess options.

**Q:** What are storyboards used for in prototyping?
**A:** Visual representation of user interaction flow that can be animated, need not be computer-based, and helps explore design alternatives.

**Q:** What is the Wizard of Oz method?
**A:** A prototyping technique where a human simulates the computer's response to test interface concepts before actual implementation.

**Q:** What are the benefits of design rationale?
**A:** Communication throughout lifecycle, reuse of design knowledge, enforces design discipline, presents arguments for trade-offs, organizes design space, captures contextual information.

**Q:** What is DRL?
**A:** Design Rationale Language – similar to QOC but with a larger language and more formal semantics.

---

## Chapter 7: Design Rules

**Q:** What are the three types of design rules?
**A:** Principles (abstract, low authority, high generality), Standards (specific, high authority, limited application), Guidelines (lower authority, general application).

**Q:** What are the three main principles to support usability?
**A:** Learnability (ease new users begin), Flexibility (multiplicity of ways to exchange information), Robustness (support for determining successful achievement).

**Q:** List Shneiderman's 8 Golden Rules.
**A:** 1) Strive for consistency, 2) Enable shortcuts for frequent users, 3) Offer informative feedback, 4) Design dialogs for closure, 5) Error prevention and simple handling, 6) Permit easy reversal, 7) Support internal locus of control, 8) Reduce short-term memory load.

**Q:** List Norman's 7 Principles.
**A:** 1) Use knowledge in world and head, 2) Simplify task structure, 3) Make things visible (bridge gulfs), 4) Get mappings right, 5) Exploit constraints, 6) Design for error, 7) Standardize when all else fails.

**Q:** What is the difference between adaptability and adaptivity?
**A:** Adaptability: user modifies the UI (user-driven). Adaptivity: system modifies the UI (system-driven). Both are forms of customizability.

**Q:** What is predictability in learnability?
**A:** The ability to determine the effect of future actions based on past interaction history.

**Q:** What is synthesizability?
**A:** The ability to assess the effect of past actions – immediate vs eventual honesty.

**Q:** What is dialogue initiative?
**A:** Freedom from system-imposed constraints on input dialogue – who has control, system vs user pre-emptiveness.

**Q:** What is multithreading?
**A:** The ability of a system to support user interaction for more than one task at a time – concurrent or interleaving.

**Q:** What is task migratability?
**A:** Passing responsibility for task execution between user and system.

**Q:** What is substitutivity?
**A:** Allowing equivalent values of input and output to be substituted for each other – representation multiplicity.

**Q:** What is observability in robustness?
**A:** The ability of the user to evaluate the internal state of the system from its perceivable representation.

**Q:** What is recoverability?
**A:** The ability of the user to take corrective action once an error has been recognized – includes forward/backward recovery.

**Q:** What is responsiveness?
**A:** How the user perceives the rate of communication with the system.

**Q:** What are HCI design patterns?
**A:** Invariant solutions to recurrent problems within specific contexts, originated in architecture (Alexander). Patterns capture design practice, not theory.

**Q:** What is a pattern language?
**A:** A collection of patterns linked together that enable complete designs to be generated – a generative tool.

**Q:** What is the relationship between consistency and learnability?
**A:** Consistency is a learnability principle – likeness in input/output behavior arising from similar situations or task objectives helps users predict system behavior.

---

## Chapter 8: Implementation

**Q:** What are the two main programming paradigms for windowing systems?
**A:** Read-evaluation loop (repeat read-event → process → quit) and Notification-based (register callbacks, notifier dispatches to handlers).

**Q:** What is the difference between read-evaluation loop and notification-based?
**A:** Read-eval: explicit loop reading events and processing via case statement. Notification: register callback functions, system calls them when events occur.

**Q:** How does "going with the grain" affect design?
**A:** Modal dialogs are easy with event-loop (extra read), hard with notification (mode flags). Non-modal dialogs are hard with event-loop (complex main loop), easy with notification (extra handler).

**Q:** What is X Windows architecture?
**A:** Client-server model: application client → X11 server → device drivers → hardware. Separate window manager client enforces I/O policies.

**Q:** What are the three layers of the Seeheim model?
**A:** Presentation (lexical), Dialogue Control (syntactic), Functionality/Semantic (application interface), connected by a switch.

**Q:** What are the three feedback levels?
**A:** Lexical (mouse movement), Syntactic (menu highlights), Semantic (data changes like sum of numbers).

**Q:** What is MVC?
**A:** Model-View-Controller – Model holds internal state, View renders on screen, Controller processes input. Data flows: Model→View, Controller→Model, View↔Controller.

**Q:** What is the PAC model?
**A:** Abstraction (logical state), Presentation (manages I/O), Control (mediates between them). Closer to Seeheim, manages hierarchy, cleaner separation than MVC.

**Q:** What is a UIMS?
**A:** User Interface Management System – adds abstraction above toolkits, separating presentation from application semantics for portability, reusability, multiple interfaces, and customizability.

**Q:** What are the benefits of separating presentation from semantics?
**A:** Portability (runs on different systems), Reusability (components reused), Multiple interfaces (same functionality), Customizability (by designer and user).

**Q:** What is the Arch/Slinky model?
**A:** Physical → Lexical → Dialogue → Functional core adaptor → Functional core. Like a slinky spring – different layers are thicker (more important) in different systems.

**Q:** What is the bypass/switch in Seeheim?
**A:** Direct communication between application and presentation for rapid semantic feedback, regulated by dialogue control.

**Q:** Why does the controller "talk" to the view in MVC?
**A:** Because input only has meaning in relation to output – you need to know what was clicked (view knows what's shown where), so separation isn't complete in practice.

**Q:** What are interaction toolkits?
**A:** Libraries providing interaction objects (widgets/gadgets) that promote consistency and generalizability through similar look and feel, amenable to OO programming.

**Q:** What is the difference between AWT and Swing in Java?
**A:** AWT: Abstract Windowing Toolkit, notification-based, lower level. Swing: built on AWT, higher level features, uses MVC architecture.

**Q:** What is dialogue control drift?
**A:** Three levels: Internal control (e.g., read-eval loop), External control (independent of application/presentation), Presentation control (e.g., graphical specification).

**Q:** What are constraints in UI implementation?
**A:** Instead of specifying what happens, specify what should be true. Used in groupware as well as single user interfaces (ALV – abstraction-link-view).

---

## Chapter 9: Evaluation

**Q:** What are the three goals of evaluation?
**A:** 1) Assess extent of system functionality, 2) Assess effect of interface on user, 3) Identify specific problems.

**Q:** What is a cognitive walkthrough?
**A:** An expert walks through a design evaluating how well it supports user learning, using psychological principles to identify potential problems.

**Q:** What is heuristic evaluation?
**A:** Experts examine a design against usability heuristics (e.g., predictability, consistency, feedback) to identify violations – it "debugs" design.

**Q:** What is the difference between laboratory and field studies?
**A:** Lab: specialist equipment, uninterrupted, but lacks context. Field: natural environment, context retained, longitudinal possible, but distractions and noise.

**Q:** What is an independent variable (IV)?
**A:** The characteristic changed to produce different experimental conditions (e.g., interface style, number of menu items).

**Q:** What is a dependent variable (DV)?
**A:** The characteristic measured in the experiment (e.g., time taken, number of errors).

**Q:** What is a null hypothesis?
**A:** States there is no difference between conditions – the aim of the experiment is to disprove it.

**Q:** What is the difference between within-groups and between-groups design?
**A:** Within-groups: each subject performs under each condition (transfer possible, less costly). Between-groups: each subject under one condition (no transfer, more users needed).

**Q:** What are parametric vs non-parametric tests?
**A:** Parametric: assume normal distribution, robust, powerful. Non-parametric: no normal distribution assumption, less powerful, more reliable.

**Q:** What is the think aloud method?
**A:** User performs task while describing what they're doing, why, and what they think is happening. Simple but subjective and may alter performance.

**Q:** What is cooperative evaluation?
**A:** Variation on think aloud where user and evaluator collaborate, both can ask questions. Less constrained, user encouraged to criticize system.

**Q:** What is EVA?
**A:** Evaluator-based approach – a post-task walkthrough where the user reacts to their actions after the event, allowing the analyst to focus on relevant incidents.

**Q:** What are the two types of eye tracking measurements?
**A:** Fixations (stable position, duration indicates difficulty) and Saccades (rapid movement between points). Scan paths show optimal movement patterns.

**Q:** What are the seven dimensions for choosing an evaluation method?
**A:** When in process, Style (lab/field), How objective, Type of measures (qual/quant), Level of information, Level of interference, Resources available.

**Q:** What is distributed cognition?
**A:** Studying work in context, recognizing that cognition is distributed across people, tools, and environment rather than just in the individual's head.

**Q:** What is situated action?
**A:** Real action where the physical and social environment are both crucial to understanding behavior.

**Q:** What are the protocol analysis methods?
**A:** Paper and pencil (cheap, limited), Audio (good for think aloud), Video (accurate, obtrusive), Computer logging (automatic, large data), User notebooks (coarse, longitudinal).

**Q:** What are the five observational methods?
**A:** Think Aloud, Cooperative Evaluation, Protocol Analysis, Automated Analysis (EVA), Post-task Walkthroughs.

**Q:** What are the advantages of questionnaires over interviews?
**A:** Quick, reaches large groups, can be analyzed more rigorously. But less flexible and less probing than interviews.

**Q:** What are the physiological measurement methods?
**A:** Heart activity (blood pressure, pulse), Galvanic Skin Response (sweat glands), Electromyogram (muscle activity), Electroencephalogram (brain activity).

**Q:** What is the difference between subjective and objective evaluation?
**A:** Subjective: based on user opinions and feelings. Objective: based on measurable performance data like time, errors, and task completion.

**Q:** What are the 4 components of GOMS?
**A:** 1) Goals (what the user wants to achieve), 2) Operators (primitive physical/mental actions like keystrokes and clicks), 3) Methods (sequences of operators that accomplish a goal), 4) Selection rules (choose between alternative methods when multiple exist).

**Q:** What are the KLM operators? (list with symbols)
**A:** K (Keystroke, ~0.2s), P (Pointing, ~1.1s), Mh (Mental hesitation, ~1.35s), H (Home hand to device, ~0.4s), D (Draw on screen, varies), Rc (System response wait, varies), Wb (Write by hand, ~1.5s/char), Bb (Browse/scroll button, ~0.2s).

**Q:** What are Nielsen's severity ratings (0-4)?
**A:** 0 = Not a usability problem, 1 = Cosmetic (fix only if extra time), 2 = Minor (low priority), 3 = Major (high priority, important to fix), 4 = Catastrophe (must fix before release).

**Q:** What are the 8 factors for choosing an evaluation method?
**A:** 1) Stage in cycle (design vs implementation), 2) Style (lab vs field), 3) Objectivity (subjective vs objective), 4) Measures (quantitative vs qualitative), 5) Information level (low vs high), 6) Immediacy (during vs post-hoc), 7) Intrusiveness (obtrusive vs unobtrusive), 8) Resources (time, money, equipment, participants).

**Q:** What are the 4 questions in a cognitive walkthrough?
**A:** 1) Is the effect of the action the same as the user's goal at that point? 2) Will users see that the action is available? 3) Once users have found the correct action, will they know it is the one they need? 4) After the action is taken, will users understand the feedback?
