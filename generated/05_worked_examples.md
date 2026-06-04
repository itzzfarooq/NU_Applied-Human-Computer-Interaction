# Worked Examples and Case Analyses

## How to Use This Document

Each example walks through a realistic HCI problem step-by-step. Study the reasoning process, not just the answer. Exam questions often mirror these patterns.

---

## Example 1: Heuristic Evaluation Walkthrough

**Scenario**: You are asked to evaluate a mobile banking app's "Transfer Money" screen using Nielsen's 10 Heuristics. The screen shows: a recipient field, an amount field, a "Send" button, and a small "?" icon for help. There is no confirmation step. Error messages appear as red text at the top of the screen.

**Task**: Identify heuristic violations and rate severity.

### Step-by-Step Analysis

| Heuristic | Finding | Violation? | Severity |
|-----------|---------|------------|----------|
| 1. Visibility of system status | No loading indicator after pressing Send | YES | 3 (Major) |
| 2. Match system and real world | Uses "IBAN" without explanation for non-expert users | YES | 2 (Minor) |
| 3. User control and freedom | No undo or cancel after Send; no confirmation dialog | YES | 4 (Catastrophe) |
| 4. Consistency and standards | Help icon placement inconsistent with other screens | YES | 1 (Cosmetic) |
| 5. Error prevention | No confirmation before transferring real money | YES | 4 (Catastrophe) |
| 6. Recognition over recall | Recipient field has no autocomplete from contacts | Partial | 2 (Minor) |
| 7. Flexibility and efficiency | No way to save frequent recipients | YES | 2 (Minor) |
| 8. Aesthetic/minimalist design | Clean layout, only necessary fields shown | No | 0 |
| 9. Help recognize/diagnose/recover from errors | Error text at top is easy to miss; no suggestion for fix | YES | 3 (Major) |
| 10. Help and documentation | "?" icon present but requires leaving the screen | Partial | 2 (Minor) |

### Key Findings

**Critical issues** (severity 4): No confirmation step and no undo for money transfers. These must be fixed before release.

**Major issues** (severity 3): Missing loading feedback and poor error presentation.

**Recommended fixes**:
1. Add confirmation dialog: "Transfer $500 to John? [Cancel] [Confirm]"
2. Add loading spinner after Send
3. Move error messages inline (next to the field they relate to)
4. Add recipient autocomplete from contact list
5. Allow saving frequent recipients

### Exam Takeaway

When performing heuristic evaluation: (1) go through each heuristic systematically, (2) note specific violations with screen locations, (3) rate severity independently, (4) combine evaluator findings — five evaluators find ~75% of problems.

---

## Example 2: Cognitive Walkthrough Analysis

**Scenario**: A new user wants to print a document from a word processor. The interface has: a toolbar with a printer icon, a File menu with "Print" option, and Ctrl+P keyboard shortcut. The user has never used this application before.

**Task**: Perform a cognitive walkthrough for the toolbar printer icon path.

### Step-by-Step (Four Questions per Action)

**Action 1: User notices the toolbar**

| Question | Analysis | Answer |
|----------|----------|--------|
| 1. Is the effect of the action the same as the user's goal? | User wants to print; printer icon suggests printing | YES |
| 2. Will users see the action is available? | Printer icon is visible on toolbar | YES |
| 3. Once found, will users know it's the right action? | Printer icon is universally recognized | YES |
| 4. After action, will users understand feedback? | Print dialog appears — clear confirmation | YES |

**Result**: No usability problem on this path.

**Action 2: User clicks the printer icon**

| Question | Analysis | Answer |
|----------|----------|--------|
| 1. Effect matches goal? | Clicking opens print dialog — matches "print" goal | YES |
| 2. Visible? | Icon was visible and clickable | YES |
| 3. Recognized as correct? | Standard print icon — yes | YES |
| 4. Feedback understood? | Print dialog shows settings and Print button | YES |

**Result**: No problem. But now consider: what if the user doesn't recognize the printer icon? They might try File menu instead.

**Action 3: User opens File menu**

| Question | Analysis | Answer |
|----------|----------|--------|
| 1. Effect matches goal? | File menu often contains Print — yes | YES |
| 2. Visible? | "File" is visible in menu bar | YES |
| 3. Recognized? | Users familiar with menus know File often has Print | YES (for experienced users) |
| 4. Feedback understood? | Menu drops down showing options including Print | YES |

**Result**: For experienced computer users, this path works. For complete novices, the term "File" may not clearly indicate "Print" — potential problem at Question 3.

### Key Findings

The toolbar icon path has no problems for users who recognize the printer icon. The File menu path may confuse novices who don't associate "File" with "Print."

**Design recommendation**: Add a visible "Print" label or tooltip on hover to bridge the gap for novice users.

### Exam Takeaway

Cognitive walkthrough focuses on **learnability** — can a user figure out what to do through exploration? The four questions systematically check each step of the task. Negative answers at any question = usability problem.

---

## Example 3: KLM/GOMS Calculation

**Scenario**: Compare two designs for "send an email" task.

**Design A (Classic)**:
1. Click "Compose" button (toolbar)
2. Type recipient email address (18 keystrokes)
3. Press Tab
4. Type subject line (12 keystrokes)
5. Press Tab
6. Type body (45 keystrokes)
7. Click "Send" button

**Design B (Smart Compose)**:
1. Click "New Message" button (toolbar)
2. Start typing recipient — autocomplete appears after 3 keystrokes
3. Press Enter to accept autocomplete
4. Type subject (12 keystrokes)
5. Press Tab
6. Type body (45 keystrokes)
7. Click "Send" button

### KLM Operator Times

| Operator | Symbol | Time |
|----------|--------|------|
| Keystroke | K | 0.2s |
| Pointing | P | 1.1s |
| Mental preparation | Mh | 1.35s |
| Home (hand to device) | H | 0.4s |

### Design A Calculation

| Step | Operators | Time |
|------|-----------|------|
| Mental: decide to compose | Mh | 1.35s |
| Point to Compose button | P | 1.1s |
| Click | K | 0.2s |
| Mental: think of recipient | Mh | 1.35s |
| Home hand to keyboard | H | 0.4s |
| Type 18-character email | 18K | 3.6s |
| Mental: move to subject | Mh | 1.35s |
| Press Tab | K | 0.2s |
| Type 12-char subject | 12K | 2.4s |
| Mental: move to body | Mh | 1.35s |
| Press Tab | K | 0.2s |
| Type 45-char body | 45K | 9.0s |
| Mental: locate Send | Mh | 1.35s |
| Home hand to mouse | H | 0.4s |
| Point to Send | P | 1.1s |
| Click Send | K | 0.2s |
| **Total** | | **24.6s** |

### Design B Calculation

| Step | Operators | Time |
|------|-----------|------|
| Mental: decide to compose | Mh | 1.35s |
| Point to New Message button | P | 1.1s |
| Click | K | 0.2s |
| Mental: think of recipient | Mh | 1.35s |
| Home hand to keyboard | H | 0.4s |
| Type 3 keystrokes | 3K | 0.6s |
| Mental: recognize autocomplete | Mh | 1.35s |
| Press Enter to accept | K | 0.2s |
| Mental: move to subject | Mh | 1.35s |
| Type 12-char subject | 12K | 2.4s |
| Press Tab | K | 0.2s |
| Mental: move to body | Mh | 1.35s |
| Type 45-char body | 45K | 9.0s |
| Mental: locate Send | Mh | 1.35s |
| Home hand to mouse | H | 0.4s |
| Point to Send | P | 1.1s |
| Click Send | K | 0.2s |
| **Total** | | **23.55s** |

### Comparison

| Metric | Design A | Design B |
|--------|----------|----------|
| Total predicted time | 24.6s | 23.55s |
| Time saved | — | 1.05s (4.3%) |
| Keystrokes | 75 | 60 |

**Design B is faster** due to autocomplete reducing keystrokes from 18 to 3 for the email address. However, the mental operator for recognizing the autocomplete suggestion partially offsets the keystroke savings.

### Exam Takeaway

KLM calculation: list every operator, multiply by standard times, sum. Don't forget mental operators (Mh = 1.35s each) — they are often the largest time component. The formula is: **Total time = Σ(operator times)**.

---

## Example 4: Comparing Two Interface Designs

**Scenario**: A hospital is choosing between two nurse call systems.

**System A (Button-based)**: Each bed has a physical button. Nurse presses button to acknowledge. LED shows call status. Dedicated device at nurse station.

**System B (App-based)**: Each bed has a touchscreen. Nurse uses smartphone app. Push notifications. Dashboard shows all beds. History and notes feature included.

### Comparison Using Usability Principles

| Criterion | System A (Button) | System B (App) | Winner |
|-----------|-------------------|----------------|--------|
| **Learnability** | Instant — one button | Requires training | A |
| **Reliability** | Physical, no network needed | Depends on WiFi/battery | A |
| **Speed of use** | Immediate press | Unlock phone → open app → find bed | A |
| **Error prevention** | Single action, hard to error | Multiple steps, possible errors | A |
| **Flexibility** | None — just acknowledge | Notes, history, prioritization | B |
| **Observability** | LED shows status | Dashboard with overview | B |
| **Recoverability** | None — can't undo | Can reassign, add notes | B |
| **Information** | Binary (call/no call) | Rich (patient info, history) | B |
| **Scalability** | One device per station | Works across hospital | B |
| **Cost** | Low per unit | Higher (software + devices) | A |

### Analysis

**System A wins on core usability** (learnability, reliability, speed, error prevention). In emergencies, simplicity and speed save lives.

**System B wins on information and flexibility**. Better for coordination, documentation, and long-term workflow.

**Recommendation**: System A for emergency call buttons (critical path), System B for status monitoring and documentation (non-critical path). The physical button is the right choice when: task is critical, time pressure is high, and users need zero learning curve.

### Exam Takeaway

When comparing interfaces, don't just list features. Evaluate against **usability principles** (learnability, flexibility, robustness). Consider the **context of use** — a hospital emergency has different needs than an office email system.

---

## Example 5: Scenario-Based Design Problem

**Scenario**: Elderly users (70+) in a care home struggle to video call their families. Current interface: open app → find contact → tap video icon → wait for answer. Problems: small icons, complex navigation, unreliable WiFi causes dropped calls.

**Task**: Suggest a design solution using HCI principles.

### Step 1: Identify User Characteristics (Chapter 1)

- Reduced visual acuity (need larger targets)
- Possible motor tremor (Fitts' Law: large targets, short distances)
- Limited short-term memory (7±2 rule; chunking)
- May have hearing difficulties (visual feedback essential)
- Low frustration tolerance with technology
- Strong emotional motivation (connecting with family)

### Step 2: Apply Design Principles

**Norman's Principles**:
- **Knowledge in the world**: Show family photos as large buttons, not text names
- **Make things visible**: One big button per family member
- **Design for error**: Confirm before calling, easy cancel
- **Constraints**: Limit to 4-5 most-called family members

**Nielsen's Heuristics**:
- **Visibility of system status**: Show "Calling..." with progress
- **User control and freedom**: Easy hang-up, redial
- **Error prevention**: Confirmation dialog before calling
- **Recognition over recall**: Photos instead of names

### Step 3: Proposed Design

**Physical device**: Large tablet mounted on wall. Single physical "Call" button per family member (4 large photo buttons). Each button has the family member's photo and name in large text.

**Workflow**: Press photo button → screen shows "Calling [Name]..." → if no answer after 20 seconds, auto-cancels with message "No answer — try again later?"

**Accessibility features**:
- Volume automatically at maximum
- Visual ring indicator (flashing border) for hearing-impaired
- Auto-answer option for incoming calls
- Button size: 80mm × 80mm (large target per Fitts' Law)

### Exam Takeaway

Scenario-based design: (1) identify user characteristics, (2) map to design principles, (3) propose concrete solution, (4) justify with principles. Always ground your design in the specific user population's capabilities and limitations.

---

## Example 6: Applying Norman's Model to Debug an Interface

**Scenario**: A user wants to resize a window in an unfamiliar application. They try dragging the title bar (nothing happens), then right-click the title bar (context menu appears with "Resize" option), then select Resize (cursor changes), then drag the edge to resize.

**Task**: Analyze this interaction using Norman's 7 stages.

### Stage-by-Stage Analysis

| Stage | User Action | Analysis |
|-------|-------------|----------|
| 1. Goal | "Make window bigger" | Clear goal established |
| 2. Intention | "I will drag the edge to resize" | User forms specific plan |
| 3. Specify action sequence | "Drag title bar to move/resize" | **WRONG** — title bar is for moving, not resizing |
| 4. Execute action | Drags title bar | Action executed — but wrong action for goal |
| 5. Perceive system state | Window moves instead of resizes | Feedback received |
| 6. Interpret state | "That didn't work — it moved, not resized" | User correctly interprets |
| 7. Evaluate | "Goal not achieved" | Loop continues |

### Gap Analysis

**Gulf of Execution** (Stage 3-4): User specified wrong action. The interface didn't make it clear that resizing requires dragging the **edge**, not the title bar. The system allows resizing, but the mapping between user intention and available actions is unclear.

**Gulf of Evaluation** (Stage 5-6): After the first attempt, the user correctly perceived and interpreted the result (window moved, didn't resize). The evaluation gulf is bridged — the user knows what happened.

**Fix**: Add resize handles (visible grips at window corners/edges) to make the resize affordance visible. This bridges the execution gulf by making the correct action discoverable.

### Exam Takeaway

When applying Norman's model: (1) identify the goal, (2) trace through each stage, (3) identify which stage fails, (4) determine if it's an execution or evaluation gulf, (5) propose a fix that bridges that specific gulf.

---

## Example 7: Evaluation Method Selection

**Scenario**: You are designing a new e-commerce checkout flow. You have: 3 weeks until deadline, a paper prototype, a budget of $500, and access to your target users.

**Task**: Choose the most appropriate evaluation method(s) and justify.

### Analysis Using the 8 Dimensions

| Dimension | Your Situation | Implication |
|-----------|---------------|-------------|
| 1. Stage in cycle | Design stage (paper prototype) | Expert methods preferred |
| 2. Style | Not yet implemented | Lab/field not applicable yet |
| 3. Objectivity | Need qualitative feedback | Subjective methods OK |
| 4. Measures | Want both: specific problems + overall impression | Mixed methods |
| 5. Information level | Need low-level (specific issues) and high-level (is it usable?) | Both levels needed |
| 6. Immediacy | Want real-time feedback during walkthrough | Immediate methods |
| 7. Intrusiveness | Can accept some intrusiveness | Think aloud acceptable |
| 8. Resources | $500, 3 weeks, user access | Moderate resources |

### Recommended Methods

**Primary: Cognitive Walkthrough** (Week 1)
- Works on paper prototype
- Expert analysis — no user cost
- Identifies learnability problems
- Cost: ~$0 (internal expertise)

**Secondary: Think-Aloud with 3-5 Users** (Week 2)
- Test paper prototype with real users
- Users walk through checkout while talking
- Reveals unexpected problems
- Cost: ~$300 (participant incentives at $60-75 each)

**Tertiary: Questionnaire** (Week 3)
- After prototype refinement
- Likert scales on ease-of-use, confidence, satisfaction
- Quantitative data for comparison
- Cost: ~$0

### Methods NOT Recommended (and Why)

| Method | Why Not |
|--------|---------|
| Full experiment | Too early (paper prototype); too expensive; too time-consuming |
| Eye tracking | No implementation to track; equipment too expensive |
| Heuristic evaluation | Good alternative to cognitive walkthrough; either works |
| Field study | Not yet implemented; can't observe in real context |

### Exam Takeaway

Method selection depends on: (1) what stage you're at, (2) what questions you need answered, (3) your resources. There is no single best method — match the method to the situation.

---

## Example 8: Statistical Analysis Decision

**Scenario**: You tested two menu designs (5-item vs. 7-item) with 12 participants. Each participant completed a selection task with both designs (randomized order). You measured time to complete. The data is: Mean(5-item) = 3.2s, Mean(7-item) = 4.1s.

**Task**: What statistical test should you use? Why?

### Step-by-Step Decision

**1. Identify variable types**:
- IV: Menu size (5-item vs. 7-item) — **two-valued** (discrete, two levels)
- DV: Time to complete — **continuous**, positive, likely **normally distributed** (task time = sum of many small components)

**2. Identify experimental design**:
- Each participant experienced BOTH conditions → **within-subjects** (repeated measures)

**3. Check normality assumption**:
- Task completion times are typically normal (central limit theorem applies with complex tasks)
- With 12 participants, assume normality holds unless data shows otherwise

**4. Select test**:

| Factor | Value | Implication |
|--------|-------|-------------|
| IV type | Two-valued | Could use t-test or Wilcoxon |
| DV type | Continuous, normal | Parametric test appropriate |
| Design | Within-subjects | Need paired comparison |
| Normality | Assumed | Parametric OK |

**Decision**: **Paired-samples t-test** (within-subjects variant of Student's t-test)

If normality is violated → use **Wilcoxon signed-rank test** (non-parametric equivalent)

**5. Additional considerations**:
- Counterbalancing: Half did 5-item first, half did 7-item first — controls for learning effects
- Report: mean difference (0.9s), confidence interval, p-value, effect size
- Rule: **Look at your data** (check for outliers), **Save your data** (never discard originals)

### Exam Takeaway

Statistical test selection: (1) Identify IV and DV types, (2) identify experimental design (between/within), (3) check normality assumption, (4) select parametric or non-parametric accordingly. For two-valued IV + normal DV + within-subjects → paired t-test.
