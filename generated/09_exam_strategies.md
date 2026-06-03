# HCI Final Exam Preparation Strategy Guide
## Chapters 1-9 | Applied Human-Computer Interaction

---

## 1. EXAM FORMAT OVERVIEW

### What to Expect
HCI exams typically test conceptual understanding over rote memorization. Expect questions that require you to apply principles to scenarios, compare frameworks, and evaluate designs.

### Typical Question Types

| Question Type | What It Tests | Strategy |
|---------------|---------------|----------|
| **Definition** | Recall of key terms | State definition + example |
| **Comparison** | Understanding differences between similar concepts | Use tables, highlight distinctions |
| **Application** | Applying theory to scenarios | Reference specific principles/models |
| **Evaluation** | Critiquing designs using HCI principles | Use heuristics as checklist |
| **Essay** | Deep understanding + synthesis | Structure: Define → Explain → Example → Relate |
| **Short Answer** | Quick recall + precision | Be concise, hit key points |

### Exam Strategy
- **Read all questions first** before answering any
- **Allocate time proportionally** (e.g., 10 questions × 6 min each for 60-min exam)
- **Answer high-confidence questions first** to secure marks
- **Always relate back to HCI theory** — don't just describe, analyze

---

## 2. HIGH-PRIORITY TOPICS

These topics are most likely to appear based on frequency of emphasis in lecture notes and cross-chapter references.

### Tier 1: Critical (Almost Certain to Appear)

#### Norman's Model and Gulfs (Ch. 3)
- **7 stages**: Goal → Intention → Specify actions → Execute → Perceive → Interpret → Evaluate
- **Gulf of Execution**: User's formulation ≠ system's allowed actions
- **Gulf of Evaluation**: User's expectation ≠ actual system state
- **Exam tip**: Draw the model, label execution/evaluation loops, give examples of each gulf
- **Connection**: Links to affordances (Ch. 5), design principles (Ch. 7), errors (Ch. 1)

#### Fitts' Law (Ch. 1)
- **Formula**: Mt = a + b log₂(D/S + 1)
  - Mt = movement time, a/b = constants, D = distance, S = size
- **Design implications**: Make targets large, keep distances short
- **Exam tip**: Can be applied to pointing devices, menu design, button placement
- **Common mistake**: Forgetting the +1 in the formula

#### STM vs LTM (Ch. 1)
| Property | STM | LTM |
|----------|-----|-----|
| Capacity | 7 ± 2 chunks | Unlimited |
| Decay | Rapid (~200ms) | Very slow, if any |
| Access | Rapid (~70ms) | Slow (~100ms) |
| Types | Working memory | Episodic + Semantic |
| Storage | Temporary | Permanent |

- **Chunking**: Groups information to exceed STM limits
- **Exam tip**: Give examples of chunking, explain why it matters for interface design

#### Gestalt Principles (Ch. 5)
- **Proximity**: Items close together → perceived as group
- **Similarity**: Items that look alike → perceived as group
- **Closure**: Mind completes incomplete shapes
- **Continuity**: Eye follows smooth paths
- **Exam tip**: Apply to screen design — how would you group related items?

#### Affordances (Ch. 5)
- Properties of an object that suggest how it can be used
- Button "affords" pressing, slider "affords" sliding
- **Physical affordances** (real world) vs **perceived affordances** (interface)
- **Exam tip**: Relate to Norman's principle "Make things visible"

#### Nielsen's 10 Heuristics (Ch. 9)
1. Visibility of system status
2. Match between system and real world
3. User control and freedom
4. Consistency and standards
5. Error prevention
6. Recognition over recall
7. Flexibility and efficiency of use
8. Aesthetic and minimalist design
9. Help users recognize, diagnose, and recover from errors
10. Help and documentation

#### Shneiderman's 8 Golden Rules (Ch. 7)
1. Strive for consistency
2. Enable frequent users to use shortcuts
3. Offer informative feedback
4. Design dialogs to yield closure
5. Offer error prevention and simple error handling
6. Permit easy reversal of actions
7. Support internal locus of control
8. Reduce short-term memory load

#### Norman's 7 Principles (Ch. 7)
1. Use both knowledge in the world and knowledge in the head
2. Simplify the structure of tasks
3. Make things visible: bridge the gulfs
4. Get the mappings right
5. Exploit the power of constraints
6. Design for error
7. When all else fails, standardize

#### Experimental Design (Ch. 9)
- **IV (Independent Variable)**: What you change
- **DV (Dependent Variable)**: What you measure
- **Within groups**: Same subjects, all conditions (transfer risk, fewer users)
- **Between groups**: Different subjects per condition (no transfer, more users)
- **Null hypothesis**: No difference — aim is to disprove

#### MVC vs PAC vs Seeheim (Ch. 8)

| Model | Components | Key Feature |
|-------|------------|-------------|
| **MVC** | Model (data), View (rendering), Controller (input) | Controller talks to View |
| **PAC** | Abstraction, Presentation, Control | Clean separation, manages hierarchy |
| **Seeheim** | Presentation, Dialogue Control, Functionality | Conceptual contribution; switch connects layers |

- **MVC**: Used in practice (Java Swing)
- **PAC**: Cleaner conceptually but less used
- **Seeheim**: Arose from implementation but principal contribution is conceptual

### Tier 2: Important (Likely to Appear)

#### Verification vs Validation (Ch. 6)
- **Verification**: Designing the product right (Does implementation match specification?)
- **Validation**: Designing the right product (Does system meet user needs?)

#### ISO 9241 Usability (Ch. 6)
- **Effectiveness**: Can you achieve what you want?
- **Efficiency**: Can you do it without wasting effort?
- **Satisfaction**: Do you enjoy the process?

#### Prototyping Types (Ch. 5-6)
- **Throwaway**: Built quickly, discarded
- **Incremental**: Built piece by piece
- **Evolutionary**: Evolves into final system
- **Wizard of Oz**: Human simulates computer response

#### Design Rationale (Ch. 6)
- **IBIS** (Issue-Based Information System): Issues → Positions → Arguments (process-oriented)
- **QOC** (Question-Option-Criterion): Questions → Options → Criteria (structure-oriented)
- **DRL** (Design Rationale Language): More formal than QOC

#### Interaction Styles Comparison (Ch. 3)
- Command line: Expert users, repetitive tasks
- Menus: Recognition-based, less recall
- Natural language: Vague, ambiguous
- WIMP: Default for most systems

### Tier 3: Supporting (May Appear)

- **Ergonomics/Human factors** (Ch. 3)
- **Direct manipulation** (Ch. 4)
- **Ubiquitous computing** (Ch. 4)
- **Eye tracking** (Ch. 9)
- **Questionnaire/interview methods** (Ch. 9)

---

## 3. COMMON EXAM TRAPS

### Slips vs Mistakes (Ch. 1, 3)
| | Slip | Mistake |
|---|------|---------|
| **Goal** | Correct | Incorrect |
| **Action** | Wrong | May be correct |
| **Cause** | Inattention, poor skill | Wrong understanding |
| **Fix** | Better interface design | Better system understanding |
| **Example** | Clicking wrong button | Searching in wrong menu |

**Trap**: Students often confuse which is which. Remember: **Slips = right intention, wrong action. Mistakes = wrong intention.**

### Deduction vs Induction vs Abduction (Ch. 1)
| Type | Direction | Reliability | Example |
|------|-----------|-------------|---------|
| **Deduction** | General → Specific | Logically valid (not necessarily true) | If raining → ground wet. Raining → ground wet |
| **Induction** | Specific → General | Unreliable (can only prove false) | All elephants seen have trunks → all elephants have trunks |
| **Abduction** | Event → Cause | Unreliable (can lead to false explanations) | Sam drives fast → assume drunk |

**Trap**: Deduction can be **logically valid but factually wrong** (e.g., "If it is raining then the ground is dry. It is raining. Therefore the ground is dry.")

### Within Groups vs Between Groups (Ch. 9)
| | Within Groups | Between Groups |
|---|---------------|----------------|
| **Subjects** | Each performs all conditions | Each performs one condition |
| **Learning transfer** | Possible (risk) | None |
| **Users needed** | Fewer | More |
| **Cost** | Lower | Higher |

**Trap**: Students forget that within groups has **transfer of learning** as a confounding variable.

### Parametric vs Non-Parametric Tests (Ch. 9)
| | Parametric | Non-Parametric |
|---|------------|----------------|
| **Distribution** | Assumes normal | No assumption |
| **Power** | More powerful | Less powerful |
| **Reliability** | Less reliable (if assumption violated) | More reliable |
| **Use when** | Normal distribution confirmed | Non-normal or unknown distribution |

**Trap**: Parametric tests are more powerful but only valid if distribution is normal. Using parametric on non-normal data gives misleading results.

### Seeheim vs MVC vs PAC (Ch. 8)
- **Seeheim**: Conceptual model (Presentation → Dialogue → Functionality). Principal contribution is conceptual, not implementation.
- **MVC**: Implementation model (Model → View → Controller). Controller needs to talk to View (separation not complete in practice).
- **PAC**: Clean separation but less used in practice.

**Trap**: Students confuse Seeheim with PAC. Seeheim has **3 layers + switch**, PAC has **3 components + control mediates**. Seeheim is more abstract; PAC is more concrete.

### Cognitive Walkthrough vs Heuristic Evaluation (Ch. 9)
| | Cognitive Walkthrough | Heuristic Evaluation |
|---|----------------------|----------------------|
| **Focus** | Learning support | Heuristic violations |
| **Performed by** | Cognitive psychology expert | Usability experts |
| **Method** | Walks through design step-by-step | Checks against heuristics list |
| **Output** | Learning problems | Heuristic violations |

**Trap**: Cognitive walkthrough is about **how users learn**, heuristic evaluation is about **checking against principles**.

### Verification vs Validation (Ch. 6)
- **Verification**: "Are we building the product right?" (Does implementation match spec?)
- **Validation**: "Are we building the right product?" (Does it meet user needs?)

**Trap**: Students swap these. Remember: **V**erification = **V**ersion (implementation), **V**alidation = **V**alue (to user).

### Affordance vs Signifier (Ch. 5)
- **Affordance**: What an object CAN do (button can be pressed)
- **Signifier**: What an object SUGGESTS it can do (button looks pressable)

**Trap**: Norman distinguishes these in later work. Affordance is objective; signifier is perceived.

---

## 4. KEY FORMULAS TO MEMORIZE

### Fitts' Law (Ch. 1)
```
Mt = a + b × log₂(D/S + 1)
```
- **Mt**: Movement time
- **a, b**: Empirically determined constants (experimentally derived)
- **D**: Distance to target
- **S**: Size of target

**Quick check**: If D = 10cm, S = 2cm → Mt = a + b × log₂(10/2 + 1) = a + b × log₂(6) = a + b × 2.58

**Design rule**: Maximize S, minimize D → minimize Mt

### STM Capacity (Ch. 1)
```
STM capacity = 7 ± 2 chunks
```
- Range: 5-9 chunks
- Access time: ~70ms
- Decay time: ~200ms

**Design implication**: Don't present more than 7 items at once in menus/lists

### Reaction Times (Ch. 1)
| Stimulus Type | Reaction Time |
|---------------|---------------|
| Visual | ~200ms |
| Auditory | ~150ms |
| Pain | ~700ms |

**Design implication**: Auditory feedback is faster; use for critical alerts

### Human Hearing Range (Ch. 1)
```
20Hz - 15,000Hz (15kHz)
```
- Less accurate at high frequencies
- Cocktail party phenomenon: can focus on one voice in noise

### Colour Blindness (Ch. 1, 2)
```
8% males, 1% females
```
**Design rule**: Don't rely on colour alone — use shapes, patterns, text labels

---

## 5. ESSAY WRITING TIPS

### Structure for HCI Essay Answers

#### 1. Introduction (1-2 sentences)
- State the concept/framework being discussed
- Briefly define it

#### 2. Explanation (2-3 sentences)
- Describe the concept in detail
- Reference the theorist/model

#### 3. Example (1-2 sentences)
- Give a concrete example
- Relate to interface design

#### 4. Relationship (1-2 sentences)
- Connect to other HCI concepts
- Show understanding of broader context

#### 5. Evaluation (1-2 sentences)
- Strengths/weaknesses
- When it applies/doesn't apply

### Example: "Explain the Gulf of Execution and give an example"

> The **Gulf of Execution** (Norman, 1988) is the gap between what a user intends to do and what actions the system allows. It occurs when the user's formulation of actions does not match the system's available operations. For example, a user wanting to delete a file may look for a trash can icon, but the system only offers a keyboard shortcut — the user cannot formulate the correct action because the system does not provide the expected mechanism. This connects to Norman's principle of **making things visible** and highlights the importance of **affordances** in interface design.

### Key Essay Tips
- **Always reference theorists** by name (Norman, Shneiderman, Nielsen)
- **Use HCI terminology** correctly (gulf, affordance, heuristic)
- **Give examples** — abstract answers score poorly
- **Compare/contrast** when asked about relationships
- **Structure clearly** — markers scan for organization

### Phrases That Score Marks
- "This relates to Norman's principle of..."
- "In contrast to [concept X], [concept Y]..."
- "The practical implication is..."
- "This can be seen in the example of..."
- "This connects to [related concept] because..."

---

## 6. QUICK REFERENCE CARD

### Last-Minute Facts (Print This Section)

#### Models & Frameworks
| Concept | Key Points |
|---------|------------|
| **Norman's Model** | 7 stages, execution/evaluation loop, gulfs |
| **Abowd & Beale** | User, Input, System, Output — each has own language |
| **MVC** | Model (data), View (output), Controller (input) |
| **PAC** | Abstraction, Presentation, Control — cleaner separation |
| **Seeheim** | Presentation → Dialogue → Functionality (+ switch) |

#### Heuristics & Principles
| Framework | Count | Key Examples |
|-----------|-------|--------------|
| **Nielsen's Heuristics** | 10 | Visibility, match real world, error prevention |
| **Shneiderman's Golden Rules** | 8 | Consistency, shortcuts, feedback, closure |
| **Norman's Principles** | 7 | Knowledge in world/head, visible, constraints |

#### Human Factors
| Property | Value |
|----------|-------|
| STM capacity | 7 ± 2 chunks |
| STM access | ~70ms |
| STM decay | ~200ms |
| LTM access | ~100ms |
| LTM capacity | Unlimited |
| Visual reaction | ~200ms |
| Auditory reaction | ~150ms |
| Hearing range | 20Hz-15kHz |
| Colour blindness | 8% males, 1% females |

#### Fitts' Law
```
Mt = a + b log₂(D/S + 1)
Make targets LARGE, distances SHORT
```

#### Verification vs Validation
```
Verification = Building the product RIGHT (implementation vs spec)
Validation = Building the RIGHT product (system vs user needs)
```

#### Evaluation Methods
| Method | Type | When |
|--------|------|------|
| Cognitive Walkthrough | Expert | Design phase |
| Heuristic Evaluation | Expert | Design phase |
| Think Aloud | User | Implementation |
| Cooperative Evaluation | User | Implementation |
| Lab Study | User | Implementation |
| Field Study | User | Implementation |

#### Interaction Styles
| Style | Best For | Weakness |
|-------|----------|----------|
| Command line | Experts, repetition | Learning curve |
| Menus | Novices, recognition | Screen space |
| WIMP | General use | Default for most |
| Natural language | Familiarity | Ambiguity |

---

## 7. CHAPTER-BY-CHAPTER MUST-KNOW

### Chapter 1: The Human
1. **Fitts' Law**: Formula + design implications (targets large, distances short)
2. **STM vs LTM**: Capacity, access speed, decay, types (episodic/semantic)
3. **Chunking**: How it overcomes STM limits
4. **Slips vs Mistakes**: Right intention vs wrong intention
5. **Deduction/Induction/Abduction**: Direction and reliability differences

### Chapter 2: The Computer
1. **Colour models**: RGB (additive, displays), CMYK (subtractive, printing), HSB (intuitive)
2. **Colour blindness**: 8% males, 1% females — never rely on colour alone
3. **Fitts' Law application**: Apply to pointing devices, menus, buttons
4. **Screen design**: Grouping (Gestalt), alignment, white space, consistency
5. **Text display**: Sans-serif for screens, 50-75 char line length, high contrast

### Chapter 3: The Interaction
1. **Norman's model**: 7 stages, execution/evaluation loop
2. **Gulfs of Execution and Evaluation**: Definition + examples
3. **Interaction styles**: Command line, menus, WIMP — when to use each
4. **WIMP elements**: Windows, Icons, Menus, Pointers
5. **Physical design**: Constraints (ergonomic, physical, legal, economic)

### Chapter 4: Paradigms
1. **Paradigm shifts**: Batch → Time-sharing → Graphical → Personal → WWW → Ubiquitous
2. **Direct manipulation** (Shneiderman 1982): Visibility, feedback, reversibility
3. **WYSIWYG**: What You See Is What You Get
4. **Ubiquitous computing** (Weiser 1991): Technologies that disappear
5. **Metaphor**: Benefits (relating to real world) and problems (cultural bias)

### Chapter 5: Interaction Design Basics
1. **Gestalt principles**: Proximity, similarity, closure, continuity
2. **Affordances**: Properties that suggest how to use
3. **Prototyping**: Throwaway, incremental, evolutionary
4. **Wizard of Oz**: Human simulates computer response
5. **Navigation design**: Four golden rules (landmarks, routes, overviews, context)

### Chapter 6: HCI in the Software Process
1. **Waterfall model**: Sequential but needs feedback loops for interactive systems
2. **Verification vs Validation**: Building right vs building right product
3. **ISO 9241**: Effectiveness, efficiency, satisfaction
4. **Design rationale**: IBIS (issues, positions, arguments) vs QOC (questions, options, criteria)
5. **Prototyping types**: Throwaway, incremental, evolutionary

### Chapter 7: Design Rules
1. **Shneiderman's 8 Golden Rules**: Consistency, shortcuts, feedback, closure, error prevention, reversal, locus of control, reduce memory load
2. **Norman's 7 Principles**: Knowledge in world/head, simplify, visible, mappings, constraints, design for error, standardize
3. **Principles of usability**: Learnability, flexibility, robustness
4. **Design patterns**: Invariant solution to recurrent problem
5. **Standards vs guidelines**: Standards = high authority; Guidelines = high generality

### Chapter 8: Implementation Support
1. **MVC**: Model (data), View (output), Controller (input) — used in Java Swing
2. **PAC**: Abstraction, Presentation, Control — cleaner separation
3. **Seeheim**: Presentation → Dialogue → Functionality (+ switch) — conceptual contribution
4. **Windowing systems**: Device independence + resource sharing
5. **Client-server architecture**: Clients (apps) ↔ Server (resource manager) ↔ Devices

### Chapter 9: Evaluation Techniques
1. **Cognitive walkthrough**: Expert evaluates learning support
2. **Heuristic evaluation**: Experts check for heuristic violations
3. **Experimental design**: IV (what you change), DV (what you measure)
4. **Within vs Between groups**: Transfer vs no transfer, fewer vs more users
5. **Eye tracking**: Fixations (difficulty), saccades (movement), scan paths (optimal)

---

## 8. STUDY PLAN RECOMMENDATIONS

### Day Before Exam (6-8 hours)
| Time | Activity |
|------|----------|
| **Hour 1-2** | Review Tier 1 high-priority topics |
| **Hour 3-4** | Practice applying concepts to scenarios |
| **Hour 5-6** | Review common exam traps |
| **Hour 7** | Quick reference card review |
| **Hour 8** | Active recall — test yourself without notes |

### Night Before
- **Do**: Review quick reference card, sleep well
- **Don't**: Learn new material, stay up late

### Morning of Exam
- **Do**: Glance at quick reference card, eat breakfast
- **Don't**: Panic, cram, skip meals

---

## 9. ACTIVE RECALL PRACTICE QUESTIONS

### Quick Self-Test
1. What is the formula for Fitts' Law?
2. What are the two gulfs in Norman's model?
3. What is the capacity of STM?
4. Name 3 Gestalt principles
5. What is the difference between verification and validation?
6. What are the three components of MVC?
7. Name 3 of Shneiderman's 8 Golden Rules
8. What is the difference between within and between groups designs?
9. What are Nielsen's top 3 heuristics?
10. What is an affordance?

*(Answers: 1. Mt = a + b log₂(D/S + 1), 2. Execution + Evaluation, 3. 7±2, 4. Proximity/Similarity/Closure, 5. Right product vs product right, 6. Model/View/Controller, 7. Consistency/Feedback/Error prevention, 8. Same subjects vs different subjects, 9. Visibility/Match real world/User control, 10. Properties suggesting how to use)*

---

## 10. FINAL CHECKLIST

Before entering the exam, confirm you can:
- [ ] State Fitts' Law formula and its design implications
- [ ] Explain Norman's 7 stages and both gulfs
- [ ] Compare STM and LTM on 4 dimensions
- [ ] List and explain 3 Gestalt principles
- [ ] Define affordance and give an example
- [ ] Explain the difference between slips and mistakes
- [ ] Compare deduction, induction, and abduction
- [ ] State Shneiderman's 8 Golden Rules
- [ ] State Norman's 7 Principles
- [ ] Explain verification vs validation
- [ ] Define ISO 9241 usability (effectiveness, efficiency, satisfaction)
- [ ] Compare MVC, PAC, and Seeheim models
- [ ] Explain within vs between groups experimental designs
- [ ] Compare cognitive walkthrough vs heuristic evaluation
- [ ] Name 3 prototyping types and explain Wizard of Oz
- [ ] Explain IBIS vs QOC design rationale

---

*Good luck on your exam! Remember: understand concepts, don't just memorize. Apply theory to examples. Use HCI terminology correctly.*
