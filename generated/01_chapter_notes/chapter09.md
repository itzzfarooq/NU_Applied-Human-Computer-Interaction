# Chapter 9: Evaluation Techniques

## The Big Picture

You've designed an interface (Chapters 5–8) following principles (Chapter 7). Now: **does it actually work?** Evaluation answers that question — not as a final phase, but **continuously** throughout the lifecycle. Fixing problems early is far cheaper than fixing them late.

Two broad approaches:
1. **Expert analysis** — specialists inspect the design (cheap, works on specs/prototypes, but no actual use observed)
2. **User participation** — real people use the system (requires working prototype, but assesses real use)

Neither replaces the other.

---

## 1. What Is Evaluation?

Evaluation has three main goals:

| Goal | What It Means |
|------|---------------|
| **Assess functionality** | Does the system do what users need? Is functionality clearly reachable? Does it match user expectations of the task? |
| **Assess user experience** | Is it learnable? Usable? Satisfying? Does it overload the user? |
| **Identify specific problems** | What causes confusion, unexpected results, or errors? These trouble-spots can then be rectified. |

Evaluation can happen in a **laboratory** (controlled, specialist equipment), in the **field** (real context, natural behavior), or **collaboratively with users** (participatory).

---

## 2. Expert Evaluation — Inspecting Without Users

Cheap, flexible, works at **any stage** (specs to full systems). Does **not assess actual use**.

### 2.1 Cognitive Walkthrough

Adapted from software engineering code walkthroughs. Focus: **learning through exploration**.

**What you need**: (1) specification/prototype, (2) representative task, (3) complete action list, (4) user profile

**Four questions** — for each action in the task sequence:

| # | Question | What It Checks |
|---|----------|---------------|
| 1 | Is the effect of the action the same as the user's goal? | Goal-action match |
| 2 | Will users see that the action is available? | Visibility (not recognition) |
| 3 | Will users know it's the correct action? | Meaning is clear |
| 4 | Will users understand the feedback? | Completion confirmation |

Any negative answer → **usability problem report** (system version, date, evaluator, description, severity).

### 2.2 Heuristic Evaluation

By **Nielsen & Molich**. A heuristic = guideline or rule of thumb. **3–5 independent evaluators** critique the system against heuristics. Five evaluators find ~**75%** of problems.

**Nielsen's Severity Rating Scale (0–4)**:
- **0** = Not a usability problem
- **1** = Cosmetic — fix only if extra time available
- **2** = Minor — low priority
- **3** = Major — high priority, important to fix
- **4** = Catastrophe — must fix before release

**Nielsen's Ten Usability Heuristics**:

| # | Heuristic | Key Idea |
|---|-----------|----------|
| 1 | **Visibility of system status** | Keep users informed through feedback within reasonable time |
| 2 | **Match between system and real world** | Use user's language, follow real-world conventions, natural/logical order |
| 3 | **User control and freedom** | Provide "emergency exit," support undo/redo |
| 4 | **Consistency and standards** | Don't make users wonder if different words/situations mean the same thing |
| 5 | **Error prevention** | Prevent problems before they occur (better than good error messages) |
| 6 | **Recognition rather than recall** | Make objects/actions/options visible; minimize memory load |
| 7 | **Flexibility and efficiency of use** | Accelerators for experts; cater to inexperienced and experienced users |
| 8 | **Aesthetic and minimalist design** | No irrelevant information; every extra unit competes with relevant units |
| 9 | **Help users recognize, diagnose, and recover from errors** | Plain language, precise problem indication, constructive suggestions |
| 10 | **Help and documentation** | Searchable, task-focused, concrete steps, not too large |

**Key characteristic**: Discount usability technique — cheap, flexible, any stage. Evaluations must be **independent**. Domain-specific heuristics can supplement (e.g., "awareness of other users" for groupware).

### 2.3 Model-Based Evaluation

- **GOMS** (Goals, Operators, Methods, Selection) — predicts user performance; filters design options (Section 8 below)
- **KLM** — lower-level, predicts task execution time (Section 8 below)
- **Dialog models** — state transition networks evaluate dialog sequences for unreachable states, circular dialogs, complexity
- **Design rationale** (Ch. 6) — evaluate options against criteria with supporting evidence

### 2.4 Using Previous Studies

Literature reviews can support/refute design decisions without repeating experiments. **Caution**: must verify transferability — experimental design, participant population, and assumptions may not apply to your context.

---

## 3. User-Based Evaluation

Expert techniques are **not a replacement** for usability testing with actual users. User-based methods include experimental, observational, query, and physiological techniques.

### 3.1 Laboratory vs. Field Studies

| Dimension | Laboratory | Field |
|-----------|-----------|-------|
| **Environment** | Controlled, specialist equipment | Real work environment |
| **Pros** | Interruption-free; sophisticated recording; variable manipulation | Natural context; observe cooperation; longitudinal |
| **Cons** | Lack of context; hard to observe cooperation | Noise; observer effect (Heisenberg principle) |
| **Best for** | Dangerous/remote; constrained tasks; controlled comparisons | Context crucial; actual use; long-duration activities |

### 3.2 Experimental Evaluation

Most powerful method for **empirical evidence**.

**Participants**: Must match expected user population. **Nielsen & Landauer**: 1 user → ~33% problems; 5 users → ~75%. For statistical experiments, at least **10 participants**.

**Variables**: **IV** (manipulated) vs **DV** (measured). Each IV value = a **level**.

**Hypotheses**: Prediction in terms of IV/DV. Aim: **disprove the null hypothesis** (no difference).

**Experimental Designs**:

| Design | How It Works | Pros | Cons |
|--------|-------------|------|------|
| **Between-subjects** | Each participant → one condition | No learning transfer; cleaner | More participants; individual variation |
| **Within-subjects** | Each participant → all conditions | Fewer users; less variation | Transfer possible (mitigate via counterbalancing) |
| **Mixed** | One variable between, one within | Compromise | Complex analysis |

**Key concepts**: **Control condition** (identical except manipulation); **Counterbalancing** (vary order to reduce transfer); **Transfer effect** (practice from condition 1 affects condition 2).

### 3.3 Statistical Analysis

**Two rules**: (1) **Look** at your data (visualize — spot outliers), (2) **Save** your data (never discard originals).

**Data types**: Discrete (finite values), continuous (any value in range), positive continuous (no negatives — e.g., response time).

**Statistical test selection**:

| Test Type | Assumption | When to Use | Trade-off |
|-----------|-----------|-------------|-----------|
| **Parametric** | Normal distribution | Robust, powerful | Fragile if assumption violated |
| **Non-parametric** | No distribution assumption (rank-based) | Non-normal or ordinal data | Less powerful |
| **Contingency table** | Discrete attributes, count combinations | Categorical data (chi-squared) | Limited to categorical |

**When is data normal?** If it's the sum/average of many small independent effects, likely normal. Subjective ratings are typically **not** normal.

**Common tests** (Table 9.1):
- Two-valued IV + Normal DV → **Student's t test**
- Discrete IV + Normal DV → **ANOVA**
- Continuous IV + Normal DV → **Regression**
- Non-parametric equivalents: **Wilcoxon rank-sum**, **Spearman's correlation**

**Three questions about data**:
1. **Is there a difference?** (hypothesis testing)
2. **How big?** (point estimation)
3. **How accurate?** (confidence intervals)

**Within-subjects analysis**: Subtract each participant's overall mean from condition scores to remove inter-participant differences, then analyze residuals.

### 3.4 Evaluating Group Systems

Harder than single-user: more participants (3 people × 10 experiments = 30 participants), longer sessions, scheduling, enormous data, extreme group variation.

**Solutions**: within-group experiments; **micro-analysis** of gaps between utterances; **anecdotal/qualitative analysis** (critical incidents); **ethnography** (detailed contextual recording, observer outside the situation).

---

## 4. Observational Techniques — Watching Users Work

Users are observed completing tasks. Simple observation rarely suffices — users are asked to **think aloud**.

### 4.1 Think Aloud

User **talks through what they're doing** while being observed.

| Pros | Cons |
|------|------|
| Simple; little expertise needed | Subjective and selective |
| Useful insight into problems | Describing changes performance ("centipede effect") |
| Works throughout design process | |

### 4.2 Cooperative Evaluation (Nielsen)

User sees themselves as **collaborator**. Evaluator can ask **"why?"** and **"what-if?"**; user can ask for clarification. Less constrained than standard think aloud; user is **encouraged to criticize the system**.

### 4.3 Protocol Analysis — Recording Methods

| Method | Pros | Cons |
|--------|------|------|
| **Paper/pencil** | Cheap; captures extraneous events | Limited by writing speed |
| **Audio** | Good for think aloud | Hard to identify exact actions |
| **Video** | See what participant does | Camera positioning; obtrusive |
| **Computer logging** | Automatic, unobtrusive; excellent for **longitudinal** | Huge data volume; "semantics free" (no why) |
| **User notebooks** | Good for longitudinal; captures unusual tasks | Coarse; interpreted records |

Methods are **mixed** in practice. Transcription loses nuances; coding schemes help but are hard to apply consistently.

### 4.4 Automatic Protocol Analysis Tools

**EVA** (Experimental Video Annotator): multimedia workstation linked to video recorder. Evaluator tags events during recording (timestamps, snapshots, errors). Tagged segments reviewed after session. **Drawback**: tagging can distract from observing.

Other: **Workplace project** (Xerox PARC) for synchronized multi-stream analysis; **DRUM** (MUSiC toolkit) for usability metrics.

### 4.5 Post-Task Walkthroughs

Replays transcript to participant for comment. **Immediate**: participant remembers why. **Delayed**: analyst frames focused questions but loses freshness. **Essential** when participant cannot talk during task (critical/intensive tasks).

---

## 5. Query Techniques — Asking Users Directly

Gets the **user's viewpoint directly**. Relatively simple and cheap, but information is **subjective** and may be a "rationalized" account.

### 5.1 Interviews

| Pros | Cons |
|------|------|
| Flexible; probe deeply | Subjective; time-consuming |
| Elicits unanticipated problems | |
| High-level evaluation (preferences, attitudes) | |

**Approach**: Top-down — general questions → leading ("why?", "what if?"). Plan in advance but adapt. Best **with observation** to clarify events.

### 5.2 Questionnaires

| Pros | Cons |
|------|------|
| Quick; large groups; rigorous | Fixed questions; less probing |
| Multiple design stages | Low return rate (~25–30%) |

**Five question styles**:

| Style | Description | Example |
|-------|-------------|---------|
| **General** | User background | Demographics |
| **Open-ended** | Unprompted opinion | "Any improvements?" |
| **Scalar (Likert)** | Numeric scale rating | "Easy to recover from mistakes" — Disagree 1 2 3 4 5 Agree |
| **Multi-choice** | Select from responses | "How do you get help?" |
| **Ranked** | Order by preference | "Rank these methods" (1 = most useful) |

**Scalar scales**: 1–5 or 1–7 most effective. Odd scales = neutral option; even scales force choice. Prefer **closed questions** to reduce burden. Always **pilot study** (4–5 users) before distribution.

**Specific validated questionnaires**: **QUIS** (User Interface Satisfaction), **SUS** (System Usability Scale), **NASA-TLX** (Task Load Index — cognitive workload).

---

## 6. Physiological Measures — Measuring the Body

Objective usability testing — measuring what users do and how they feel directly.

### 6.1 Eye Tracking

Eye movements reflect **cognitive processing**. Modern systems are non-invasive.

| Measurement | What It Indicates |
|-------------|-------------------|
| **Number of fixations** | More = less efficient search |
| **Fixation duration** | Longer = difficulty |
| **Saccades** | Rapid movements between fixations |
| **Scan path** | Overall pattern — cognitive load; optimal = straight to target |

**Status**: Promising but expensive; more research needed for interpretation.

### 6.2 Other Physiological Measurements

| Measure | Tracks | Associated With |
|---------|--------|-----------------|
| **Heart activity** | Blood pressure, pulse | Stress |
| **GSR** | Sweat gland activity | Arousal, mental effort |
| **EMG** | Muscle electrical activity | Task involvement |
| **EEG** | Brain electrical activity | Decision making, attention |

**Key limitation**: Unclear relationship between physiological changes and specific interaction events. Increased pulse could mean frustration OR task stress. Mapping physiological patterns to emotional states remains an **active research question**.

---

## 7. Choosing an Evaluation Method — Eight Dimensions

No single "best" method. Eight factors distinguish techniques:

| Factor | Options |
|--------|---------|
| **1. Stage in cycle** | Design (cheap, analytic) vs. Implementation (comprehensive, user-based) |
| **2. Style** | Laboratory (controlled) vs. Field (natural context) |
| **3. Objectivity** | Subjective (evaluator expertise) vs. Objective (repeatable) |
| **4. Measures** | Quantitative (statistical) vs. Qualitative (detailed but harder to analyze) |
| **5. Information level** | Low-level (specific decisions) vs. High-level (overall impression) |
| **6. Immediacy** | Immediate (during interaction) vs. Post-hoc (after event; recall bias) |
| **7. Intrusiveness** | Obtrusive (alters behavior) vs. Unobtrusive (limited info) |
| **8. Resources** | Time, money, equipment, participants, expertise |

**Classification tables** (textbook Tables 9.4–9.7):

**Analytic** (Table 9.4): CW, HE, Review, Model — all throughout design; HE = high-level, CW = low-level

**Experimental/Query** (Table 9.5): Experiment = objective/quantitative; Interviews/Qnaire = subjective, high-level

**Observational** (Table 9.6): Think Aloud, Protocol, Post-Task — all implementation stage, qualitative

**Monitoring** (Table 9.7): Eye Tracking, Physiological — objective, quantitative, high equipment cost

---

## 8. GOMS and Performance Models

**GOMS** (Goals, Operators, Methods, Selection) — model-based evaluation predicting user performance.

| Component | Definition | Example |
|-----------|-----------|---------|
| **Goals** | What user wants to achieve | "Send an email" |
| **Operators** | Primitive physical/mental actions | Keystrokes, mouse clicks, pointing |
| **Methods** | Sequences of operators for a goal | Open compose → type address → click send |
| **Selection rules** | Choose between alternative methods | If attachment → use "attach then send" |

### Keystroke-Level Model (KLM)

Lower-level GOMS variant predicting task execution time:

| Operator | Symbol | Typical Time |
|----------|--------|-------------|
| **Keystroke** | K | ~0.2–0.3s |
| **Pointing** | P | ~1.1s |
| **Mental hesitation** | Mh | ~1.35s |
| **Home (hand to device)** | H | ~0.4s |
| **Draw** | D | Varies |
| **System response** | Rc | Varies |
| **Write (handwriting)** | Wb | ~1.5s/char |
| **Browse button** | Bb | ~0.2s |

**Total time** = Σ(operator times) + mental operators. Allows **pre-implementation** comparison of interface designs. **Limitation**: best for low-level physical tasks; doesn't capture learning or error recovery well.

---

## Relationships to Other Topics

| Related Topic | Connection |
|---------------|------------|
| **Chapter 3 (Interaction models)** | Cognitive walkthrough's fourth question addresses the execution–evaluation cycle |
| **Chapter 6 (Design processes)** | Evaluation feeds back into design; design rationale supports model-based evaluation |
| **Chapter 7 (Usability principles)** | Heuristics are related to principles and guidelines; evaluation criteria drawn from Chapter 7 principles |
| **Chapter 12 (GOMS in detail)** | GOMS/KLM discussed more thoroughly; prediction of user performance |
| **Chapter 13 (Requirements)** | Observation and surveying users contribute to requirements capture |
| **Chapter 16 (Dialog models)** | State transition networks evaluate dialog designs prior to implementation |
| **Wizard of Oz (Ch. 6)** | Simulation technique for evaluating systems without full implementation |

---

## Common Misconceptions

1. **"Evaluation is just testing at the end"** — WRONG. Evaluation should occur **throughout** the design lifecycle, with results feeding back continuously.
2. **"Expert evaluation replaces user testing"** — WRONG. Expert methods don't assess actual use; they check adherence to principles. Both are needed.
3. **"Five users are always enough"** — Nielsen's finding applies to observational studies finding usability issues. Controlled experiments with statistical analysis need larger samples (at least 10).
4. **"More users = better experiment"** — Not necessarily. With between-subjects design, adding more users without controlling for variation can actually reduce statistical power.
5. **"Parametric tests are always better"** — They're more powerful but require normal distribution. If the assumption is violated, results are invalid. Non-parametric tests are safer when assumptions are uncertain.
6. **"Think aloud doesn't affect performance"** — It does. Describing what you're doing often changes how you do it (the centipede effect).
7. **"Field studies are always more valid"** — They have ecological validity but are expensive, hard to control, and the observer effect still applies (Heisenberg uncertainty principle).
8. **"Heuristic evaluation finds all problems"** — Five evaluators find ~75%. You need multiple independent evaluators.
9. **"Subjective measures are useless"** — They provide high-level information (preferences, impressions) that objective measures miss. Ideally, both are used.
10. **"Statistical significance = practical significance"** — A statistically significant result may have a trivially small effect size. Always consider both.

---

## Key Concepts for Exam

1. **Evaluation goals**: assess functionality, user experience, and specific problems
2. **Evaluation throughout design lifecycle** — cheapest to fix early, most expensive late
3. **Cognitive walkthrough**: expert analyzes learning support per task step using **four questions** (goal match, visibility, recognition, feedback)
4. **Heuristic evaluation** (Nielsen & Molich): **3–5 independent evaluators** check for violations of **10 heuristics**; severity rated **0–4**; **five evaluators find ~75%** of problems
5. **Nielsen's 10 heuristics**: visibility of status, match real world, user control/freedom, consistency/standards, error prevention, recognition over recall, flexibility/efficiency, aesthetic/minimalist, help recover from errors, help/documentation
6. **Review-based evaluation**: literature supports/refutes design; must verify transferability
7. **GOMS model**: Goals, Operators, Methods, Selection — predicts user performance
8. **KLM operators**: K (keystroke), P (pointing), Mh (mental), H (home to device), D (draw), Rc (system response), Wb (write), Bb (browse button)
9. **Laboratory studies**: controlled, specialist equipment, lacks context
10. **Field studies**: natural environment, context retained, observer effect applies
11. **Experimental evaluation**: hypothesis → IV/DV → controlled conditions → statistical analysis
12. **IV** (manipulated between conditions) vs **DV** (measured outcome)
13. **Null hypothesis**: no difference — aim to **disprove** it
14. **Between-subjects**: each subject does one condition (no transfer, more users needed)
15. **Within-subjects**: each subject does all conditions (transfer possible via counterbalancing, fewer users needed)
16. **Mixed design**: one variable between-groups, one within-groups
17. **Parametric tests**: assume normal distribution (powerful but fragile)
18. **Non-parametric tests**: no distribution assumption (rank-based; reliable but less powerful)
19. **ANOVA**: used when discrete IV + normal DV (more than two groups)
20. **Student's t test**: two-valued IV + normal DV
21. **Look at your data; save your data** — two rules of statistical analysis
22. **Group studies**: harder than single-user — more participants, scheduling, task design, data synchronization, extreme variation
23. **Ethnography**: detailed contextual recording; observer remains outside the situation
24. **Think aloud**: user describes thoughts — simple but subjective, affects performance
25. **Cooperative evaluation**: user + evaluator collaborate; user encouraged to criticize system; evaluator can ask "why?" and "what-if?"
26. **Protocol analysis**: paper/audio/video/logging/notebooks — mixed methods in practice
27. **EVA (Experimental Video Annotator)**: automatic protocol analysis tool; tag events during recording
28. **Post-task walkthroughs**: transcript replay — immediate or delayed; essential when user can't talk during task
29. **Interviews**: flexible, probe deeply, subjective, time-consuming; top-down approach
30. **Questionnaires**: quick, large groups, rigorous — **5 question styles** (general, open-ended, scalar, multi-choice, ranked)
31. **Scalar scales**: 1–5 or 1–7 most effective; odd-numbered for neutral option
32. **Pilot study**: test questionnaire on 4–5 users before distribution
33. **Return rate**: questionnaires typically 25–30%; send to random subset
34. **Eye tracking**: fixations (difficulty), saccades (movement), scan path (search strategy/cognitive load)
35. **Physiological measures**: GSR (arousal/mental effort), EMG (task involvement), EEG (decision making/attention), heart activity (stress)
36. **Limitation of physiological measures**: unclear relationship between changes and specific interaction events
37. **Choosing method**: **8 dimensions** — stage, style, objectivity, measures, information level, immediacy, intrusiveness, resources
38. **No single best method** — match to your stage, needs, and resources
39. **Discount usability**: heuristic evaluation is cheap, flexible, works at any stage
40. **Nielsen & Landauer**: 1 user → ~33% problems; 5 users → ~75% problems
