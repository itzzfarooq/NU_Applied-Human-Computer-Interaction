# Chapter 5: Interaction Design Basics — How to Actually Design Interfaces

## The Big Picture

This is the **largest and most critical chapter** (92 slides). Previous chapters covered *what* human and computer bring to interaction and *how* we got here. This chapter is about the **process of designing** interactive systems: how to understand users, explore ideas, structure navigation, lay out screens, and iterate toward a good design.

The core message: **design is iterative, user-centered, and never done right the first time.**

---

## 1. THE DESIGN PROCESS

### What is Design?

Design = applying creative thought to produce a **plan** for making something. For interactive systems, the goal is **usable** systems.

### Who Does Design?

Designers don't work in isolation. They collaborate with:
- **Customers/clients** — who pay for it
- **Users** — who will use it
- **Other designers** — who bring different expertise

### User-Centered Design (UCD)

The fundamental principle: **involve users throughout the design process**. You need to understand their tasks, their environment, and their requirements. Use multiple methods to build that understanding.

---

## 2. UNDERSTANDING THE USER

### Who Are the Users?

Not just the person at the keyboard. Also: operators, customers, managers, co-workers, maintenance staff, trainees — anyone affected by the system.

### Techniques for Understanding Users

| Technique | How It Works | When to Use |
|-----------|-------------|-------------|
| **Personas** | Fictional users representing real user categories | Throughout design — keeps users in mind |
| **Cultural probes** | Packages sent to participants to document their own lives | Early exploration of context/culture |
| **Contextual inquiry** | Observe and interview users in their natural work environment | Understanding work practices |

**Personas** are especially powerful — they give designers a concrete person to design for, help argue for features, and should be realistic and research-based.

**Cultural probes** are NOT for direct requirements gathering — they inspire and reveal context.

**Contextual inquiry** builds rapport and reveals what people actually do (vs. what they say they do).

---

## 3. SCENARIOS — Stories About Use

**Scenarios** are stories about users and systems. They capture what a user might do and illustrate how interaction takes place — without specifying exact interface details.

| Type | What It Is | Use Case |
|------|-----------|----------|
| **Concrete** | Specific instance, particular user and task | Exploring specific design alternatives |
| **Abstract** | General pattern, not tied to instance | Understanding general requirements |

Scenarios help **explore alternatives, communicate ideas, evaluate proposals, and document rationale**.

---

## 4. NAVIGATION DESIGN — How Users Move Through the System

### What is Navigation?

Navigation = how users move through an information space. Forward, backward, between different parts of the system.

### Goal-Seeking — How Users Decide What to Do Next

Users look at the current state, consider their goal, and choose an action. **Local navigation** is movement within a small area (menu selection, tab switching).

### The Four Golden Rules of Navigation

1. **Provide landmarks** — help users know **where they are**
2. **Provide routes** — clear **paths** through information
3. **Provide overviews** — show the **overall structure**
4. **Provide context** — show relationship to other parts

**Breadcrumbs** implement all four — they show the path taken, allow return, and provide orientation.

### Modes

| Type | Behaviour | Example |
|------|-----------|---------|
| **Modal** | Interface behaves differently depending on mode | Caps lock, drawing tool modes |
| **Modeless** | Same behaviour regardless of state | Most scroll/zoom interactions |

### Information Structures

| Structure | How It Works | Best For |
|-----------|-------------|----------|
| **Hierarchical** | Tree, parent-child relationships | Well-organized, nested info |
| **Network** | Multiple paths between nodes | Interconnected, non-linear info |

---

## 5. SCREEN DESIGN — The Visual Layer

### Grouping — Gestalt Principles

Our brains automatically group visual elements:

| Principle | What It Means | Design Rule |
|-----------|---------------|-------------|
| **Proximity** | Close items → perceived as group | Group related items together |
| **Similarity** | Alike items → perceived as group | Use consistent styles for same type |
| **Closure** | Mind completes incomplete shapes | You don't need to draw everything |
| **Continuity** | Eye follows smooth paths | Align elements along lines |

### Alignment
- Visual consistency across the interface
- Align elements to a grid
- Creates order, professionalism, reduces clutter

### White Space
- Space between elements = breathing room
- Reduces cognitive load
- Improves readability and comprehension
- **Don't fill every pixel**

### Physical Controls
Buttons, sliders, knobs — consider ergonomics, affordances, and feedback.

---

## 6. USER ACTION AND CONTROL

### Affordances

**Affordance** = a property of an object that suggests how it can be used.
- A button **affords** pressing
- A slider **affords** sliding
- Real objects have **physical** affordances
- Interface objects have **perceived** affordances (learned, not innate)

### Aesthetics

How the interface looks and feels triggers an emotional response. The **aesthetic-usability effect**: attractive things are perceived as working better. Good aesthetics matter for usability, not just beauty.

### Colour in Design

- Use colour meaningfully and consistently
- Consider colour blindness (8% men, 1% women)
- Don't rely on colour alone — use redundant cues

### Internationalisation & Localisation

| | What It Is | When |
|---|---|---|
| **Internationalisation** | Design for multiple cultures from the start | Before building |
| **Localisation** | Adapt a product for a specific locale | Per market |

Consider: text direction, date/time formats, currency, cultural symbols.

---

## 7. PROTOTYPING AND ITERATION

### Prototyping

Create mock-ups to test ideas before building the real thing.

| Dimension | Options |
|-----------|---------|
| **Fidelity** | Low (paper sketches) vs. High (interactive mock-ups) |
| **Strategy** | Throwaway (discard after learning), Evolutionary (refine into final), Incremental (add piece by piece) |

### Iteration — The Heart of Design

```
Test → Learn → Improve → Repeat (until acceptable)
```

**Don't expect to get it right the first time.** Each cycle reveals problems you couldn't have anticipated.

---

## KEY CONCEPTS FOR EXAM

1. **Design process**: iterative, user-involved, multiple methods
2. **User-centered design**: involve users throughout
3. **Personas**: fictional users from research, represent real categories
4. **Cultural probes**: self-documentation packages for context
5. **Contextual inquiry**: observe + interview in natural environment
6. **Scenarios**: stories about use — concrete (specific) or abstract (general)
7. **Navigation**: how users move through information space
8. **4 golden rules**: landmarks, routes, overviews, context
9. **Breadcrumbs**: path shown, enables return, gives orientation
10. **Modes**: modal (context-dependent) vs modeless (consistent)
11. **Gestalt principles**: proximity, similarity, closure, continuity
12. **Grouping**: related together, unrelated separated
13. **Alignment**: grid-based consistency
14. **White space**: reduces cognitive load
15. **Affordances**: perceived properties that suggest use
16. **Aesthetic-usability effect**: attractive → works better (perception)
17. **Colour blindness**: 8% men, 1% women — never rely on colour alone
18. **Internationalisation**: design for multiple cultures upfront
19. **Localisation**: adapt per locale (dates, currency, symbols)
20. **Prototyping**: low/high fidelity; throwaway/evolutionary/incremental
21. **Iteration**: test, learn, improve — never right first time
