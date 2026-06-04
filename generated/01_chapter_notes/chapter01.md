# Chapter 1: The Human — The User We Design For

## The Big Picture

HCI starts with understanding the **human**. Every interface is built for a person with specific capabilities and limits. This chapter breaks down who that person is: how they take in information (senses), store it (memory), process it (thinking), make errors, feel emotions, and differ from one another.

Think of the human as an **information processing system**:

```
Input (senses) → Memory (storage) → Processing (thinking) → Output (movement/action)
                      ↑                              ↓
                  Emotion (affects everything)    Errors (inevitable)
```

---

## 1. INPUT — How Humans Perceive the World

### Vision — The Dominant Sense

Vision happens in **two stages**:
1. **Physical reception** — light enters the eye, hits the retina
2. **Processing & interpretation** — the brain makes sense of the signal

**The eye**: Light reflects off objects and is focused **upside-down** on the retina. The retina has two kinds of photoreceptors:
- **Rods** — work in low light, no colour
- **Cones** — handle colour vision, need bright light

**Ganglion cells** (technically in the brain, not the eye) detect patterns and movement.

**How we perceive the world**:
| Aspect | Key Facts |
|--------|-----------|
| **Size & Depth** | Visual angle = how much of your view an object occupies. Visual acuity is limited. Familiar objects seem constant size. Overlapping cues help depth perception. |
| **Brightness** | Subjective reaction to luminance. Measured by "just noticeable difference." Acuity and flicker increase with luminance. |
| **Colour** | 3 dimensions: hue, intensity, saturation. Blue acuity is lowest. **8% of males, 1% of females are colour blind.** |
| **Compensation** | The visual system adapts to movement and lighting. Context resolves ambiguity. **Optical illusions** happen when it overcompensates (e.g., Ponzo illusion, Muller-Lyer illusion). |

### Reading — A Special Case of Vision

Reading is a multi-stage process:
1. Perceive the visual pattern
2. Decode using internal language representation
3. Interpret using syntax, semantics, pragmatics

Key facts: Reading uses **saccades** (fast eye jumps) and **fixations** (pauses where perception happens). **Word shape** matters for recognition. **Negative contrast** (dark text on light background) improves screen readability.

### Hearing — The Secondary Channel

The ear has three parts: **outer** (amplifies & protects), **middle** (transmits vibrations), **inner** (converts to nerve impulses).

Sound has three properties:
- **Pitch** — frequency
- **Loudness** — amplitude
- **Timbre** — quality

Humans hear **20Hz to 15kHz**, are less accurate at high frequencies, and can filter sounds (the **cocktail party phenomenon** — focusing on one voice in noise).

### Touch — The Underappreciated Sense

Skin has three receptor types:
- **Thermoreceptors** — heat and cold
- **Nociceptors** — pain
- **Mechanoreceptors** — pressure (some instant, some continuous)

**Kinesthesia** (awareness of body position) affects comfort and performance. Some areas (like fingers) are far more sensitive than others.

### Movement — The Output Channel

Response time = **reaction time + movement time**

| Stimulus | Reaction Time |
|----------|--------------|
| Visual | ~200ms |
| Auditory | ~150ms |
| Pain | ~700ms |

**Fitts' Law** predicts movement time to a target:

> **Mt = a + b log₂(D/S + 1)**

Where D = distance to target, S = target size. **Design rule**: make targets **large** and distances **small**.

---

## 2. STORAGE — The Three Memory Systems

Memory flows through three stages:

```
Sensory Memory → (Attention) → Short-Term/Working Memory → (Rehearsal) → Long-Term Memory
```

### Sensory Memory
Ultra-short buffers for each sense:
- **Iconic** (visual) — e.g., a sparkler's trail
- **Echoic** (aural) — e.g., stereo sound persistence
- **Haptic** (tactile)

Continuously overwritten by new input.

### Short-Term Memory (STM)
The "scratch pad" for temporary recall:
- **Rapid access** (~70ms)
- **Rapid decay** (~200ms)
- **Limited capacity**: **7 ± 2 chunks**

**Chunking** groups items to fit more in STM:
- Raw: 212348278493202
- Chunked: 0121 414 2626
- Meaningful: HEC ATR ANU PTH ETR EET

### Long-Term Memory (LTM)
The permanent repository:
- **Slow access** (~1/10 second)
- **Very slow decay** (practically permanent)
- **Huge/unlimited capacity**

**Two types**:
1. **Episodic** — serial memory of events (autobiographical)
2. **Semantic** — structured memory of facts, concepts, skills (derived from episodic)

**How LTM is structured** (four models):

| Model | How It Works | Example |
|-------|-------------|---------|
| **Semantic Network** | Nodes with inheritance; child inherits parent properties | ANIMAL → DOG → COLLIE → LASSIE; Collie inherits "barks" from Dog |
| **Frames** | Slots with fixed/default/variable values | DOG: legs=4 (fixed), diet=carnivorous (default), colour=? (variable) |
| **Scripts** | Stereotypical situations with entry conditions, props, roles, scenes, tracks | Visit to the vet: dog ill → vet examines → owner pays |
| **Production Rules** | IF condition THEN action | IF dog is wagging tail THEN pat dog |

**How we remember (and forget)**:
- **Storage**: rehearsal moves STM → LTM. Total time hypothesis (more rehearsal = more retention). Distributed practice is better than cramming. Structure, meaning, and familiarity help.
- **Forgetting**: decay (gradual loss) and interference (new info replaces old = **retroactive**; old interferes with new = **proactive**). Memory is selective and affected by emotion.
- **Retrieval**: **Recall** (reproduce from memory, aided by cues) vs. **Recognition** (recognize as seen before — easier).

---

## 3. PROCESSING — How Humans Think

### Reasoning — Three Types

| Type | Description | Reliability |
|------|-------------|-------------|
| **Deduction** | Logically necessary conclusion from premises | Valid logic ≠ true in reality (people bring world knowledge) |
| **Induction** | Generalize from seen to unseen | Unreliable (can't prove true, only false), but useful |
| **Abduction** | Reason from event to cause | Unreliable (can lead to false explanations) |

**Wason's Cards**: Given cards showing 7, E, 4, K and the rule "If vowel → even number on other side," most people fail to check the 7 (odd → should have consonant). **Humans are poor at using negative evidence.**

### Problem Solving

Three theories:

1. **Gestalt Theory** — problem solving is both reproductive (using past experience) and productive (insight/restructuring). Insight is real but hard to study.
2. **Problem Space Theory** — problems have states; solving = generating new states using legal operators. **Heuristics** (like means-ends analysis) help choose operators. Works well for well-defined puzzles, less for knowledge-rich domains.
3. **Analogy** — using knowledge from a similar problem in a similar domain. Hard if domains are semantically different.

**Skill Acquisition**: Skilled performers use **chunking** — conceptual rather than surface-level grouping of problems. Information is structured more effectively.

---

## 4. OUTPUT — Errors Are Inevitable

### Slips vs. Mistakes

| Type | What Happens | Cause | Fix |
|------|-------------|-------|-----|
| **Slip** | Right intention, wrong action | Poor skill, inattention | Better **interface design** |
| **Mistake** | Wrong intention | Incorrect mental model | Better **understanding** of the system |

People build **mental models** to explain how a system works. If the mental model is wrong, mistakes follow.

---

## 5. THE MODULATOR — Emotion Affects Everything

### Theories of Emotion

- **James-Lange**: Emotion = interpretation of physiological response (we feel afraid because we run)
- **Cannon**: Emotion = psychological response to stimuli
- **Schacter-Singer**: Emotion = evaluation of physiological response in context

### Affect in Design

- **Positive affect** → creative problem solving, more forgiving of design flaws
- **Negative affect** → narrow thinking, harder to do even easy tasks

**Design implication**: Stress increases difficulty. Relaxed users are more forgiving. **Aesthetically pleasing interfaces increase positive affect.**

---

## 6. VARIATION — No Two Users Are Alike

### Individual Differences

- **Long-term**: sex, physical and intellectual abilities
- **Short-term**: stress, fatigue
- **Changing**: age

**Design question**: Will your design decision exclude a section of the user population?

---

## 7. BRIDGING PSYCHOLOGY TO DESIGN

Psychology knowledge feeds directly into design through:
- **Guidelines** (Chapter 7) — distilled principles
- **Cognitive models** (Chapter 12) — predicting user behavior
- **Evaluation techniques** (Chapter 9) — testing with real users

**Example**: Blue acuity is poor → don't use blue for critical detail.

But context matters — psychological findings depend on specific experimental conditions. Apply with understanding, not as rigid rules.

---

## KEY CONCEPTS FOR EXAM

1. **Human info processing**: Input (senses) → Memory → Processing → Output, modulated by emotion
2. **Vision stages**: Physical reception + interpretation; rods (low light) vs cones (colour)
3. **Colour**: hue/intensity/saturation; blue acuity lowest; 8% males/1% females colour blind
4. **Reading**: saccades + fixations; word shape important; negative contrast better
5. **Hearing**: 20Hz-15kHz; cocktail party phenomenon; pitch/loudness/timbre
6. **Touch**: thermoreceptors, nociceptors, mechanoreceptors; kinesthesia
7. **Fitts' Law**: Mt = a + b log₂(D/S + 1) → large targets, short distances
8. **Sensory memory**: iconic (visual), echoic (aural), haptic (tactile) — continuously overwritten
9. **STM**: 7±2 chunks, rapid decay (~200ms), rapid access (~70ms), chunking
10. **LTM**: episodic (events) vs semantic (facts); unlimited capacity; slow access (~100ms)
11. **Semantic networks**: inheritance, supports inference
12. **Frames**: slots with fixed/default/variable values
13. **Scripts**: stereotypical situations with entry conditions, props, roles, scenes, tracks
14. **Production rules**: IF condition THEN action (procedural knowledge)
15. **Deduction**: logically necessary conclusion (may not be true in reality)
16. **Induction**: generalize seen→unseen (unreliable but useful); poor at negative evidence (Wason)
17. **Abduction**: event→cause reasoning (unreliable)
18. **Problem Space Theory**: states + operators + heuristics (means-ends analysis)
19. **Slips**: right intention, wrong action (fix: interface design)
20. **Mistakes**: wrong intention (fix: better understanding)
21. **Emotion**: positive affect → creative; negative → narrow; aesthetics matter
22. **Individual differences**: long/short-term/changing — don't exclude users
