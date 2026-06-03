# Chapter 9: Evaluation Techniques - HCI Notes

## Overview
Chapter 9 covers evaluation methods for HCI: the rationale for evaluation, goals, expert evaluation (cognitive walkthrough, heuristic evaluation, review-based), user-based evaluation (lab/field studies), experimental evaluation, observational methods, query techniques, physiological methods, and choosing the right evaluation method.

---

## 1. WHAT IS EVALUATION?

### Definition
- Tests usability and functionality of system
- Occurs in laboratory, field and/or in collaboration with users
- Evaluates both design and implementation
- Should be considered at all stages in the design life cycle

### Goals of Evaluation
1. Assess extent of system functionality
2. Assess effect of interface on user
3. Identify specific problems

---

## 2. EVALUATING DESIGNS

### Three Methods
1. Cognitive Walkthrough
2. Heuristic Evaluation
3. Review-based Evaluation

### Cognitive Walkthrough
- Proposed by Polson et al.
- Evaluates design on how well it supports user in learning task
- Usually performed by expert in cognitive psychology
- Expert 'walks through' design to identify potential problems using psychological principles
- Forms used to guide analysis

#### For Each Task Walkthrough Considers
- What impact will interaction have on user?
- What cognitive processes are required?
- What learning problems may occur?

#### Analysis Focus
- Goals and knowledge: does the design lead the user to generate the correct goals?

### Heuristic Evaluation
- Proposed by Nielsen and Molich
- Usability criteria (heuristics) are identified
- Design examined by experts to see if these are violated

#### Example Heuristics
- System behaviour is predictable
- System behaviour is consistent
- Feedback is provided

Heuristic evaluation 'debugs' design.

### Review-based Evaluation
- Results from the literature used to support or refute parts of design
- Care needed to ensure results are transferable to new design
- **Model-based evaluation**: cognitive models used to filter design options (e.g. GOMS prediction)
- Design rationale can also provide useful evaluation information

---

## 3. EVALUATING THROUGH USER PARTICIPATION

### Laboratory Studies
**Advantages:**
- Specialist equipment available
- Uninterrupted environment

**Disadvantages:**
- Lack of context
- Difficult to observe several users cooperating

**Appropriate when:**
- System location is dangerous or impractical
- Constrained single user systems
- Need controlled manipulation of use

### Field Studies
**Advantages:**
- Natural environment
- Context retained (though observation may alter it)
- Longitudinal studies possible

**Disadvantages:**
- Distractions
- Noise

**Appropriate when:**
- Context is crucial
- Longitudinal studies

---

## 4. EVALUATING IMPLEMENTATIONS

Requires an artefact: simulation, prototype, or full implementation.

---

## 5. EXPERIMENTAL EVALUATION

### Definition
Controlled evaluation of specific aspects of interactive behaviour.

### Process
1. Evaluator chooses hypothesis to be tested
2. A number of experimental conditions are considered which differ only in the value of some controlled variable
3. Changes in behavioural measure are attributed to different conditions

### Experimental Factors
- **Subjects** – who: representative, sufficient sample
- **Variables** – things to modify and measure
- **Hypothesis** – what you'd like to show
- **Experimental design** – how you are going to do it

### Variables
- **Independent variable (IV)**: characteristic changed to produce different conditions (e.g. interface style, number of menu items)
- **Dependent variable (DV)**: characteristics measured in the experiment (e.g. time taken, number of errors)

### Hypothesis
- Prediction of outcome, framed in terms of IV and DV
- Example: "error rate will increase as font size decreases"
- **Null hypothesis**: states no difference between conditions – aim is to disprove this

### Experimental Design

#### Within Groups Design
- Each subject performs experiment under each condition
- Transfer of learning possible
- Less costly and less likely to suffer from user variation

#### Between Groups Design
- Each subject performs under only one condition
- No transfer of learning
- More users required
- Variation can bias results

---

## 6. ANALYSIS OF DATA

### Before Statistics
- Look at data
- Save original data

### Choice of Statistical Technique
Depends on:
- Type of data
- Information required

### Type of Data
- **Discrete** – finite number of values
- **Continuous** – any value

### Types of Test
- **Parametric** – assume normal distribution, robust, powerful
- **Non-parametric** – do not assume normal distribution, less powerful, more reliable
- **Contingency table** – classify data by discrete attributes, count number in each group

### What Information is Required?
- Is there a difference?
- How big is the difference?
- How accurate is the estimate?

Parametric and non-parametric tests mainly address the first question.

---

## 7. EXPERIMENTAL STUDIES ON GROUPS

### Difficulties
More difficult than single-user experiments.

Problems with:
- Subject groups
- Choice of task
- Data gathering
- Analysis

### Subject Groups
- Larger number of subjects → more expensive
- Longer time to 'settle down' → even more variation!
- Difficult to timetable
- So... often only three or four groups

### The Task
Must encourage cooperation. Perhaps involve multiple channels.

Options:
- **Creative task** – e.g. 'write a short report on ...'
- **Decision games** – e.g. desert survival task
- **Control task** – e.g. ARKola bottling plant

### Data Gathering
- Several video cameras + direct logging of application
- Problems: synchronization, sheer volume!
- One solution: record from each perspective

### Analysis
- Vast variation between groups
- Solutions: within groups experiments, micro-analysis (e.g. gaps in speech), anecdotal and qualitative analysis
- Look at interactions between group and media
- Controlled experiments may 'waste' resources!

---

## 8. FIELD STUDIES

### Key Concepts
- Experiments dominated by group formation
- Field studies more realistic
- **Distributed cognition** → work studied in context
- Real action is **situated action**
- Physical and social environment both crucial

### Contrast
- Psychology – controlled experiment
- Sociology and anthropology – open study and rich data

---

## 9. OBSERVATIONAL METHODS

### Five Methods
1. Think Aloud
2. Cooperative Evaluation
3. Protocol Analysis
4. Automated Analysis (EVA)
5. Post-task Walkthroughs

### Think Aloud
- User observed performing task
- User asked to describe what he is doing and why, what he thinks is happening etc.

**Advantages:**
- Simplicity – requires little expertise
- Can provide useful insight
- Can show how system is actually used

**Disadvantages:**
- Subjective
- Selective
- Act of describing may alter task performance

### Cooperative Evaluation
- Variation on think aloud
- User collaborates in evaluation
- Both user and evaluator can ask each other questions throughout

**Additional Advantages:**
- Less constrained and easier to use
- User is encouraged to criticize system
- Clarification possible

### Protocol Analysis
- **Paper and pencil** – cheap, limited to writing speed
- **Audio** – good for think aloud, difficult to match with other protocols
- **Video** – accurate and realistic, needs special equipment, obtrusive
- **Computer logging** – automatic and unobtrusive, large amounts of data difficult to analyze
- **User notebooks** – coarse and subjective, useful insights, good for longitudinal studies

- Mixed use in practice
- Audio/video transcription difficult and requires skill
- Some automatic support tools available

---

## 10. AUTOMATED ANALYSIS – EVA

### Workplace Project
- Post task walkthrough
- User reacts on action after the event
- Used to fill in intention

### Advantages
- Analyst has time to focus on relevant incidents
- Avoid excessive interruption of task

### Disadvantages
- Lack of freshness
- May be post-hoc interpretation of events

---

## 11. POST-TASK WALKTHROUGHS

### Process
- Transcript played back to participant for comment
  - **Immediately** → fresh in mind
  - **Delayed** → evaluator has time to identify questions

### Purpose
- Useful to identify reasons for actions and alternatives considered
- Necessary in cases where think aloud is not possible

---

## 12. QUERY TECHNIQUES

### Interviews
- Analyst questions user on one-to-one basis
- Usually based on prepared questions
- Informal, subjective and relatively cheap

**Advantages:**
- Can be varied to suit context
- Issues can be explored more fully
- Can elicit user views and identify unanticipated problems

**Disadvantages:**
- Very subjective
- Time consuming

### Questionnaires
- Set of fixed questions given to users

**Advantages:**
- Quick and reaches large user group
- Can be analyzed more rigorously

**Disadvantages:**
- Less flexible
- Less probing

#### Design Considerations
- Need careful design:
  - What information is required?
  - How are answers to be analyzed?

#### Styles of Question
- **General** – broad, open questions
- **Open-ended** – free-form responses
- **Scalar** – Likert scale ratings
- **Multi-choice** – select from options
- **Ranked** – order items by preference

---

## 13. PHYSIOLOGICAL METHODS

### Two Types
1. Eye tracking
2. Physiological measurement

### Eye Tracking
- Head or desk mounted equipment tracks the position of the eye
- Eye movement reflects the amount of cognitive processing a display requires

**Measurements:**
- **Fixations**: Eye maintains stable position. Number and duration indicate level of difficulty with display
- **Saccades**: Rapid eye movement from one point of interest to another
- **Scan paths**: Moving straight to a target with a short fixation at the target is optimal

### Physiological Measurements
- Emotional response linked to physical changes
- These may help determine a user's reaction to an interface

**Measurements Include:**
- **Heart activity**: Blood pressure, volume and pulse
- **Galvanic Skin Response (GSR)**: Activity of sweat glands
- **Electromyogram (EMG)**: Electrical activity in muscle
- **Electroencephalogram (EEG)**: Electrical activity in brain

**Limitation:** Some difficulty in interpreting these physiological responses – more research needed

---

## 14. CHOOSING AN EVALUATION METHOD

### Seven Key Dimensions

| Dimension | Options |
|-----------|---------|
| **When in process** | Design vs. Implementation |
| **Style of evaluation** | Laboratory vs. Field |
| **How objective** | Subjective vs. Objective |
| **Type of measures** | Qualitative vs. Quantitative |
| **Level of information** | High level vs. Low level |
| **Level of interference** | Obtrusive vs. Unobtrusive |
| **Resources available** | Time, subjects, equipment, expertise |

---

## KEY CONCEPTS FOR EXAM
1. **Evaluation goals**: assess functionality, assess effect on user, identify problems
2. **Cognitive walkthrough**: expert walks through design, evaluates learning support
3. **Heuristic evaluation**: experts check for heuristic violations (Nielsen & Molich)
4. **Review-based evaluation**: literature results support/refute design, GOMS prediction
5. **Laboratory studies**: specialist equipment, uninterrupted, but lack context
6. **Field studies**: natural environment, context retained, longitudinal possible
7. **Experimental evaluation**: controlled, IV/DV, hypothesis testing
8. **Independent variable (IV)**: changed to produce different conditions
9. **Dependent variable (DV)**: measured in experiment
10. **Null hypothesis**: no difference – aim is to disprove
11. **Within groups**: each subject performs under each condition (transfer possible, less costly)
12. **Between groups**: each subject under one condition (no transfer, more users needed)
13. **Parametric tests**: assume normal distribution, robust, powerful
14. **Non-parametric tests**: no normal distribution assumption, less powerful, more reliable
15. **Group studies**: harder than single-user, problems with subjects/tasks/data/analysis
16. **Distributed cognition**: work studied in context
17. **Situated action**: real action, physical and social environment crucial
18. **Think aloud**: user describes thoughts, simple but subjective
19. **Cooperative evaluation**: user + evaluator collaborate, less constrained
20. **Protocol analysis**: paper, audio, video, logging, notebooks – mixed use
21. **EVA**: post-task walkthrough, user reacts after event
22. **Post-task walkthroughs**: transcript played back, immediate vs delayed
23. **Interviews**: one-to-one, informal, subjective, cheap
24. **Questionnaires**: fixed questions, quick, large groups, rigorous analysis
25. **Question styles**: general, open-ended, scalar, multi-choice, ranked
26. **Eye tracking**: fixations (difficulty), saccades (movement), scan paths (optimal)
27. **Physiological measurements**: GSR (sweat), EMG (muscle), EEG (brain), heart activity
28. **Choosing method**: 7 dimensions – process stage, lab/field, subjective/objective, qualitative/quantitative, high/low info, obtrusive/unobtrusive, resources
