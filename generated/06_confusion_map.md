# Confusion Map: Commonly Confused Concepts in HCI

## How to Use This Document

Each entry identifies two (or more) concepts that students frequently confuse. Study the **difference** column — that's where exam marks are won or lost.

---

## 1. Usability vs. User Experience (UX)

| | Usability | User Experience |
|---|-----------|-----------------|
| **Focus** | Can the user complete the task effectively, efficiently, and with satisfaction? | The entire experience — emotional, aesthetic, social, meaningful |
| **Scope** | Narrower — task completion | Broader — includes pleasure, trust, engagement, aesthetics |
| **Measurement** | ISO 9241: effectiveness, efficiency, satisfaction | Subjective: interviews, experience sampling, diaries |
| **Timing** | During use | Before, during, and after use |
| **Relationship** | UX includes usability | Usability is a component of UX |

**Exam trap**: "Usability and UX are the same thing" — WRONG. Usability is a subset of UX. A system can be usable but have poor UX (boring, ugly, frustrating emotionally).

---

## 2. Learnability vs. Memorability

| | Learnability | Memorability |
|---|-------------|--------------|
| **Focus** | How easy for **new** users to become competent | How easy for **returning** users to remember how to use it |
| **Question** | "Can a first-time user figure this out?" | "After a month away, can the user pick up where they left off?" |
| **Design implication** | Clear affordances, consistent patterns, good onboarding | Consistent placement, meaningful names, recognizable elements |
| **Measurement** | Time to first successful task | Time to re-learn after break |

**Key distinction**: Learnability is about the first use. Memorability is about subsequent uses after a gap.

---

## 3. Slips vs. Mistakes

| | Slips | Mistakes |
|---|-------|----------|
| **What's wrong** | The **action** is wrong | The **goal/intention** is wrong |
| **User's mental model** | Correct | Incorrect |
| **Example** | Reaching for the wrong button (meant to click Save, clicked Delete) | Thinking "Format" means "Save" and clicking Format |
| **Cause** | Inattention, poor skill, bad interface design | Incorrect understanding of how the system works |
| **Fix** | Better **interface design** (affordances, constraints, feedback) | Better **system understanding** (documentation, training, clearer labels) |

**Norman's connection**: Slips = Gulf of Execution (right goal, wrong action). Mistakes = Gulf of Evaluation (wrong goal).

---

## 4. Verification vs. Validation

| | Verification | Validation |
|---|-------------|------------|
| **Question** | "Are we building the product **right**?" | "Are we building the **right** product?" |
| **Focus** | Does it meet the specification? | Does it solve the user's actual problem? |
| **Approach** | Can be automated (testing against spec) | Requires **subjective judgment** (the "formality gap") |
| **Example** | "The button saves the file when clicked" (per spec) | "Users actually need auto-save, not a manual save button" |

**Exam trap**: Assuming verification = validation. Verification can be automated; validation always requires human judgment.

---

## 5. Adaptability vs. Adaptivity

| | Adaptability | Adaptivity |
|---|-------------|------------|
| **Who changes** | The **user** changes the system | The **system** changes itself |
| **Control** | User-initiated | System-initiated |
| **Example** | User customizes toolbar layout, chooses dark mode | System suggests shortcuts based on usage patterns |
| **Nielsen's term** | Under "Customizability" in Flexibility | Under "Customizability" in Flexibility |
| **Principle** | User has control | System is intelligent |

**Both** are sub-types of **Customizability** (a flexibility principle). The difference is who initiates the change.

---

## 6. Direct Manipulation vs. Command Language

| | Direct Manipulation | Command Language |
|---|--------------------|------------------|
| **How it works** | User acts on visible objects | User types text commands |
| **Representation** | Visual "world" | Text-based mediator |
| **Example** | Drag file to trash | Type `rm file.txt` |
| **Learnability** | High (intuitive) | Low (must learn syntax) |
| **Efficiency** | Medium (mouse travel) | High (for experts) |
| **Expressiveness** | Limited to visible objects | Very high |
| **Reversibility** | Easy (undo) | Harder (need undo command) |
| **Error prevention** | High (valid actions only) | Low (syntax errors possible) |

**Shneiderman's 5 properties of DM**: visibility, incremental action, rapid feedback, reversibility, syntactic correctness.

---

## 7. Modal vs. Modeless Interfaces

| | Modal | Modeless |
|---|-------|----------|
| **Behavior** | Interface behaves differently depending on current mode | Same behavior regardless of state |
| **User control** | Limited (computer leads) | Full (user leads) |
| **Example** | Caps Lock changes what typing does; modal dialog blocks other interaction | Most scroll/zoom; menu that closes when you click elsewhere |
| **Problem** | Users get "stuck" in wrong mode | Less structured, may overwhelm novice |
| **Norman's principle** | Violates user control | Supports user control |

**Exam trap**: Forgetting that modal dialogs are pre-emptive — they temporarily take control from the user. Use sparingly.

---

## 8. Parametric vs. Non-Parametric Tests

| | Parametric | Non-Parametric |
|---|-----------|----------------|
| **Assumption** | Data follows **normal distribution** | No distribution assumption |
| **Based on** | Actual data values | Data **ranks** |
| **Power** | More powerful (can detect subtle differences) | Less powerful (may miss real differences) |
| **When to use** | Data is normal, continuous | Data is non-normal, ordinal, or ranked |
| **Example** | Student's t-test, ANOVA | Wilcoxon, Spearman's rank correlation |
| **Fragility** | Fragile if normality assumption violated | Robust (works regardless of distribution) |

**Rule**: Use parametric if you can justify normality. Use non-parametric if you can't. Never assume normality without checking.

---

## 9. Between-Subjects vs. Within-Subjects Design

| | Between-Subjects | Within-Subjects |
|---|-----------------|-----------------|
| **How it works** | Each participant experiences **one** condition | Each participant experiences **all** conditions |
| **Participants needed** | More (one per condition per comparison) | Fewer (same group does everything) |
| **Transfer effects** | None (different groups) | Possible (learning from condition 1 affects condition 2) |
| **Individual variation** | Can bias results (groups may differ) | Controlled (same people) |
| **Counterbalancing** | Not needed | Essential (vary order: A→B vs B→A) |
| **Statistical test** | Independent t-test / between-subjects ANOVA | Paired t-test / within-subjects ANOVA |

**Key trade-off**: Between-subjects is cleaner but needs more users. Within-subjects is efficient but risks transfer effects.

---

## 10. Verification vs. Validation (Software Engineering)

*See entry #4 above — included twice because it appears in both Chapter 6 (software process) and Chapter 9 (evaluation) and is a frequent exam topic.*

---

## 11. Affordance vs. Perception vs. Signifier

| | Affordance | Perception | Signifier |
|---|-----------|------------|-----------|
| **Definition** | What an object **can do** (real property) | What the user **senses** | What **indicates** the affordance |
| **Example (chair)** | Supports sitting | You see the chair | The flat surface and backrest |
| **Example (button)** | Can be pressed | You see a raised rectangle | The 3D appearance, label |
| **In interface** | Perceived affordance (learned) | User's sensory input | Visual cues that suggest use |
| **Key distinction** | Real capability | Sensory experience | Design element that communicates |

**Norman's refinement**: In interfaces, affordances are **perceived** (not innate like physical objects). Signifiers communicate where action should take place.

---

## 12. Internal vs. External Consistency

| | Internal Consistency | External Consistency |
|---|---------------------|---------------------|
| **Scope** | Within **one** application | Across **multiple** applications on a platform |
| **Example** | All dialogs in Word have OK/Cancel at bottom | Ctrl+S saves in Word, Excel, PowerPoint |
| **Violation** | Different shortcut keys within same app | Different paste shortcuts across apps |
| **Importance** | Users learn one app's patterns | Users transfer learning across apps |

**Also**: Input consistency (same input → same output), Output consistency (similar situations → similar responses), Conceptual consistency (matches mental model).

---

## 13. Sensory Memory vs. Short-Term Memory vs. Long-Term Memory

| | Sensory Memory | Short-Term Memory | Long-Term Memory |
|---|---------------|-------------------|-----------------|
| **Capacity** | One sense at a time | **7 ± 2 chunks** | **Unlimited** |
| **Duration** | Ultra-short (ms) | ~200ms decay, ~70ms access | Practically permanent |
| **Access** | Automatic | Rapid (~70ms) | Slow (~100ms) |
| **Forgetting** | Overwritten by new input | Decay and interference | Decay and interference |
| **Design implication** | Don't rely on persistence of sensory icons | Don't exceed 7±2 items; use chunking | Leverage existing LTM (familiar metaphors) |

---

## 14. Deduction vs. Induction vs. Abduction

| | Deduction | Induction | Abduction |
|---|-----------|-----------|-----------|
| **Direction** | General → Specific | Specific → General | Event → Cause |
| **Reliability** | Valid logic (but premises may be false) | **Unreliable** (can't prove true) | **Unreliable** (can lead to false explanations) |
| **Example** | "All dogs bark. Rex is a dog. Therefore Rex barks." | "I've seen 100 white swans. All swans are white." | "The grass is wet. It must have rained." (Could be sprinkler) |
| **Human tendency** | Natural but brings world knowledge | Common but biased | Common but error-prone |
| **Wason's finding** | Humans are poor at using **negative evidence** | | |

---

## 15. Evaluation Only at the End (EXAM TRAP)

**Wrong belief**: "Evaluation happens only after the system is built."

**Correct understanding**: Evaluation should occur **throughout the entire design lifecycle**:
- **Design stage**: Cognitive walkthrough, heuristic evaluation (on specs/prototypes)
- **Implementation stage**: Think aloud, experiments, questionnaires
- **Post-deployment**: Field studies, longitudinal monitoring

**Why it matters**: The later an error is discovered, the more costly it is to fix. Early evaluation (even on paper prototypes) prevents expensive rework.

---

## 16. More Users = Better Experiment (EXAM TRAP)

**Wrong belief**: "More participants always gives better results."

**Correct understanding**:
- For **usability testing** (finding problems): 5 users find ~75% of problems (Nielsen & Landauer). Adding more yields diminishing returns.
- For **controlled experiments** (statistical analysis): Need at least **10 participants** (twice five) for statistical power.
- For **between-subjects**: Adding users without controlling for individual variation can actually **reduce** statistical power.
- For **within-subjects**: Fewer users needed because each person is their own control.

**Key insight**: Quality of participant selection matters more than quantity.

---

## 17. Throwaway vs. Evolutionary vs. Incremental Prototyping

| | Throwaway | Evolutionary | Incremental |
|---|-----------|-------------|-------------|
| **What happens** | Build quickly, discard after learning | Prototype evolves into final product | Build piece by piece, add to final |
| **When to use** | Early exploration, uncertain direction | Direction clear but details unclear | Parts are independent |
| **Cost** | Low (discarded) | Medium (refined over time) | Medium (built up) |
| **Risk** | Wasted if not discarded early | May accumulate technical debt | Integration challenges |

---

## 18. Goals vs. Tasks vs. Domains

| | Domain | Goal | Task |
|---|--------|------|------|
| **Definition** | The area of work | What you want to achieve | How you go about doing it |
| **Level** | Broadest | Intermediate | Most specific |
| **Example** | Graphic design | Create a red triangle | Select fill tool, click over triangle |
| **Exam note** | These terms are used **differently** across HCI literature — especially task vs. goal |

---

## 19. Episodic vs. Semantic Memory

| | Episodic Memory | Semantic Memory |
|---|----------------|-----------------|
| **Content** | Events, experiences (autobiographical) | Facts, concepts, skills |
| **Time** | Bound to specific time/place | Timeless (general knowledge) |
| **Example** | "I ate lunch at café X yesterday" | "Cafés serve coffee" |
| **Relationship** | Source material | Derived from episodic memory |
| **Design implication** | Leverage user's personal experience | Leverage user's general knowledge (mental models) |

---

## 20. Laboratory vs. Field Studies

| | Laboratory | Field |
|---|-----------|-------|
| **Environment** | Controlled, specialist equipment | Real work environment |
| **Context** | Lost (no interruptions, filing cabinets, colleagues) | Preserved |
| **Control** | High (manipulate variables) | Low (noise, distractions) |
| **Observer effect** | Minimal (instrumented room) | Present (Heisenberg principle) |
| **Cost** | High (equipment, setup) | Higher (travel, access, coordination) |
| **Best for** | Controlled comparisons, dangerous tasks | Contextual study, long-duration activities |

**Neither is universally better** — trade off between control (lab) and ecological validity (field).

---

## 21. GOMS vs. KLM

| | GOMS | KLM |
|---|------|-----|
| **Full name** | Goals, Operators, Methods, Selection | Keystroke-Level Model |
| **Level** | Higher-level (task decomposition) | Lower-level (physical actions) |
| **Components** | Goals, Operators, Methods, Selection rules | K, P, Mh, H, D, Rc, Wb, Bb |
| **Use** | Predict performance, compare designs | Calculate precise task times |
| **Scope** | Can model complex tasks with decisions | Best for low-level physical tasks |
| **Relationship** | KLM is a **subset** of GOMS | KLM provides GOMS' operator-level detail |

---

## 22. Earcons vs. Auditory Icons

| | Earcons | Auditory Icons |
|---|---------|---------------|
| **How they work** | Musical sounds representing actions/objects | Real-world sounds (e.g., crumpling paper = delete) |
| **Mapping** | Abstract (must be learned) | Natural (uses existing knowledge) |
| **Example** | Rising musical scale = success | Paper tearing = delete |
| **Learning curve** | Higher (abstract mapping) | Lower (familiar mapping) |
| **Cultural dependence** | High | Moderate |

---

## 23. Internationalisation vs. Localisation

| | Internationalisation | Localisation |
|---|---------------------|-------------|
| **When** | **Before** building (design phase) | **After** building (per market) |
| **What** | Design for multiple cultures from the start | Adapt a product for a specific locale |
| **Example** | Use icons instead of text labels; support RTL layouts | Translate text; change date format; use local currency |
| **Cost** | Lower (built-in from start) | Higher (retrofitting) |

---

## 24. Verification vs. Validation vs. Usability Testing

| | Verification | Validation | Usability Testing |
|---|-------------|------------|-------------------|
| **Question** | Does it meet the spec? | Does it solve the right problem? | Can users actually use it? |
| **Who** | Developers | Stakeholders/users | Real users |
| **Method** | Automated testing | Subjective judgment | Observation, measurement |
| **Timing** | During development | Throughout | Throughout (especially post-prototype) |

---

## 25. Consistency Can Be Dangerous (EXAM TRAP)

**Wrong belief**: "Consistency is always good."

**Correct understanding** (Grudin, 1989): Consistency can be **dangerous** when taken too far.
- The QWERTY keyboard was "consistent" with mechanical typewriters but inefficient
- Sometimes breaking consistency serves users better (e.g., different shortcut for different context)
- Consistency within a system ≠ consistency across all systems

**Lesson**: Understand the **justification** behind guidelines — this helps resolve conflicts when guidelines contradict each other.
