# Chapter 9: Evaluation Techniques — How to Tell If Your Design Works

## The Big Picture

You've designed and built an interface (Chapters 5-8) following principles (Chapter 7). Now: **does it actually work?** Evaluation is the process of answering that question.

Evaluation happens **throughout** the design lifecycle — not just at the end. There are two broad approaches:
1. **Expert evaluation** — specialists inspect the design
2. **User evaluation** — real people use the system

Each has strengths and weaknesses. Choosing the right method depends on where you are in the process, what you need to learn, and what resources you have.

---

## 1. WHAT IS EVALUATION?

### Goals

1. **Assess functionality** — does the system do what users need?
2. **Assess effect on user** — is it usable, learnable, satisfying?
3. **Identify specific problems** — what's broken or confusing?

### Where Evaluation Happens

- **Laboratory** — controlled, specialist equipment
- **Field** — real context, natural behavior
- **In collaboration with users** — participatory

---

## 2. EXPERT EVALUATION — No Users Needed

Three methods where evaluators (not users) inspect the design:

### Cognitive Walkthrough

**Who**: Expert in cognitive psychology
**How**: Walks through each task step, analyzing what cognitive processes are required and what learning problems may occur.
**Focus**: Does the design support users in **learning** the task?

For each step, the expert asks:
- What impact will this interaction have on the user?
- What cognitive processes are required?
- What learning problems might occur?

### Heuristic Evaluation

**Who**: Usability experts
**How**: Evaluators check the interface against a set of **usability heuristics** (rules of thumb). Each violation is a potential problem.
**Example heuristics**: system behaviour is predictable, consistent, provides feedback.

Think of it as **debugging the design**.

### Review-Based Evaluation

**How**: Use results from the published HCI literature to support or refute design decisions.
**Caution**: Ensure results from prior studies actually transfer to your design context.
**Related**: **Model-based evaluation** (e.g., GOMS) — use cognitive models to predict performance and filter design options.

---

## 3. USER EVALUATION — Getting Real Feedback

### Laboratory Studies

| Pros | Cons |
|------|------|
| Specialist equipment available | Lack of context |
| Uninterrupted environment | Hard to observe multiple users cooperating |

**Best for**: Dangerous or impractical field settings, constrained single-user systems, controlled manipulation of use.

### Field Studies

| Pros | Cons |
|------|------|
| Natural environment | Distractions |
| Context retained | Noise |
| Longitudinal studies possible | Observation may alter behavior |

**Best for**: When context is crucial, longitudinal studies.

---

## 4. EVALUATING IMPLEMENTATIONS

Requires an **artefact** to test: simulation, prototype, or full implementation. Earlier in design → lighter evaluation. Later → more rigorous.

---

## 5. EXPERIMENTAL EVALUATION — The Scientific Approach

### The Process

1. Choose a **hypothesis**
2. Define **experimental conditions** (differ in exactly one variable)
3. Measure **behavioral changes**
4. Attribute changes to the different conditions

### Key Experimental Concepts

| Concept | Definition | Example |
|---------|-----------|---------|
| **Subjects** | Who participates — representative, sufficient sample | 20 users representative of your target audience |
| **Independent Variable (IV)** | What you change between conditions | Interface style (menu vs. command) |
| **Dependent Variable (DV)** | What you measure | Time to complete task, error rate |
| **Hypothesis** | Your prediction | "Error rate increases as font size decreases" |
| **Null hypothesis** | No difference between conditions (aim to disprove) | "Font size has no effect on error rate" |

### Experimental Designs

| Design | How It Works | Pros | Cons |
|--------|-------------|------|------|
| **Within Groups** | Each subject experiences all conditions | Less costly, less user variation | Transfer of learning possible |
| **Between Groups** | Each subject experiences one condition | No transfer of learning | More users needed, variation can bias |

---

## 6. ANALYSIS OF DATA

### Before Statistics

- **Look at your data** — visualize it
- **Save original data** — never work on the only copy

### Choosing a Statistical Test

Depends on:
1. **Type of data**: Discrete (finite values) vs. Continuous (any value)
2. **Information required**: Is there a difference? How big? How accurate?

### Types of Tests

| Test Type | Assumption | Pros | Cons |
|-----------|-----------|------|------|
| **Parametric** | Normal distribution | Robust, powerful | Assumption may not hold |
| **Non-parametric** | No distribution assumption | More reliable | Less powerful |
| **Contingency table** | Classify by discrete attributes | Simple count data | Limited to categorical |

---

## 7. GROUP STUDIES — Evaluating Collaboration

More difficult than single-user experiments.

### Challenges

- **Subject groups**: larger numbers, more expensive, harder to timetable, more variation
- **Tasks**: must encourage cooperation — creative tasks, decision games, control tasks
- **Data gathering**: multiple video cameras + logging; sync is hard, volume is huge
- **Analysis**: vast variation between groups

### Solutions

- Within-groups experiments
- **Micro-analysis** (e.g., gaps in speech)
- Anecdotal and qualitative analysis
- Look at interactions between group and medium

---

## 8. FIELD STUDIES — Real-World Context

- Experiments are dominated by group formation
- Field studies are more realistic
- **Distributed cognition** — study work in context
- Real action is **situated action** — physical and social environment both crucial

**Contrast**: Psychology → controlled experiments. Sociology/anthropology → open studies with rich data.

---

## 9. OBSERVATIONAL METHODS — Watching Users Work

### Five Methods

| Method | How It Works | Best For |
|--------|-------------|----------|
| **Think Aloud** | User describes thoughts while performing task | Simple, insightful |
| **Cooperative Evaluation** | User + evaluator collaborate, both ask questions | Less constrained, user criticizes system |
| **Protocol Analysis** | Record via paper/audio/video/logging/notebooks | Mixed approach in practice |
| **EVA (Automated)** | Post-task walkthrough, user reacts after event | Focused analysis, less interruption |
| **Post-task Walkthrough** | Transcript played back to user for comment | Immediate (fresh) or delayed (prepared questions) |

### Think Aloud — The Classic

**Pros**: Simple, requires little expertise, useful insight, shows actual use.
**Cons**: Subjective, selective, describing may alter task performance.

### Protocol Analysis — Recording Methods

| Method | Pros | Cons |
|--------|------|------|
| Paper & pencil | Cheap | Limited to writing speed |
| Audio | Good for think aloud | Hard to sync with other data |
| Video | Accurate, realistic | Special equipment, obtrusive |
| Computer logging | Automatic, unobtrusive | Large data volume |
| User notebooks | Good for longitudinal | Coarse, subjective |

In practice, methods are **mixed**.

---

## 10. QUERY TECHNIQUES — Asking Users Directly

### Interviews

| Pros | Cons |
|------|------|
| Can be varied to context | Very subjective |
| Issues explored fully | Time consuming |
| Elicits unanticipated problems | |

### Questionnaires

| Pros | Cons |
|------|------|
| Quick, reaches large groups | Less flexible |
| Can be analyzed rigorously | Less probing |

**Styles of questions**:
- **General** — broad, open
- **Open-ended** — free-form responses
- **Scalar** — Likert scale ratings
- **Multi-choice** — select from options
- **Ranked** — order by preference

**Key**: Design the questionnaire carefully. Know what information you need and how you'll analyze it beforehand.

---

## 11. PHYSIOLOGICAL METHODS — Measuring the Body

### Eye Tracking

Measures:
- **Fixations** — eye pauses (number/duration = difficulty level)
- **Saccades** — rapid eye movements between fixations
- **Scan paths** — overall movement pattern (straight to target + short fixation = optimal)

### Physiological Measurements

| Measure | What It Tracks |
|---------|---------------|
| **Heart activity** | Blood pressure, volume, pulse |
| **Galvanic Skin Response (GSR)** | Sweat gland activity |
| **Electromyogram (EMG)** | Muscle electrical activity |
| **Electroencephalogram (EEG)** | Brain electrical activity |

**Limitation**: Interpreting these responses is difficult — more research needed.

---

## 12. CHOOSING AN EVALUATION METHOD — Seven Dimensions

| Dimension | Options |
|-----------|---------|
| **When in process** | Design vs. Implementation |
| **Style** | Laboratory vs. Field |
| **Objectivity** | Subjective vs. Objective |
| **Measures** | Qualitative vs. Quantitative |
| **Information level** | High level vs. Low level |
| **Interference** | Obtrusive vs. Unobtrusive |
| **Resources** | Time, subjects, equipment, expertise |

**There is no single "best" method.** The right choice depends on where you are, what you need to learn, and what you can afford.

---

## KEY CONCEPTS FOR EXAM

1. **Evaluation goals**: assess functionality, effect on user, identify problems
2. **Cognitive walkthrough**: expert analyzes learning support per task step
3. **Heuristic evaluation**: experts check for heuristic violations (Nielsen & Molich)
4. **Review-based evaluation**: literature supports/refutes design; GOMS prediction
5. **Lab studies**: controlled, specialist equipment, lacks context
6. **Field studies**: natural environment, context retained, longitudinal possible
7. **Experimental evaluation**: hypothesis, IV/DV, controlled conditions
8. **IV** (changed between conditions) vs **DV** (measured)
9. **Null hypothesis**: no difference — aim to disprove
10. **Within groups**: each subject does all conditions (transfer possible, less costly)
11. **Between groups**: each subject does one condition (no transfer, more users)
12. **Parametric**: normal distribution assumed (powerful but fragile)
13. **Non-parametric**: no distribution assumption (reliable but less powerful)
14. **Group studies**: harder than single-user — subjects, tasks, data, analysis problems
15. **Distributed cognition**: work studied in context
16. **Situated action**: real action, physical + social environment crucial
17. **Think aloud**: user describes thoughts — simple but subjective
18. **Cooperative evaluation**: user + evaluator collaborate
19. **Protocol analysis**: paper/audio/video/logging/notebooks
20. **EVA**: post-task walkthrough, less interruption
21. **Post-task walkthroughs**: transcript playback — immediate or delayed
22. **Interviews**: one-to-one, flexible, subjective, time-consuming
23. **Questionnaires**: quick, large groups, rigorous — 5 question styles
24. **Eye tracking**: fixations (difficulty), saccades (movement), scan paths
25. **Physiological**: GSR, EMG, EEG, heart — hard to interpret
26. **Choosing method**: 7 dimensions — match to your stage, needs, and resources
