# Chapter 6: HCI in the Software Process — Building Usability Into Engineering

## The Big Picture

Previous chapters focused on *what* to design. This chapter focuses on *how* to fit HCI activities into the standard software engineering lifecycle. The conflict: traditional software engineering is **linear** (waterfall), but good UI design is **iterative**. This chapter explores how to reconcile them.

**Core tension**: Software engineers want to plan everything upfront. HCI designers need to iterate based on user feedback. The solution involves usability engineering, prototyping, and design rationale.

---

## 1. THE SOFTWARE LIFECYCLE

### The Waterfall Model — The Traditional View

Classic software engineering divides development into sequential stages:

```
Requirements → Architecture → Detailed Design → Coding → Integration → Maintenance
```

**Problem for HCI**: This assumes you can specify all requirements upfront. But for interactive systems, **you can't know the right interface until users try it**. The waterfall doesn't allow for the feedback loops that HCI requires.

**Reality for interactive systems**: Multiple feedback loops between all stages. Design is never linear.

### Verification vs. Validation

| | Definition | Question |
|---|---|---|
| **Verification** | Designing the product **right** | "Does it meet the spec?" |
| **Validation** | Designing the **right** product | "Does it solve the user's problem?" |

**The formality gap**: Validation always relies on subjective proof — you can't fully automate the question "is this good for users?"

---

## 2. USABILITY ENGINEERING — Making Usability Measurable

Usability engineering demands that **specific usability measures be made explicit as requirements** — just like performance requirements.

### Usability Specification

Each usability attribute is specified across five dimensions:

| Dimension | What It Is | Example (VCR undo) |
|-----------|-----------|-------------------|
| **Attribute** | The usability principle | Backward recoverability |
| **Measuring concept** | What to measure | Undo an erroneous programming sequence |
| **Measuring method** | How to measure | Number of explicit user actions to undo |
| **Now level** | Current baseline | No product allows undo |
| **Worst case** | Minimum acceptable | As many actions as needed to program it in |
| **Planned level** | Target | Maximum 2 explicit user actions |
| **Best case** | Stretch goal | One explicit cancel action |

### Problems with Usability Engineering
- Requires detail that may not be available early in design
- Satisfying the spec doesn't guarantee actual usability

### ISO 9241 Usability Standard

Three dimensions:

| Dimension | Question |
|-----------|----------|
| **Effectiveness** | Can you achieve what you want? |
| **Efficiency** | Can you do it without wasting effort? |
| **Satisfaction** | Do you enjoy the process? |

### Example ISO Metrics

| Objective | Effectiveness | Efficiency | Satisfaction |
|-----------|--------------|------------|--------------|
| Suitability for task | % goals achieved | Time to complete | Rating scale |
| Learnability | % functions learned | Time to learn criterion | Ease-of-learning scale |
| Error tolerance | % errors corrected | Time correcting errors | Error-handling scale |

---

## 3. ITERATIVE DESIGN AND PROTOTYPING

### Why Iterate?

Because requirements are always incomplete initially. The only way to discover what users really need is to **show them something and get feedback**.

### Types of Prototypes

| Type | How It Works | When to Use |
|------|-------------|-------------|
| **Throwaway** | Build quickly, discard after learning | Early exploration |
| **Incremental** | Build piece by piece, add to final system | When parts are independent |
| **Evolutionary** | Prototype evolves into final product | When direction is clear but details aren't |

### Prototyping Techniques

**Storyboards**: Visual representation of user interaction flow. Need not be computer-based. Can be animated.

**Limited Functionality Simulations**: Some part of system functionality provided by designers (e.g., HyperCard).

**Wizard of Oz**: A human simulates the computer's response behind the scenes. User thinks they're interacting with a real system.

### Warning — Design Inertia

Early bad decisions tend to persist. Be careful diagnosing real usability problems vs. just treating symptoms.

---

## 4. DESIGN RATIONALE — Why the System Is the Way It Is

**Design rationale** = the information that explains why design decisions were made.

### Benefits

1. **Communication** — keeps everyone on the same page across the lifecycle
2. **Reuse** — design knowledge transfers to future products
3. **Discipline** — forces designers to justify decisions
4. **Trade-off analysis** — makes design space explicit
5. **Organization** — structures a potentially large design space
6. **Context** — captures the reasoning, not just the result

### Two Approaches

| Approach | Focus | Preserves |
|----------|-------|-----------|
| **Process-oriented** | Order of deliberation and decisions | The journey |
| **Structure-oriented** | Post-hoc structuring of alternatives | The map |

---

## 5. IBIS — Issue-Based Information System

Process-oriented. Structures design discussions around three elements:

```
Issue (a problem to resolve)
  ├── Position (a proposed resolution)
  │     ├── Argument (supports the position)
  │     └── Argument (objects to the position)
  ├── Position (another resolution)
  │     └── Argument (supports)
  └── Sub-issue (a related sub-problem)
```

**gIBIS** = graphical IBIS, showing the structure as a node diagram.

---

## 6. DESIGN SPACE ANALYSIS

### QOC — Questions, Options, Criteria

Structure-oriented. Maps the design space:

```
Question (what to decide)
  ├── Option A (possible solution)
  │     └── Criteria (how to evaluate)
  ├── Option B
  │     └── Criteria
  └── Option C
        └── Criteria
```

### DRL — Design Rationale Language

Similar to QOC but larger vocabulary and more formal semantics.

---

## 7. PSYCHOLOGICAL DESIGN RATIONALE

Focuses on making explicit the **consequences of design for users**:

1. Identify tasks the system will support
2. Suggest scenarios to test each task
3. Observe users on the system
4. Make psychological claims explicit
5. Use negative findings to improve next iteration

Supports the **task-artefact cycle**: user tasks are affected by the systems they use, which changes what users want to do, which drives new designs.

---

## KEY CONCEPTS FOR EXAM

1. **Software lifecycle**: requirements → architecture → detailed design → coding → integration → maintenance
2. **Waterfall model**: sequential — doesn't fit interactive systems (need feedback)
3. **Verification**: product right; **Validation**: right product
4. **Formality gap**: validation needs subjective judgement
5. **Usability engineering**: measurable usability requirements
6. **Usability spec**: attribute, measuring concept, method, now/worst/planned/best
7. **ISO 9241**: effectiveness, efficiency, satisfaction
8. **Iterative design**: overcomes incomplete requirements
9. **Prototypes**: throwaway, incremental, evolutionary
10. **Storyboards**: visual user interaction flow
11. **Wizard of Oz**: human simulates computer response
12. **Design rationale**: why the system is the way it is
13. **IBIS/gIBIS**: Issues, Positions, Arguments (process-oriented)
14. **QOC**: Questions, Options, Criteria (structure-oriented)
15. **DRL**: Design Rationale Language — formal QOC variant
16. **Psychological design rationale**: make consequences for users explicit
