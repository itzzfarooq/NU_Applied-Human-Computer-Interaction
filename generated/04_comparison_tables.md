# HCI Course — Comparison Tables

## 1. STM vs LTM (Short-Term Memory vs Long-Term Memory)

| Feature              | STM                                  | LTM                                       |
|----------------------|--------------------------------------|-------------------------------------------|
| **Capacity**         | Limited (7 ± 2 items)                | Virtually unlimited                       |
| **Access Speed**     | Fast, immediate                      | Slower retrieval                          |
| **Duration**         | Brief (seconds)                      | Hours to lifetime                         |
| **Decay**            | Rapid without rehearsal              | Forgetting curve; can persist indefinitely|
| **Encoding**         | Acoustic / phonological              | Semantic / visual / elaborative           |
| **Types**            | Single store (working memory)        | Episodic, semantic, procedural            |

---

## 2. Slips vs Mistakes

| Feature    | Slip                                    | Mistake                                      |
|------------|-----------------------------------------|----------------------------------------------|
| **Definition** | Execution error — intended plan is wrong but carried out | Planning error — plan itself is wrong        |
| **Cause**     | Inattention, automatic behavior, wrong action selected | Poor mental model, insufficient knowledge    |
| **Fix**       | Better feedback, confirmation dialogs   | Better training, clearer system semantics    |

---

## 3. Deduction vs Induction vs Abduction

| Feature        | Deduction                          | Induction                          | Abduction                                |
|----------------|------------------------------------|------------------------------------|------------------------------------------|
| **Definition** | Reasoning from general to specific| Reasoning from specific to general| Best explanation for an observation      |
| **Reliability**| Certain if premises true           | Probabilistic                      | Plausible but fallible                   |
| **Example**    | All men are mortal → Socrates mortal | observed many swans white → all swans white | smoke → fire is the best explanation |

---

## 4. Office vs Industrial Interfaces

| Feature            | Office Interfaces                  | Industrial Interfaces                 |
|--------------------|------------------------------------|----------------------------------------|
| **Data Type**      | Text, spreadsheets, documents     | Real-time sensor data, control signals |
| **Rate of Change** | Relatively slow                    | Very fast, continuous                  |
| **Environment**    | Quiet, well-lit, controlled       | Noisy, harsh, variable conditions      |
| **User Expertise** | General office workers             | Specialist operators                   |
| **Safety Concern** | Low                                | High (critical systems)                |

---

## 5. Direct vs Indirect Manipulation

| Feature        | Direct Manipulation                    | Indirect Manipulation                  |
|----------------|----------------------------------------|----------------------------------------|
| **Definition** | Continuous visibility of objects, physical actions, rapid reversible effects | Mediated through abstract commands     |
| **Context**    | GUIs, drawing tools, spreadsheets     | Command lines, batch processing        |
| **Issues**     | Limited for complex tasks, scalability| Steep learning curve, lack of visibility|

---

## 6. Command Line vs Menu vs WIMP Interfaces

| Feature         | Command Line                              | Menu-Based                               | WIMP                                     |
|-----------------|-------------------------------------------|------------------------------------------|------------------------------------------|
| **Suitability** | Expert users, scripting                   | Novice users, limited options            | General-purpose, desktop computing       |
| **Advantages**  | Fast, flexible, powerful, scriptable      | Easy to learn, reduces errors            | Visual, intuitive, direct manipulation   |
| **Disadvantages**| Steep learning curve, errors costly       | Slow for experts, limited options        | Requires hardware (mouse), screen space  |

---

## 7. Pull-down vs Drop-down vs Pop-up vs Pie Menus

| Menu Type    | Mechanism                                      | Typical Use Case                       |
|--------------|------------------------------------------------|----------------------------------------|
| **Pull-down**| Opens downward from menu bar item              | Application menu bars (File, Edit)     |
| **Drop-down**| Overlays content, triggered by click/hover     | Form fields, selection lists           |
| **Pop-up**   | Appears at cursor on right-click or trigger    | Context menus, secondary actions       |
| **Pie**      | Radial menu with items around a central point  | Rapid selection (gesture-based, gaming)|

---

## 8. Norman's Model vs Abowd & Beale

| Feature          | Norman's Execution–Evaluation Cycle           | Abowd & Beale (Interactors)              |
|------------------|----------------------------------------------|------------------------------------------|
| **Components**   | User, System, Gulf of Execution, Gulf of Evaluation | User, Interface, System                |
| **Languages**    | Vocabulary of target, vocabulary of articulation | Input, Output, Kernel, Interactor      |
| **Approach**     | Two-gulf model of interaction                | Four-component model with mapping layers|

---

## 9. Computing Paradigms

| Paradigm          | Year       | Key Feature                                |
|-------------------|------------|--------------------------------------------|
| **Batch**         | 1950s–60s  | No direct interaction; jobs queued         |
| **Time-sharing**  | 1960s–70s  | Multiple users share a single computer     |
| **Networking**    | 1970s–80s  | Distributed computing, email               |
| **Graphical**     | 1980s–present| GUIs, desktop metaphor, direct manipulation|

---

## 10. Throwaway vs Incremental vs Evolutionary Prototypes

| Prototype Type    | Definition                                         | Use Case                                |
|-------------------|----------------------------------------------------|-----------------------------------------|
| **Throwaway**     | Built to explore design, then discarded            | Early requirements gathering            |
| **Incremental**   | Developed in stages, each adding functionality     | Large systems built over time           |
| **Evolutionary**  | Continuously refined based on user feedback        | User-centered iterative design          |

---

## 11. IBIS vs QOC (Design Rationale)

| Feature         | IBIS (Issue-Based)                        | QOC (Questions-Options-Criteria)       |
|-----------------|--------------------------------------------|----------------------------------------|
| **Orientation** | Issue-driven, problem-focused              | Decision-driven, solution-focused      |
| **Elements**    | Issues, Positions, Arguments               | Questions, Options, Criteria           |
| **Approach**    | Captures rationale for unresolved issues   | Captures rationale for design decisions|

---

## 12. Principles vs Standards vs Guidelines

| Feature        | Principles                                | Standards                                 | Guidelines                                |
|----------------|-------------------------------------------|-------------------------------------------|-------------------------------------------|
| **Authority**  | Theoretical, universal                    | Formal, mandatory                         | Advisory, recommended                     |
| **Generality** | Very general, high-level                  | Specific, measurable                      | Moderately specific, contextual           |
| **Application**| Inform design philosophy                  | Compliance and accessibility (e.g., WCAG) | Practical day-to-day design decisions     |

---

## 13. Shneiderman's 8 vs Norman's 7

| Feature          | Shneiderman's 8 Golden Rules               | Norman's 7 Principles                   |
|------------------|--------------------------------------------|-----------------------------------------|
| **Focus**        | Interface design and usability             | User-centered design and cognitive fit  |
| **Approach**     | Practical heuristics for interface design  | Principles of good design for action    |
| **Key Points**   | Consistency, feedback, shortcuts, error handling, etc. | Visibility, feedback, constraints, mapping, etc. |

---

## 14. Read-Eval Loop vs Notification-Based Interaction

| Feature          | Read-Eval Loop                              | Notification-Based                      |
|------------------|---------------------------------------------|-----------------------------------------|
| **Mechanism**    | System waits for user input, processes, returns result | System pushes information to user       |
| **Pros**         | Simple, predictable, easy to implement      | Timely, reduces user effort             |
| **Cons**         | No proactive behavior, can miss events      | Can overwhelm, interrupt user flow      |

---

## 15. Seeheim vs MVC vs PAC

| Feature       | Seeheim                                      | MVC (Model-View-Controller)           | PAC (Presentation-Abstraction-Control) |
|---------------|----------------------------------------------|---------------------------------------|-----------------------------------------|
| **Components**| Presentation, Control, Application Model     | Model, View, Controller               | Presentation, Abstraction, Control     |
| **Layers**    | Three layers                                 | Three layers (loosely coupled)        | Three layers (hierarchical agents)     |
| **Relationship**| Presentation ↔ Control ↔ Model             | View observes Model; Controller mediates | Each agent is MVC triple; agents nest |

---

## 16. Cognitive Walkthrough vs Heuristic Evaluation

| Feature           | Cognitive Walkthrough                        | Heuristic Evaluation                    |
|-------------------|----------------------------------------------|-----------------------------------------|
| **Who Performs**  | Designers, evaluators (small team)           | Usability experts (3–5)                 |
| **Method**        | Step-by-step task walkthrough                | Compare against established heuristics |
| **Focus**         | Learnability for new users                   | General usability problems              |

---

## 17. Think Aloud vs Cooperative Evaluation

| Feature          | Think Aloud Protocol                         | Cooperative Evaluation                  |
|------------------|----------------------------------------------|-----------------------------------------|
| **Process**      | User verbalizes thoughts during task         | Evaluator and user discuss problems     |
| **Advantages**   | Rich insight into user reasoning             | More interactive, deeper exploration    |
| **Disadvantages**| May slow user, artificial                    | Evaluator bias, more resource-intensive |

---

## 18. Interviews vs Questionnaires

| Feature        | Interviews                                  | Questionnaires                          |
|----------------|---------------------------------------------|-----------------------------------------|
| **Flexibility**| High (follow-up, probing)                   | Low (fixed questions)                   |
| **Reach**      | Limited (one at a time)                     | Large populations                       |
| **Analysis**   | Qualitative, time-consuming                 | Quantitative, scalable                  |

---

## 19. Within Groups vs Between Groups (Study Design)

| Feature            | Within Groups                               | Between Groups                          |
|--------------------|---------------------------------------------|-----------------------------------------|
| **Design**         | Same participants in all conditions         | Different participants per condition    |
| **Cost**           | Fewer participants needed                   | More participants needed                |
| **Learning Transfer**| Risk of carryover/order effects           | No carryover effects                    |
| **Sensitivity**    | Higher (controls individual differences)    | Lower (more variance)                   |

---

## 20. Parametric vs Non-Parametric Tests

| Feature          | Parametric Tests                            | Non-Parametric Tests                    |
|------------------|---------------------------------------------|-----------------------------------------|
| **Assumptions**  | Normal distribution, equal variance         | Few or no distributional assumptions    |
| **Power**        | Higher when assumptions met                 | Lower, but more robust to violations    |
| **Reliability**  | Sensitive to outliers and skewness          | More robust,适用于ordinal/small data    |

---

## 21. Eye Tracking Measurements

| Measurement     | Description                                         |
|-----------------|-----------------------------------------------------|
| **Fixations**   | Stable gaze on a region; indicates processing/attention |
| **Saccades**    | Rapid eye movements between fixations               |
| **Scan Paths**  | Sequential pattern of fixations and saccades        |
| **Pupil Size**  | Changes indicate cognitive load or arousal           |
| **Blink Rate**  | Associated with fatigue or mental effort             |

---

## 22. Physiological Measurements

| Measurement     | Abbreviation | What It Measures                               |
|-----------------|--------------|------------------------------------------------|
| **Galvanic Skin Response** | GSR   | Skin conductance — emotional arousal/stress    |
| **Electromyography**      | EMG   | Muscle activity — tension, micro-expressions   |
| **Electroencephalography**| EEG   | Brain electrical activity — cognitive load     |
| **Heart Rate / HRV**      | HR    | Heart rate variability — stress, attention     |

---

## 23. Laboratory vs Field Studies

| Feature        | Laboratory Studies                            | Field Studies                            |
|----------------|-----------------------------------------------|------------------------------------------|
| **Context**    | Controlled, artificial                        | Natural, real-world                      |
| **Equipment**  | Specialized lab equipment                     | Portable or in-situ tools                |
| **Validity**   | High internal validity, low ecological        | High ecological validity, low control    |

---

## 24. Design Rationale Types

| Type              | Focus                                      | Structure                               |
|-------------------|--------------------------------------------|-----------------------------------------|
| **IBIS**          | Issues, positions, arguments               | Graph-based, issue-driven               |
| **QOC**           | Questions, options, criteria               | Decision-focused, criteria-based        |
| **Psychological** | User mental models, cognitive fit          | Theory-driven, user-centered            |

---

*Generated for NU Applied HCI Course — Exam Preparation*
