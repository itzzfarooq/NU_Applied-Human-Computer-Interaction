# Chapter 7: Design Rules — Principles, Standards, and Heuristics for Usability

## The Big Picture

Chapters 5 and 6 covered *how* to design and *how* to fit HCI into the software process. This chapter provides the **rules of thumb** — the accumulated wisdom that helps designers make good decisions without reinventing the wheel every time.

Design rules exist on a spectrum from **abstract principles** (high generality, low authority) to **specific standards** (low generality, high authority). Guidelines sit in between.

---

## 1. THE SPECTRUM OF DESIGN RULES

```
Generality ↑                    Authority ↓
       Principles (abstract, flexible)
       Guidelines (moderate)
       Standards (specific, rigid)
Generality ↓                    Authority ↑
```

**Trade-off**: The more general a rule, the more situations it applies to — but the harder it is to enforce or verify. The more specific, the more enforceable — but the fewer situations it fits.

---

## 2. THREE PRINCIPLES TO SUPPORT USABILITY

Everything in this chapter traces back to three high-level principles:

| Principle | Question It Answers |
|-----------|-------------------|
| **Learnability** | Can new users start using it easily? |
| **Flexibility** | Can users interact in multiple ways? |
| **Robustness** | Does it support users in achieving their goals? |

---

## 3. LEARNABILITY — Making It Easy to Start

Five sub-principles that make a system easy to learn:

| Principle | Definition | Practical Example |
|-----------|-----------|------------------|
| **Predictability** | Can you determine effect of future actions from past experience? | "Save" button always works the same way |
| **Synthesizability** | Can you assess the effect of past actions? | Undo tells you what was undone |
| **Familiarity** | Does prior knowledge apply? (Guessability / Affordance) | Trash can icon = delete |
| **Generalizability** | Can you extend specific knowledge to new situations? | Ctrl+C / Ctrl+V in any app |
| **Consistency** | Similar situations → similar input/output behaviour | All dialogs have OK/Cancel in same order |

---

## 4. FLEXIBILITY — Supporting Multiple Ways to Interact

Five sub-principles that give users choice:

| Principle | Definition | Example |
|-----------|-----------|---------|
| **Dialogue Initiative** | Freedom from system-imposed constraints | User can interrupt system, not just respond |
| **Multithreading** | Support multiple tasks at once | Concurrent (split screen) vs. interleaving (tab switching) |
| **Task Migratability** | Pass responsibility between user and system | Spellcheck: system finds errors, user decides |
| **Substitutivity** | Equivalent values can substitute for each other | Enter a date by typing or calendar picker |
| **Customizability** | UI can be modified | **Adaptability** (user changes settings) vs. **Adaptivity** (system auto-adapts) |

---

## 5. ROBUSTNESS — Supporting Goal Achievement

Four sub-principles that ensure users can accomplish their goals:

| Principle | Definition | Key Concepts |
|-----------|-----------|-------------|
| **Observability** | Can user evaluate system state from what they see? | Browsability, defaults, reachability, persistence |
| **Recoverability** | Can user correct errors once recognized? | Undo, forward/backward recovery, commensurate effort |
| **Responsiveness** | How fast does the system feel? | Stability of response (consistent speed matters) |
| **Task Conformance** | Does the system support all of the user's tasks? | Task completeness & task adequacy |

---

## 6. STANDARDS — The Rule of Law

**Standards** are set by national or international bodies. They have **high authority** but apply to **narrow situations**.

- Hardware standards are more common than software
- Require sound underlying theory and stable technology
- **ISO 9241** — defines usability as effectiveness, efficiency, satisfaction

---

## 7. GUIDELINES — The Middle Ground

**Guidelines** are more suggestive than standards, more concrete than principles.

| Type | When Applied | Example |
|------|-------------|---------|
| **Abstract (principles)** | Early lifecycle | "Be consistent" |
| **Detailed (style guides)** | Later lifecycle | "Use 12pt sans-serif for body text" |

Best practice: understand the **justification** behind guidelines — this helps resolve conflicts when they contradict each other.

---

## 8. GOLDEN RULES AND HEURISTICS — The Practitioner's Toolkit

"Broad brush" design rules. Not perfect, but **better than nothing**. Three famous collections:

### Nielsen's 10 Heuristics

1. **Visibility of system status** — keep users informed about what's happening
2. **Match between system and the real world** — speak the user's language
3. **User control and freedom** — easy undo/redo, "emergency exit"
4. **Consistency and standards** — follow platform conventions
5. **Error prevention** — better than good error messages
6. **Recognition rather than recall** — minimize memory load
7. **Flexibility and efficiency of use** — accelerators for experts
8. **Aesthetic and minimalist design** — no irrelevant information
9. **Help users recognize, diagnose, and recover from errors** — clear error messages
10. **Help and documentation** — searchable, concrete, step-by-step

### Shneiderman's 8 Golden Rules

1. **Strive for consistency** — similar actions, similar results
2. **Enable frequent users to use shortcuts** — accelerators for experts
3. **Offer informative feedback** — every action should have a response
4. **Design dialogs to yield closure** — tell users when they're done
5. **Offer error prevention and simple error handling** — prevent, then forgive
6. **Permit easy reversal of actions** — undo is essential
7. **Support internal locus of control** — users feel in charge, not the system
8. **Reduce short-term memory load** — don't make users remember (7±2 rule)

### Norman's 7 Principles

1. **Use both knowledge in the world and knowledge in the head** — don't rely on memory alone
2. **Simplify the structure of tasks** — reduce complexity
3. **Make things visible** — bridge the gulfs of Execution and Evaluation
4. **Get the mappings right** — natural relationships between controls and effects
5. **Exploit the power of constraints** — natural and artificial
6. **Design for error** — assume errors will happen
7. **When all else fails, standardize** — if you can't make it intuitive, make it consistent

---

## 9. HCI DESIGN PATTERNS — Reusable Solutions

### What Are Patterns?

Originated in architecture (Christopher Alexander). A pattern is an **invariant solution to a recurrent problem within a specific context**.

**Examples**:
- Architecture: "Light on Two Sides of Every Room"
- HCI: "Go back to a safe place"

### Pattern Languages

Patterns don't exist in isolation — they link to other patterns in **languages** that enable complete designs.

### Characteristics of Good Patterns

- Capture **practice** not theory
- Capture the essential common properties of good designs
- Represent knowledge at varying levels: social, organizational, conceptual, detailed
- Embody values — can express what is humane in interface design
- Intuitive and readable — usable by all stakeholders, not just designers
- A pattern language should be **generative** — it should help create complete designs

---

## KEY CONCEPTS FOR EXAM

1. **Types of design rules**: principles (abstract, low authority) → guidelines → standards (specific, high authority)
2. **Learnability**: ease for new users — predictability, synthesizability, familiarity, generalizability, consistency
3. **Flexibility**: multiple interaction ways — dialogue initiative, multithreading, task migratability, substitutivity, customizability
4. **Robustness**: goal achievement support — observability, recoverability, responsiveness, task conformance
5. **ISO 9241**: effectiveness, efficiency, satisfaction
6. **Nielsen's 10 Heuristics**: visibility, real-world match, user control, consistency, error prevention, recognition over recall, flexibility, aesthetics, error recovery, help
7. **Shneiderman's 8 Golden Rules**: consistency, shortcuts, feedback, closure, error prevention, reversal, locus of control, reduce memory load
8. **Norman's 7 Principles**: knowledge in world/head, simplify tasks, visibility, mappings, constraints, design for error, standardize
8. **Design patterns**: invariant solution to recurrent problem — capture practice, pattern languages
