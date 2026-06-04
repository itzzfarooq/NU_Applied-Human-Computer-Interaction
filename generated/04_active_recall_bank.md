# Active Recall Question Bank — Applied HCI (Chapters 1–9)

---

## Chapter 1: The Human

### Definitions (What is X?)

**Q1.** Define Fitts' Law. What are the variables, and what design rule does it imply?
> **A:** Mt = a + b log₂(D/S + 1), where D = distance to target, S = target size. Design rule: make targets large and distances short.

**Q2.** What is the cocktail party phenomenon?
> **A:** The ability to focus on one auditory source (voice) while filtering out background noise. Demonstrates selective attention.

**Q3.** What is chunking?
> **A:** Grouping individual items into meaningful units to fit more information into STM. E.g., 212348278493202 → 0121 414 2626.

**Q4.** What is a semantic network in the context of LTM?
> **A:** A model where knowledge is stored as nodes with inheritance — child nodes inherit properties from parent nodes (e.g., COLLIE inherits "barks" from DOG).

**Q5.** What is a script?
> **A:** A stereotypical situation structure with entry conditions, props, roles, scenes, and tracks. E.g., visiting a vet: dog ill → vet examines → owner pays.

**Q6.** What is kinesthesia?
> **A:** Awareness of body position. It affects comfort and performance in physical interaction.

### Comparisons (How does X differ from Y?)

**Q7.** How do slips differ from mistakes?
> **A:** Slips: correct goal, wrong action (fix: better interface design). Mistakes: wrong goal (fix: better understanding/mental model).

**Q8.** Contrast STM and LTM on access speed, decay, and capacity.
> **A:** STM: fast access (~70ms), rapid decay (~200ms), limited capacity (7±2). LTM: slow access (~100ms), practically permanent, unlimited capacity.

**Q9.** What is the difference between episodic and semantic memory?
> **A:** Episodic: serial memory of events (autobiographical). Semantic: structured memory of facts, concepts, skills (derived from episodic).

**Q10.** Contrast retroactive and proactive interference.
> **A:** Retroactive: new info replaces old. Proactive: old info interferes with new.

**Q11.** How do recall and recognition differ?
> **A:** Recall: reproduce from memory (aided by cues), harder. Recognition: identify as previously seen, easier.

### Applications (Scenario-based)

**Q12.** A designer wants users to quickly tap a button on a mobile screen. Applying Fitts' Law, what two things should the designer do?
> **A:** Make the target (button) large and place it close to the user's current position (short distance).

**Q13.** You're designing a phone number entry field. How does the concept of chunking apply?
> **A:** Group digits into chunks (e.g., (555) 123-4567) to improve memorability and reduce STM load.

**Q14.** A user accidentally presses Ctrl+Z when meaning to press Ctrl+X. Is this a slip or a mistake? Why?
> **A:** A slip — the user had the correct goal (cut) but performed the wrong action. The fix is better interface design (e.g., clearer labels).

### True/False

**Q15.** True or False: Blue acuity is the highest among all colours.
> **A:** False. Blue acuity is the lowest. Don't use blue for critical detail.

**Q16.** True or False: The human visual system perceives light that enters the eye as right-side-up.
> **A:** False. Light is focused upside-down on the retina; the brain inverts the image.

**Q17.** True or False: 8% of females and 1% of males are colour blind.
> **A:** False. It's 8% of males and 1% of females.

### Fill-in-the-Blank

**Q18.** The capacity of short-term memory is approximately ___ ± ___ chunks.
> **A:** 7 ± 2

**Q19.** Sensory memory types include ___ (visual), ___ (aural), and ___ (tactile).
> **A:** Iconic, Echoic, Haptic

**Q20.** Reaction time to a visual stimulus is approximately ___ milliseconds.
> **A:** ~200ms

---

## Chapter 2: The Computer

### Definitions

**Q21.** What is colour depth?
> **A:** The number of bits per pixel used to represent colour. 1-bit = B&W, 8-bit = 256 colours, 24-bit = true colour (16.7M colours).

**Q22.** What is an earcon?
> **A:** A musical sound that represents an action or object in the interface, used as audio output.

**Q23.** What is anti-aliasing?
> **A:** A technique that smooths jagged edges in displayed graphics by using intermediate colour values.

**Q24.** What is metamerism?
> **A:** The phenomenon where different spectral compositions can appear as the same colour to the human eye.

### Comparisons

**Q25.** How do RGB, HSB, and CMYK colour models differ?
> **A:** RGB: additive (combines light), used for displays. HSB: intuitive for human design (hue/saturation/brightness). CMYK: subtractive (absorbs light), used for printing.

**Q26.** Compare text displays and graphics displays.
> **A:** Text displays: characters from fixed matrix, fast to render, limited. Graphics displays: each pixel addressable, arbitrary shapes/fonts/images, more memory needed.

**Q27.** How does a mouse differ from a trackball in terms of use case?
> **A:** Mouse: relative movement on flat surface, best for direct manipulation. Trackball: stationary ball moved by fingers, best for compact spaces.

**Q28.** Contrast earcons with auditory icons.
> **A:** Earcons: abstract musical sounds representing actions. Auditory icons: real-world sounds mapped to actions (e.g., crumpling paper = delete).

### Applications

**Q29.** A website uses red text for links and green text for confirmed actions. A colour-blind user (8% of males) cannot distinguish them. What principle is violated and what should the designer do?
> **A:** Never rely on colour alone. Use redundant cues: different shapes, patterns, or text labels alongside colour.

**Q30.** Designing a laptop touchpad interface — why is the pen/stylus's occlusion problem relevant?
> **A:** When using a pen on screen, the user's hand blocks the view of what they're drawing. Design must account for this by providing offset cursors or UI that avoids obscured areas.

### True/False

**Q31.** True or False: QWERTY was designed to maximize typing speed.
> **A:** False. QWERTY was designed to prevent mechanical jamming in typewriters, not for speed.

**Q32.** True or False: The human hearing range is 20Hz to 20kHz.
> **A:** False. It's 20Hz to 15kHz.

### Fill-in-the-Blank

**Q33.** Sound has three properties: ___ (frequency), ___ (amplitude), and ___ (quality).
> **A:** Pitch, Loudness, Timbre

**Q34.** Speech recognition can be speaker-___ or speaker-___; discrete or ___.
> **A:** Dependent, independent, continuous

---

## Chapter 3: The Interaction

### Definitions

**Q35.** What is the Gulf of Execution?
> **A:** The gap between the user's intended actions and what the system actually allows. E.g., wanting to save but not finding the save button.

**Q36.** What is the Gulf of Evaluation?
> **A:** The gap between the user's expected feedback and what the system actually shows. E.g., pressing save but seeing no confirmation.

**Q37.** What is a modal dialog box?
> **A:** A dialog that demands attention and blocks other interaction until dismissed. It is pre-emptive — good for errors, use sparingly.

**Q38.** What is WIMP?
> **A:** Windows, Icons, Menus, Pointers — the dominant interaction paradigm for desktop computing.

**Q39.** What is flow (Csikszentmihalyi)?
> **A:** The optimal experience state between anxiety and boredom, where a user is fully engaged.

### Comparisons

**Q40.** How do Norman's model and Abowd & Beale's framework differ in their view of interaction?
> **A:** Norman: user's view — 7-stage execution/evaluation cycle with gulfs. Abowd & Beale: system's view — translation between 4 languages (User, Input, System, Output).

**Q41.** Compare radio buttons and check boxes.
> **A:** Radio buttons: mutually exclusive (choose one). Check boxes: non-exclusive (choose many).

**Q42.** Contrast modal and modeless dialog boxes.
> **A:** Modal: pre-emptive, blocks other interaction, good for errors. Modeless: non-blocking, user can interact elsewhere.

**Q43.** How do the 8 interaction styles differ in learnability vs expert efficiency?
> **A:** CLI: low learnability, high efficiency. Menus/NL: high learnability, low efficiency. WIMP: moderate both. Forms: high learnability, moderate efficiency.

### Applications

**Q44.** A user wants to delete a file but can't find the delete option. Which gulf does this represent?
> **A:** Gulf of Execution — the user's intended action (delete) isn't available in a way they can find.

**Q45.** After clicking "Send" on an email, the screen shows no confirmation. The user is unsure if it sent. Which gulf? Is this a slip or mistake?
> **A:** Gulf of Evaluation. This relates to a potential mistake if the user sends again thinking it didn't work (wrong mental model of the feedback system).

### True/False

**Q46.** True or False: Pie menus are widely used in modern interfaces.
> **A:** False. Pie menus are arranged in a circle (larger targets, equal distance) but are not widely adopted.

**Q47.** True or False: WIMP stands for Windows, Icons, Menus, and Programs.
> **A:** False. WIMP = Windows, Icons, Menus, Pointers.

### Fill-in-the-Blank

**Q48.** Norman's 7 stages are: goal → intention → specify → ___ → perceive → interpret → ___.
> **A:** Execute, Evaluate

**Q49.** The value equation states that people use something ONLY IF perceived ___ exceeds ___.
> **A:** Value, Cost

---

## Chapter 4: Paradigms

### Definitions

**Q50.** What is direct manipulation (Shneiderman, 1982)?
> **A:** Interaction with a visual representation of objects using visible actions, incremental feedback, and reversibility. Properties: visibility, incremental action, rapid feedback, reversibility, syntactic correctness.

**Q51.** What is ubiquitous computing?
> **A:** Computing technology that disappears into the physical environment (Weiser, 1991). Goal: symbiosis of physical and electronic worlds.

**Q52.** What is WYSIWYG?
> **A:** "What You See Is What You Get" — the screen shows exactly what the printed/final output will look like.

**Q53.** What is hypertext?
> **A:** A non-linear browsing structure for information, where documents contain links to other documents. Pioneered by Ted Nelson; applied by Tim Berners-Lee in the WWW.

### Comparisons

**Q54.** How does direct manipulation differ from language-based interaction?
> **A:** DM: act on a visual "world" (drag file to trash). Language: type commands to a mediator (type "delete file.txt"). DM is more intuitive; language is more powerful for experts.

**Q55.** Contrast batch processing with time-sharing.
> **A:** Batch: submit job, wait, get results — no interaction. Time-sharing: one computer, many users, interactive terminals — real-time dialogue.

**Q56.** How do metaphor-based interfaces differ from direct manipulation?
> **A:** Metaphor: relate computing to real life (desktop). DM: act directly on visible objects. Metaphor can carry cultural bias; DM emphasizes visibility and feedback.

### Applications

**Q57.** The Apple Macintosh (1984) is cited as bringing a paradigm to the mainstream. Which paradigm?
> **A:** Direct manipulation.

**Q58.** A smart home system adjusts the thermostat based on learned user preferences without explicit commands. Which paradigm concept does this exemplify?
> **A:** Ubiquitous computing / context-aware interaction / sensor-based interaction.

### True/False

**Q59.** True or False: Ivan Sutherland's Sketchpad was developed in 1982.
> **A:** False. Sketchpad was developed in 1962.

**Q60.** True or False: CSCW removes the bias of single-user / single-computer systems.
> **A:** True.

### Fill-in-the-Blank

**Q61.** Mark Weiser's vision of ___ computing states that the most profound technologies are those that ___.
> **A:** Ubiquitous, disappear

**Q62.** Tim Berners-Lee combined ___ with the global network using simple protocols: ___ and ___.
> **A:** Hypertext, HTTP, HTML

---

## Chapter 5: Interaction Design Basics

### Definitions

**Q63.** What is user-centered design (UCD)?
> **A:** Design approach that involves users throughout the entire design process, understanding their tasks, environment, and requirements.

**Q64.** What is a persona?
> **A:** A fictional user based on research that represents a real user category. Gives designers a concrete person to design for.

**Q65.** What is a cultural probe?
> **A:** A package sent to participants to document their own lives. Used for early exploration of context/culture — NOT for direct requirements gathering.

**Q66.** What is an affordance?
> **A:** A property of an object that suggests how it can be used. Interface objects have perceived affordances (learned, not innate).

**Q67.** What is internationalisation?
> **A:** Designing for multiple cultures from the start, before building.

**Q68.** What is localisation?
> **A:** Adapting a product for a specific locale (dates, currency, symbols, text direction).

### Comparisons

**Q69.** How do concrete and abstract scenarios differ?
> **A:** Concrete: specific instance with particular user and task. Abstract: general pattern not tied to a specific instance.

**Q70.** Contrast throwaway, evolutionary, and incremental prototyping.
> **A:** Throwaway: build quickly, discard after learning. Evolutionary: prototype evolves into final product. Incremental: build piece by piece, add to final system.

**Q71.** How do cultural probes differ from contextual inquiry?
> **A:** Cultural probes: self-documentation for context/culture inspiration (not requirements). Contextual inquiry: observe + interview users in their natural work environment.

### Applications

**Q72.** Which 4 Golden Rules of Navigation are implemented by breadcrumbs?
> **A:** All four: landmarks (where am I), routes (path taken), overviews (structure), context (relationship to other parts).

**Q73.** A designer is building a shopping app for international users. What should they consider for text-heavy interfaces?
> **A:** Text direction (RTL for Arabic/Hebrew), date/time formats, currency symbols, cultural colour meanings, localised imagery.

### True/False

**Q74.** True or False: Gestalt principle of proximity states that similar items are perceived as a group.
> **A:** False. Proximity: close items are perceived as a group. Similarity: similar items are perceived as a group.

**Q75.** True or False: The aesthetic-usability effect means attractive interfaces are perceived as working better.
> **A:** True.

### Fill-in-the-Blank

**Q76.** The four Golden Rules of Navigation are: landmarks, ___, overviews, and ___.
> **A:** Routes, Context

**Q77.** Prototyping strategies include throwaway, ___, and ___.
> **A:** Evolutionary, Incremental

---

## Chapter 6: HCI in the Software Process

### Definitions

**Q78.** What is the waterfall model?
> **A:** A traditional software lifecycle where development proceeds sequentially: Requirements → Architecture → Design → Coding → Integration → Maintenance.

**Q79.** What is verification?
> **A:** "Designing the product right" — does it meet the specification?

**Q80.** What is validation?
> **A:** "Designing the right product" — does it solve the user's actual problem?

**Q81.** What is the formality gap?
> **A:** The observation that validation always relies on subjective proof — you can't fully automate "is this good for users?"

**Q82.** What is a Wizard of Oz prototype?
> **A:** A human simulates the computer's response behind the scenes. The user thinks they're interacting with a real system.

**Q83.** What is IBIS?
> **A:** Issue-Based Information System — a process-oriented design rationale approach using Issues, Positions, and Arguments.

### Comparisons

**Q84.** How does the waterfall model conflict with HCI design needs?
> **A:** Waterfall assumes all requirements are known upfront. HCI needs iterative feedback loops — you can't know the right interface until users try it.

**Q85.** Contrast verification and validation with an example.
> **A:** Verification: "Does the save button work per spec?" Validation: "Does the save workflow actually solve the user's need to preserve their work?"

**Q86.** Compare IBIS and QOC approaches to design rationale.
> **A:** IBIS: process-oriented, preserves the journey of deliberation (Issues→Positions→Arguments). QOC: structure-oriented, maps the design space after the fact (Questions→Options→Criteria).

### Applications

**Q87.** You're building a medical records system. Early requirements specify the interface, but user testing shows doctors can't find the patient history quickly. What approach from Chapter 6 addresses this?
> **A:** Iterative design with prototyping — the initial requirements were incomplete. Use user testing to feed back into redesign. Also, design rationale (IBIS/QOC) captures why decisions were made.

**Q88.** Usability specification for a VCR undo feature: planned level = maximum 2 explicit user actions. What are the now, worst, and best case levels?
> **A:** Now: no product allows undo. Worst: as many actions as needed to program it in. Best: one explicit cancel action.

### True/False

**Q89.** True or False: The waterfall model works well for interactive systems.
> **A:** False. It doesn't allow for the feedback loops HCI requires.

**Q90.** True or False: ISO 9241 defines usability as effectiveness, efficiency, and satisfaction.
> **A:** True.

### Fill-in-the-Blank

**Q91.** ISO 9241 usability has three dimensions: ___, ___, and ___.
> **A:** Effectiveness, Efficiency, Satisfaction

**Q92.** Design rationale approaches include process-oriented (___) and structure-oriented (___).
> **A:** IBIS, QOC

---

## Chapter 7: Design Rules

### Definitions

**Q93.** What are Nielsen's 10 Usability Heuristics? (Name at least 5)
> **A:** 1) Visibility of system status, 2) Match system and real world, 3) User control and freedom, 4) Consistency and standards, 5) Error prevention, 6) Recognition over recall, 7) Flexibility and efficiency of use, 8) Aesthetic and minimalist design, 9) Help recognize/diagnose/recover from errors, 10) Help and documentation.

**Q94.** What is predictability (as a learnability sub-principle)?
> **A:** Can the user determine the effect of future actions from past experience? E.g., "Save" button always works the same way.

**Q95.** What is customizability in the context of flexibility?
> **A:** The UI can be modified. Two types: Adaptability (user changes settings) vs Adaptivity (system auto-adapts).

**Q96.** What is an HCI design pattern?
> **A:** An invariant solution to a recurrent problem within a specific context, originated in architecture (Christopher Alexander).

### Comparisons

**Q97.** How do principles, guidelines, and standards differ?
> **A:** Principles: abstract, high generality, low authority. Guidelines: moderate. Standards: specific, high authority, narrow situations.

**Q98.** Contrast Shneiderman's 8 Golden Rules with Norman's 7 Principles.
> **A:** Shneiderman: practical rules (consistency, shortcuts, feedback, closure, error prevention, reversal, locus of control, memory). Norman: theoretical principles (knowledge in world/head, simplify tasks, visibility, mappings, constraints, design for error, standardize).

**Q99.** How do Nielsen's heuristics relate to the three high-level principles (Learnability, Flexibility, Robustness)?
> **A:** Nielsen's heuristics operationalize these principles. E.g., "Recognition over recall" supports Learnability; "Flexibility and efficiency" supports Flexibility; "Error prevention" supports Robustness.

### Applications

**Q101.** A user fills a form and presses Enter, but nothing happens and no feedback appears. Which heuristic is violated?
> **A:** Visibility of system status — every action should have a visible result.

**Q102.** A design uses red for errors and green for success, but 8% of male users can't distinguish them. Which heuristic is violated?
> **A:** Heuristic: "Match between system and real world" (colour alone).

### True/False

**Q103.** True or False: Five heuristic evaluators find approximately 75% of usability problems.
> **A:** True (from Ch9, but heuristics are defined in Ch7).

### Fill-in-the-Blank

**Q105.** The three high-level usability principles are: ___, ___, and ___.
> **A:** Learnability, Flexibility, Robustness

**Q106.** Adaptability is when the ___ changes settings; Adaptivity is when the ___ auto-adapts.
> **A:** User, System

---

## Chapter 8: Implementation Support

### Definitions

**Q107.** What is a windowing system?
> **A:** Software providing device independence (abstract interface to screens/keyboards/mice) and resource sharing (multiple apps in windows simultaneously).

**Q108.** What is a UIMS?
> **A:** User Interface Management System — enforces separation between presentation (how it looks) and application semantics (what it does).

**Q109.** What is the Seeheim Model?
> **A:** A 3-layer UIMS architecture: Presentation (lexical) ↔ Dialogue Control (syntactic) ↔ Functionality (semantic), with a switch for rapid feedback.

**Q110.** What is MVC?
> **A:** Model-View-Controller — a pattern separating internal state (Model), screen rendering (View), and input processing (Controller).

**Q111.** What is PAC?
> **A:** Presentation-Abstraction-Control — a pattern where Presentation handles unified I/O, Abstraction holds logical state, and Control mediates. Hierarchical (vs MVC's flat).

**Q112.** What does "going with the grain" mean?
> **A:** Choosing the implementation paradigm that fits your interaction style, rather than letting the implementation drive the design.

### Comparisons

**Q113.** How do read-evaluation loops and notification-based (callback) paradigms differ?
> **A:** Read-evaluation loop: modal dialogs easy (nested loop), non-modal hard. Callbacks: non-modal easy (add handler), modal hard (mode flags).

**Q114.** Contrast MVC and PAC.
> **A:** MVC: split I/O (Controller + View), flat, more common. PAC: unified I/O (Presentation), hierarchical, cleaner separation but less used.

**Q115.** How does Arch/Slinky extend the Seeheim Model?
> **A:** Adds 2 layers: Physical (raw hardware) and Functional Core Adaptor (adapts app API). 5 layers total. The "Slinky" analogy: any layer can be thicker.

### Applications

**Q116.** You're building a drawing app with complex rendering. According to Arch/Slinky, which layer would likely be thickest?
> **A:** Physical and Lexical layers — complex rendering requires heavy presentation logic.

**Q117.** A team builds a desktop app, then needs a mobile version. Which UIMS benefit does the separation of presentation and semantics provide?
> **A:** Portability — same application logic, different presentation layer for mobile.

### True/False

**Q118.** True or False: In MVC, the Controller never talks to the View in practice.
> **A:** False. In practice, the Controller talks to the View because input only has meaning relative to what's displayed.

**Q119.** True or False: The window manager is a separate client in X Windows.
> **A:** True.

### Fill-in-the-Blank

**Q120.** The Seeheim Model has three layers: ___, ___, and ___.
> **A:** Presentation, Dialogue Control, Functionality

**Q121.** Feedback levels in Seeheim: lexical (___), syntactic (___), semantic (___).
> **A:** Fast, Medium, Slowest

---

## Chapter 9: Evaluation Techniques

### Definitions

**Q122.** What is a cognitive walkthrough?
> **A:** An expert evaluation method where evaluators analyze a task sequence using 4 questions: goal match, visibility, recognition, feedback.

**Q123.** What is heuristic evaluation?
> **A:** Multiple independent evaluators (3-5) rate a system against usability heuristics, with severity ratings 0-4.

**Q124.** What is GOMS?
> **A:** Goals, Operators, Methods, Selection — a model-based evaluation predicting user performance with an interface.

**Q125.** What is the null hypothesis?
> **A:** The assumption of no difference between conditions. The aim of statistical analysis is to disprove it.

**Q126.** What is a within-subjects design?
> **A:** Each participant experiences all experimental conditions. Fewer users needed but transfer effects possible (mitigate with counterbalancing).

**Q127.** What is think aloud?
> **A:** A technique where the user verbalizes their thoughts while performing tasks, providing insight into their reasoning.

### Comparisons

**Q128.** How does cognitive walkthrough differ from heuristic evaluation?
> **A:** CW: step-by-step task analysis with 4 questions, focuses on learning. HE: global critique against 10 heuristics, focuses on principle violations.

**Q129.** Contrast laboratory and field studies.
> **A:** Lab: controlled, specialist equipment, lacks context. Field: natural environment, context retained, observer effect applies.

**Q130.** How do parametric and non-parametric statistical tests differ?
> **A:** Parametric: assume normal distribution, more powerful but fragile if violated. Non-parametric: no distribution assumption, rank-based, reliable but less powerful.

**Q131.** Compare between-subjects and within-subjects designs.
> **A:** Between: each subject does one condition (no transfer, more users needed). Within: each subject does all conditions (transfer possible, fewer users, counterbalancing needed).

**Q132.** How do the 8 dimensions for choosing evaluation methods help?
> **A:** They guide method selection based on: stage, style (lab/field), objectivity, measures (quant/qual), information level, immediacy, intrusiveness, resources.

### Applications

**Q133.** You have a working prototype and want to find the most usability problems with the fewest evaluators. How many should you use and why?
> **A:** 5 evaluators — Nielsen found they discover approximately 75% of overall usability problems.

**Q134.** A researcher wants to compare two menu designs. They give 20 participants each menu. Which design type is this and what statistical test should they use?
> **A:** Between-subjects design (each participant uses one menu). Use Student's t-test (two-valued IV + continuous DV like completion time).

**Q135.** You're testing a medical device interface in a hospital. Why might field study be preferred over lab study?
> **A:** Natural context is crucial — the hospital environment (noise, interruptions, real patients) affects how the device is actually used. Lab would lack ecological validity.

**Q136.** A questionnaire uses a 1-5 Likert scale. Why is 1-5 preferred over 1-3 or 1-10?
> **A:** 1-5: fine enough for differentiation, clear meaning. 1-3: too coarse, no room for varying agreement. 1-10: inconsistent across users, hard to distinguish levels.

### True/False

**Q137.** True or False: Nielsen & Landauer found that 5 users find about 75% of usability problems.
> **A:** True.

**Q138.** True or False: Think aloud does not affect user performance.
> **A:** False. It changes how people perform tasks — the "centipede effect."

**Q139.** True or False: Statistical significance always implies practical significance.
> **A:** False. A statistically significant result may have a trivially small effect size.

**Q140.** True or False: You should always use parametric tests because they are more powerful.
> **A:** False. They require normal distribution. If the assumption is violated, results are invalid. Non-parametric tests are safer.

### Fill-in-the-Blank

**Q141.** Nielsen's severity ratings range from ___ (not a problem) to ___ (catastrophe).
> **A:** 0, 4

**Q142.** GOMS stands for Goals, ___, Methods, and ___.
> **A:** Operators, Selection

**Q143.** Two rules of statistical analysis: ___ at your data and ___ your data.
> **A:** Look, Save

**Q144.** The three goals of evaluation are: assess ___, assess ___, and identify ___.
> **A:** Functionality, user experience, specific problems

**Q145.** Five question styles in questionnaires: general, open-ended, ___, multi-choice, and ___.
> **A:** Scalar (Likert), Ranked
