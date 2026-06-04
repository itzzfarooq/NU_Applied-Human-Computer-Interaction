# Reference Sheet: Applied HCI (Chapters 1–9)

Quick-lookup document for exam revision. Organized by topic.

---

## Key Definitions (One-Liners)

| Term | Definition |
|------|-----------|
| **HCI** | Study of interaction between people (users) and computers |
| **Usability** | Effectiveness, efficiency, and satisfaction with which users achieve goals (ISO 9241) |
| **User Experience (UX)** | The entire experience including emotional, aesthetic, and meaningful aspects |
| **Affordance** | Property of an object that suggests how it can be used |
| **Signifier** | Design element that communicates where action should take place |
| **Ergonomics** | Study of physical characteristics of interaction (human factors) |
| **Interaction Style** | The way users communicate with computers (CLI, menus, WIMP, etc.) |
| **Mental Model** | User's internal explanation of how a system works |
| **Cognitive Load** | Mental effort required for interaction |
| **Chunking** | Grouping items to fit more in working memory |
| **Heuristic** | Rule of thumb, guideline, or principle for design |
| **GOMS** | Goals, Operators, Methods, Selection — model predicting user performance |
| **KLM** | Keystroke-Level Model — quantitative prediction of low-level task time |
| **Personas** | Fictional users representing real user categories |
| **Scenarios** | Stories about users and systems illustrating interaction |
| **Wizard of Oz** | Human simulates computer response behind the scenes |
| **Formality Gap** | Validation always relies on subjective proof — can't fully automate "is this good?" |
| **Discount Usability** | Cheap, flexible evaluation methods (heuristic eval, cognitive walkthrough) |
| **Paradigm Shift** | Fundamental worldview change in computing (batch → interactive → ubiquitous) |
| **Direct Manipulation** | Interacting with visual representation of work rather than typing commands |

---

## Models and Frameworks

### Norman's 7 Stages of Interaction (Ch. 3)

```
1. Establish Goal
2. Form Intention
3. Specify Actions
4. Execute Action
         ↓
5. Perceive System State
6. Interpret State
7. Evaluate State vs. Goal
```

**Two Gulfs**: Execution (user actions ≠ system allows) | Evaluation (user expects ≠ system shows)

### Abowd & Beale Framework (Ch. 3)

```
User (U) ↔ Input (I) ↔ System (S) ↔ Output (O)
```

Each component has its own language. Interaction = translation between languages.

### Human Information Processing (Ch. 1)

```
Input (senses) → Memory (storage) → Processing (thinking) → Output (movement/action)
                      ↑                              ↓
                  Emotion (affects everything)    Errors (inevitable)
```

### Memory Systems (Ch. 1)

| System | Capacity | Duration | Access |
|--------|----------|----------|--------|
| Sensory | One sense | Ultra-short (ms) | Automatic |
| STM | 7±2 chunks | ~200ms decay | ~70ms |
| LTM | Unlimited | Permanent | ~100ms |

### LTM Structure Models (Ch. 1)

| Model | Key Idea |
|-------|----------|
| **Semantic Network** | Nodes with inheritance (child inherits parent properties) |
| **Frames** | Slots with fixed/default/variable values |
| **Scripts** | Stereotypical situations (entry conditions, props, roles, scenes) |
| **Production Rules** | IF condition THEN action |

### GOMS Model (Ch. 9)

| Component | Definition |
|-----------|-----------|
| **Goals** | What the user wants to achieve |
| **Operators** | Primitive physical/mental actions |
| **Methods** | Sequences of operators that accomplish a goal |
| **Selection Rules** | Choose between alternative methods |

### KLM Operators (Ch. 9)

| Operator | Symbol | Time |
|----------|--------|------|
| Keystroke | K | 0.2s |
| Pointing | P | 1.1s |
| Mental preparation | Mh | 1.35s |
| Home (hand to device) | H | 0.4s |
| Draw | D | Varies |
| System response | Rc | Varies |
| Write (handwriting) | Wb | 1.5s/char |
| Browse button | Bb | 0.2s |

**Total time = Σ(operator times)**

### Fitts' Law (Ch. 1)

> **Mt = a + b × log₂(D/S + 1)**

Where D = distance to target, S = target size.
**Design rule**: Make targets large and distances small.

### Seeheim Model (Ch. 8)

```
Presentation (lexical) ↔ Dialogue Control (syntactic) ↔ Functionality (semantic)
```

+ **Switch**: Direct path between Presentation and Functionality for rapid semantic feedback.

### Arch/Slinky Model (Ch. 8)

```
Physical → Lexical → Dialogue → Functional Core Adaptor → Functional Core
```

### MVC (Ch. 8)

| Component | Role |
|-----------|------|
| **Model** | Internal state / data / logic |
| **View** | Screen rendering (output) |
| **Controller** | Input processing |

**Problem**: Controller talks to View in practice (clean separation violated).

### PAC (Ch. 8)

| Component | Role |
|-----------|------|
| **Abstraction** | Logical state (like Model) |
| **Presentation** | Manages both input AND output (unified) |
| **Control** | Mediates (hierarchical) |

---

## Principles

### Nielsen's 10 Usability Heuristics (Ch. 7)

| # | Heuristic | Key Idea |
|---|-----------|----------|
| 1 | Visibility of system status | Keep users informed through feedback |
| 2 | Match system and real world | Use user's language, follow conventions |
| 3 | User control and freedom | Undo/redo, emergency exits |
| 4 | Consistency and standards | Follow platform conventions |
| 5 | Error prevention | Better than good error messages |
| 6 | Recognition rather than recall | Minimize memory load |
| 7 | Flexibility and efficiency | Accelerators for experts |
| 8 | Aesthetic and minimalist design | No irrelevant information |
| 9 | Help users recover from errors | Clear, constructive error messages |
| 10 | Help and documentation | Searchable, task-focused, concrete |

### Shneiderman's 8 Golden Rules (Ch. 7)

| # | Rule | Key Idea |
|---|------|----------|
| 1 | Strive for consistency | Similar actions → similar results |
| 2 | Enable shortcuts | Accelerators for frequent users |
| 3 | Offer informative feedback | Every action has a response |
| 4 | Design dialogs for closure | Tell users when done |
| 5 | Error prevention and handling | Prevent, then forgive |
| 6 | Permit easy reversal | Undo is essential |
| 7 | Support internal locus of control | Users feel in charge |
| 8 | Reduce short-term memory load | Don't make users remember (7±2) |

### Norman's 7 Principles (Ch. 7)

| # | Principle | Key Idea |
|---|-----------|----------|
| 1 | Knowledge in world and head | Don't rely on memory alone |
| 2 | Simplify task structure | Reduce complexity |
| 3 | Make things visible | Bridge execution and evaluation gulfs |
| 4 | Get mappings right | Natural control-effect relationships |
| 5 | Exploit constraints | Natural and artificial |
| 6 | Design for error | Assume errors will happen |
| 7 | Standardize | When all else fails, make it consistent |

### Three High-Level Usability Principles (Ch. 7)

| Principle | Sub-Principles |
|-----------|---------------|
| **Learnability** | Predictability, Synthesizability, Familiarity, Generalizability, Consistency |
| **Flexibility** | Dialogue Initiative, Multithreading, Task Migratability, Substitutivity, Customizability |
| **Robustness** | Observability, Recoverability, Responsiveness, Task Conformance |

---

## Evaluation Methods (Compact Comparison)

### Expert Methods (No Users Required)

| Method | What It Checks | When to Use | Key Requirement |
|--------|---------------|-------------|-----------------|
| **Cognitive Walkthrough** | Learning through exploration (4 questions per task step) | Design stage | Task description + action list |
| **Heuristic Evaluation** | Violations of 10 usability heuristics | Any stage | 3–5 independent evaluators |
| **Model-Based (GOMS/KLM)** | Predicted task performance | Design stage | Task decomposition |
| **Review-Based** | Literature supports/refutes design | Design stage | Relevant studies |

### User-Based Methods

| Method | What It Does | When to Use | Key Trade-off |
|--------|-------------|-------------|---------------|
| **Think Aloud** | User describes thoughts during task | Implementation | Simple but affects performance |
| **Cooperative Evaluation** | User + evaluator collaborate | Implementation | Less constrained, more probing |
| **Experiment** | Controlled comparison with IV/DV | Implementation | Most powerful, most expensive |
| **Interviews** | Flexible, deep probing | Any stage | Subjective, time-consuming |
| **Questionnaires** | Quick, large groups | Any stage | Fixed questions, low return rate |
| **Eye Tracking** | Fixations, saccades, scan paths | Implementation | Expensive equipment |
| **Physiological** | GSR, EMG, EEG, heart | Implementation | Unclear mapping to events |

### Evaluation Method Selection (8 Dimensions)

1. **Stage in cycle**: Design (analytic) vs. Implementation (user-based)
2. **Style**: Lab (controlled) vs. Field (natural)
3. **Objectivity**: Subjective (expert judgment) vs. Objective (repeatable)
4. **Measures**: Quantitative (numeric) vs. Qualitative (descriptive)
5. **Information level**: Low-level (specific) vs. High-level (overall)
6. **Immediacy**: During interaction vs. Post-hoc
7. **Intrusiveness**: Obtrusive (alters behavior) vs. Unobtrusive
8. **Resources**: Time, money, equipment, participants

### Key Numbers to Remember

| Finding | Source |
|---------|--------|
| 5 evaluators find ~75% of usability problems | Nielsen & Landauer |
| 1 user finds ~33% of problems | Nielsen & Landauer |
| 7±2 chunks in STM | Miller's Law |

| 10+ participants for controlled experiments | Nielsen |
| 1–5 or 1–7 Likert scales most effective | Questionnaire design |
| 25–30% typical questionnaire return rate | Survey research |
| 0.2s keystroke, 1.1s pointing, 1.35s mental | KLM standard times |

---

## Design Process Stages

### UCD (User-Centered Design) Process

```
1. Understand context of use
2. Specify user requirements
3. Design solutions
4. Evaluate against requirements
         ↑_______________↓
              (iterate)
```

### Software Lifecycle (Ch. 6)

```
Requirements → Architecture → Detailed Design → Coding → Integration → Maintenance
```

**Problem for HCI**: Interactive systems need feedback loops — waterfall is too linear.

### Prototyping Strategies (Ch. 6)

| Strategy | What Happens |
|----------|-------------|
| **Throwaway** | Build quickly, discard after learning |
| **Incremental** | Build piece by piece, add to final |
| **Evolutionary** | Prototype evolves into final product |

### Design Rationale Approaches (Ch. 6)

| Approach | Structure | Focus |
|----------|----------|-------|
| **IBIS** | Issue → Position → Argument | Process (the journey) |
| **QOC** | Question → Option → Criteria | Structure (the map) |
| **DRL** | Formal QOC with richer semantics | Structure (more formal) |

---

---

## Screen Design Principles (Ch. 2, Ch. 5)

### Gestalt Principles

| Principle | Rule |
|-----------|------|
| **Proximity** | Group related items close together |
| **Similarity** | Use consistent styles for same-type items |
| **Closure** | Mind completes incomplete shapes |
| **Continuity** | Align elements along smooth paths |

### Text Display Rules

| Rule | Guideline |
|------|-----------|
| Font | Sans-serif for screens, serif for print |
| Size | Minimum 12pt |
| Line length | 50–75 characters |
| Line spacing | 1.2–1.5× font size |
| Contrast | High contrast essential |

### Information Density

- Use **progressive disclosure** — show detail on demand
- Tabs, expandable sections, layered navigation

---

## Colour (Ch. 2)

| Model | Type | Use |
|-------|------|-----|
| **RGB** | Additive (light) | Displays |
| **HSB/HSV** | Intuitive | Design tools |
| **CMYK** | Subtractive (ink) | Printing |

**Critical facts**:
- 8% males, 1% females are colour blind
- Never rely on colour alone — use redundant cues
- Red = warning/error, Green = ok/success, Blue = information/links
- Blue acuity is lowest — don't use blue for critical detail

---

## Paradigm Shifts (Ch. 4)

| Era | Paradigm | Key Innovation |
|-----|----------|---------------|
| 1940s–50s | Batch Processing | Submit job, wait for results |
| 1960s | Time-Sharing | Multiple users, interactive computing |
| 1960s–70s | Networking | Email, file sharing, collaboration |
| 1962 | Graphical Displays | Sutherland's Sketchpad |
| 1970s | Microprocessor | Personal computing (Kay's Dynabook) |
| 1990s | WWW | Hypertext on global network |
| 1991+ | Ubiquitous Computing | Technology that disappears (Weiser) |

### Key Figures

| Person | Contribution |
|--------|-------------|
| **Sutherland** | Sketchpad (1962) — first graphical interaction |
| **Licklider** | Time-sharing, interactive computing |
| **Papert** | LOGO — programming for children |
| **Kay** | Dynabook vision — personal computing |
| **Shneiderman** | Direct manipulation (1982), 8 golden rules |
| **Norman** | 7 stages, 7 principles, gulfs |
| **Nielsen** | 10 heuristics, heuristic evaluation, discount usability |
| **Weiser** | Ubiquitous computing (1991) |
| **Berners-Lee** | World Wide Web |
| **Csikszentmihalyi** | Flow theory |

---

## Formulas and Calculations

### Fitts' Law

> **Mt = a + b × log₂(D/S + 1)**

- Mt = movement time
- D = distance to target
- S = target size (width along movement axis)
- a, b = constants (depend on device/user)
- **Design implication**: Larger targets and shorter distances = faster movement

### KLM Total Execution Time

> **T = Σ(operator times) + mental operators**

| Operator | Time |
|----------|------|
| K (keystroke) | 0.2s |
| P (pointing) | 1.1s |
| Mh (mental prep) | 1.35s |
| H (home to device) | 0.4s |
| D (draw) | varies |
| Rc (system response) | varies |
| Wb (write) | 1.5s/char |
| Bb (browse button) | 0.2s |

### Nielsen's Severity Rating

| Rating | Meaning |
|--------|---------|
| 0 | Not a usability problem |
| 1 | Cosmetic — fix if extra time |
| 2 | Minor — low priority |
| 3 | Major — high priority |
| 4 | Catastrophe — must fix before release |

### Reaction Times

| Stimulus | Reaction Time |
|----------|--------------|
| Visual | ~200ms |
| Auditory | ~150ms |
| Pain | ~700ms |

### Memory Characteristics

| System | Access Time | Decay | Capacity |
|--------|------------|-------|----------|
| Sensory | Instant | Ultra-short | 1 sense |
| STM | ~70ms | ~200ms | 7±2 chunks |
| LTM | ~100ms | Permanent | Unlimited |

---

## Key Comparisons

### Office vs. Industrial Interfaces (Ch. 3)

| Dimension | Office | Industrial |
|-----------|--------|------------|
| Data type | Textual | Numeric |
| Rate of change | Slow | Fast |
| Environment | Clean | Dirty |
| Manipulation | Direct | Indirect |

### Glass Interfaces (Ch. 3)

| Pros | Cons |
|------|------|
| Cheaper, more flexible | Not physically located |
| Multiple representations | Loss of context |
| Precise values | Complex interfaces |

### Prototyping Techniques (Ch. 6)

| Technique | Description |
|-----------|------------|
| **Storyboards** | Visual interaction flow (not computer-based) |
| **Limited functionality** | Some parts simulated by designers |
| **Wizard of Oz** | Human simulates computer behind the scenes |

### Question Types (Ch. 9)

| Style | Example |
|-------|---------|
| General | Demographic questions |
| Open-ended | "Any suggestions for improvement?" |
| Scalar (Likert) | "Rate ease of use: 1–5" |
| Multi-choice | "How do you get help?" (tick one) |
| Ranked | "Rank these methods by usefulness" |

---

## Design Rules Spectrum (Ch. 7)

```
High Generality, Low Authority
        ↓
    Principles (abstract, flexible)
        ↓
    Guidelines (moderate)
        ↓
    Standards (specific, rigid)
        ↓
Low Generality, High Authority
```

**Trade-off**: More general = more situations but harder to enforce. More specific = more enforceable but fewer situations.

---

## Common Exam Numbers

| Fact | Number |
|------|--------|
| STM capacity | 7 ± 2 chunks |
| Colour blind males | 8% |
| Colour blind females | 1% |
| Human hearing range | 20Hz – 15kHz |
| Visual reaction time | ~200ms |
| Auditory reaction time | ~150ms |
| Pain reaction time | ~700ms |
| KLM keystroke time | 0.2s |
| KLM pointing time | 1.1s |
| KLM mental prep time | 1.35s |
| KLM home to device | 0.4s |
| Nielsen: 5 evaluators find | ~75% problems |
| Nielsen: 1 user finds | ~33% problems |
| Min participants for experiments | 10+ |
| Likert scale optimal range | 1–5 or 1–7 |
| Questionnaire return rate | 25–30% |
| Optimal line length | 50–75 characters |
| Min font size for screens | 12pt |
