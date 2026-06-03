# Chapter 1: The Human - HCI Notes

## Overview
Chapter 1 covers the human aspects of HCI: perception (vision, hearing, touch), movement, memory systems, thinking/reasoning, emotion, and individual differences. Understanding human capabilities and limitations is fundamental to designing effective interfaces.

---

## 1. THE HUMAN - INTRODUCTION

The human is the central component in HCI. Key areas:
- **Information I/O**: visual, auditory, haptic, movement
- **Information stored in memory**: sensory, short-term, long-term
- **Information processed and applied**: reasoning, problem solving, skill, error
- **Emotion** influences human capabilities
- **Each person is different** (individual differences)

---

## 2. VISION

### Two Stages in Vision
1. Physical reception of stimulus
2. Processing and interpretation of stimulus

### The Eye - Physical Reception
- Mechanism for receiving light and transforming it into electrical energy
- Light reflects from objects
- Images are focused **upside-down** on retina
- Retina contains:
  - **Rods** – low light vision
  - **Cones** – colour vision
- **Ganglion cells** (in the brain!) detect pattern and movement

### Interpreting the Signal

#### Size and Depth
- **Visual angle** indicates how much of view object occupies (relates to size and distance from eye)
- **Visual acuity** is ability to perceive detail (limited)
- Familiar objects perceived as constant size (in spite of changes in visual angle when far away)
- Cues like overlapping help perception of size and depth

#### Brightness
- Subjective reaction to levels of light
- Affected by luminance of object
- Measured by **just noticeable difference**
- Visual acuity increases with luminance as does flicker

#### Colour
- Made up of **hue, intensity, saturation**
- Cones sensitive to colour wavelengths
- **Blue acuity is lowest**
- 8% males and 1% females are colour blind

### Visual Compensation
- The visual system compensates for movement and changes in luminance
- Context is used to resolve ambiguity
- **Optical illusions** sometimes occur due to over compensation

### Optical Illusions
- **Ponzo illusion** – two horizontal bars of equal length on converging lines (railroad tracks), making upper bar appear longer
- **Muller Lyer illusion** – two lines of equal length with different arrowhead configurations, making them appear different lengths

---

## 3. READING

Several stages:
1. Visual pattern perceived
2. Decoded using internal representation of language
3. Interpreted using knowledge of syntax, semantics, pragmatics

Key facts:
- Reading involves **saccades** (eye movements) and **fixations** (pauses)
- Perception occurs during fixations
- **Word shape** is important to recognition
- **Negative contrast** improves reading from computer screen

---

## 4. HEARING

### Purpose
Provides information about environment: distances, directions, objects etc.

### Physical Apparatus
- **Outer ear** – protects inner and amplifies sound
- **Middle ear** – transmits sound waves as vibrations to inner ear
- **Inner ear** – chemical transmitters are released and cause impulses in auditory nerve

### Sound Properties
- **Pitch** – sound frequency
- **Loudness** – amplitude
- **Timbre** – type or quality

### Key Facts
- Humans can hear frequencies from **20Hz to 15kHz**
- Less accurate distinguishing high frequencies than low
- **Auditory system filters sounds** – can attend to sounds over background noise
- **Cocktail party phenomenon** – ability to focus on one voice in noisy environment

---

## 5. TOUCH

### Purpose
Provides important feedback about environment. May be key sense for someone who is visually impaired.

### Receptors in Skin
- **Thermoreceptors** – heat and cold
- **Nociceptors** – pain
- **Mechanoreceptors** – pressure (some instant, some continuous)

### Key Facts
- Some areas more sensitive than others (e.g. fingers)
- **Kinesthesia** – awareness of body position, affects comfort and performance

---

## 6. MOVEMENT

### Response Time
Time taken to respond to stimulus = **reaction time + movement time**

Movement time dependent on age, fitness etc.

### Reaction Time by Stimulus Type
- **Visual** ~ 200ms
- **Auditory** ~ 150ms
- **Pain** ~ 700ms

Increasing reaction time decreases accuracy in the **unskilled operator** but not in the **skilled operator**.

### Fitts' Law
Describes the time taken to hit a screen target:

**Mt = a + b log₂(D/S + 1)**

Where:
- a and b = empirically determined constants
- Mt = movement time
- D = Distance to target
- S = Size of target

**Design Implications:**
- Targets as **large** as possible
- Distances as **small** as possible

---

## 7. MEMORY

### Three Types of Memory Function

**Sensory memories** → (Attention) → **Short-term memory/Working memory** → (Rehearsal) → **Long-term memory**

Selection of stimuli governed by level of arousal.

### Sensory Memory
- Buffers for stimuli received through senses
  - **Iconic memory** – visual stimuli
  - **Echoic memory** – aural stimuli
  - **Haptic memory** – tactile stimuli
- Examples: "sparkler" trail, stereo sound
- **Continuously overwritten**

### Short-Term Memory (STM)
- Scratch-pad for temporary recall
- **Rapid access** ~ 70ms
- **Rapid decay** ~ 200ms
- **Limited capacity** – **7 ± 2 chunks**

#### Chunking Example
- 212348278493202 → hard to remember
- 0121 414 2626 → easier (chunked)
- HEC ATR ANU PTH ETR EET → easiest (meaningful chunks)

### Long-Term Memory (LTM)
- Repository for all our knowledge
- **Slow access** ~ 1/10 second
- **Slow decay**, if any
- **Huge or unlimited capacity**

#### Two Types
1. **Episodic** – serial memory of events
2. **Semantic** – structured memory of facts, concepts, skills
   - Semantic LTM derived from episodic LTM

### Semantic Memory Structure
- Provides access to information
- Represents relationships between bits of information
- Supports inference

### Semantic Network Model
- **Inheritance** – child nodes inherit properties of parent nodes
- Relationships between bits of information explicit
- Supports inference through inheritance

Example: ANIMAL → DOG → COLLIE → LASSIE
- DOG inherits: breathes, moves from ANIMAL
- COLLIE inherits: barks, four legs, tail from DOG
- LASSIE is an instance of COLLIE

### Frames Model
- Information organized in data structures
- **Slots** in structure instantiated with values for instance of data
- Type-subtype relationships

Example DOG frame:
- Fixed: legs = 4
- Default: diet = carnivorous, sound = bark
- Variable: size, colour

### Scripts Model
- Model of stereotypical information required to interpret situation
- Script has elements that can be instantiated with values for context

Example: Visit to the vet
- Entry conditions: dog ill, vet open, owner has money
- Result: dog better, owner poorer, vet richer
- Props: examination table, medicine, instruments
- Roles: vet examines, diagnoses, treats; owner brings dog in, pays
- Scenes: arriving at reception, waiting, examination, paying
- Tracks: dog needs medicine, dog needs operation

### Production Rules Model
- Representation of procedural knowledge
- **Condition/action rules**: if condition is matched, then use rule to determine action

Example:
- IF dog is wagging tail THEN pat dog
- IF dog is growling THEN run away

### LTM - Storage
- **Rehearsal** – information moves from STM to LTM
- **Total time hypothesis** – amount retained proportional to rehearsal time
- **Distribution of practice effect** – optimized by spreading learning over time
- **Structure, meaning and familiarity** – information easier to remember

### LTM - Forgetting
- **Decay** – information is lost gradually but very slowly
- **Interference**:
  - New information replaces old: **retroactive interference**
  - Old may interfere with new: **proactive inhibition**
- May not forget at all – memory is selective, affected by emotion

### LTM - Retrieval
- **Recall** – information reproduced from memory, can be assisted by cues (categories, imagery)
- **Recognition** – information gives knowledge that it has been seen before, less complex than recall

---

## 8. THINKING

### Reasoning
Three types:
1. **Deduction** – derive logically necessary conclusion from given premises
   - Example: If it is Friday then she will go to work. It is Friday. Therefore she will go to work.
   - **Important**: Logical conclusion not necessarily true!
   - Example: If it is raining then the ground is dry. It is raining. Therefore the ground is dry. (Logically valid but factually wrong)
   - When truth and logical validity clash, people bring world knowledge to bear

2. **Induction** – generalize from cases seen to cases unseen
   - Example: All elephants we have seen have trunks therefore all elephants have trunks
   - **Unreliable**: can only prove false not true
   - **But useful!**
   - Humans not good at using negative evidence (e.g. Wason's cards)

3. **Abduction** – reasoning from event to cause
   - Example: Sam drives fast when drunk. If I see Sam driving fast, assume drunk.
   - **Unreliable**: can lead to false explanations

### Wason's Cards
- Four cards showing: 7, E, 4, K
- Rule: "If a card has a vowel on one side it has an even number on the other"
- Need to turn over E (vowel → check even) and 7 (odd → check consonant)
- People often get this wrong – not good at using negative evidence

### Problem Solving
Process of finding solution to unfamiliar task using knowledge.

#### Gestalt Theory
- Problem solving both productive and reproductive
- Productive draws on insight and restructuring of problem
- Attractive but not enough evidence to explain 'insight'
- Move away from behaviourism towards information processing theories

#### Problem Space Theory
- Problem space comprises problem states
- Problem solving involves generating states using legal operators
- **Heuristics** may be employed to select operators (e.g. means-ends analysis)
- Operates within human information processing system (e.g. STM limits)
- Largely applied to well-defined areas (puzzles rather than knowledge intensive areas)

#### Analogy
- Analogical mapping: use knowledge of similar problem from similar domain
- Difficult if domains are semantically different

#### Skill Acquisition
- Skilled activity characterized by **chunking**
- Conceptual rather than superficial grouping of problems
- Information is structured more effectively

---

## 9. ERRORS AND MENTAL MODELS

### Types of Error

#### Slips
- Right intention, but failed to do it right
- Causes: poor physical skill, inattention etc.
- Change to aspect of skilled behaviour can cause slip
- **Fix**: Better interface design

#### Mistakes
- Wrong intention
- Cause: incorrect understanding
- Humans create mental models to explain behaviour
- If wrong (different from actual system) errors can occur
- **Fix**: Better understanding of system

---

## 10. EMOTION

### Theories of Emotion
- **James-Lange**: emotion is our interpretation of a physiological response to a stimuli
- **Cannon**: emotion is a psychological response to a stimuli
- **Schacter-Singer**: emotion is the result of our evaluation of our physiological responses, in the light of the whole situation we are in

Emotion clearly involves both cognitive and physical responses to stimuli.

### Affect
- The biological response to physical stimuli is called **affect**
- Affect influences how we respond to situations:
  - **Positive** → creative problem solving
  - **Negative** → narrow thinking
- "Negative affect can make it harder to do even easy tasks; positive affect can make it easier to do difficult tasks" (Donald Norman)

### Implications for Interface Design
- Stress will increase the difficulty of problem solving
- Relaxed users will be more forgiving of shortcomings in design
- **Aesthetically pleasing and rewarding interfaces will increase positive affect**

---

## 11. INDIVIDUAL DIFFERENCES

### Types
- **Long term**: sex, physical and intellectual abilities
- **Short term**: effect of stress or fatigue
- **Changing**: age

### Design Question
- Will design decision exclude section of user population?

---

## 12. PSYCHOLOGY AND DESIGN OF INTERACTIVE SYSTEMS

### Direct Applications
- Blue acuity is poor → blue should not be used for important detail

### Key Insight
Correct application generally requires understanding of context in psychology, and an understanding of particular experimental conditions.

Much knowledge has been distilled in:
- Guidelines (Chapter 7)
- Cognitive models (Chapter 12)
- Experimental and analytic evaluation techniques (Chapter 9)

---

## KEY CONCEPTS FOR EXAM
1. **Vision**: Two stages (reception + interpretation), rods (low light) vs cones (colour), images focused upside-down, visual angle, visual acuity
2. **Colour**: hue/intensity/saturation, blue acuity lowest, 8% males/1% females colour blind
3. **Reading**: saccades + fixations, perception during fixations, word shape important, negative contrast better for screens
4. **Hearing**: 20Hz-15kHz, cocktail party phenomenon, pitch/loudness/timbre
5. **Touch**: thermoreceptors (heat/cold), nociceptors (pain), mechanoreceptors (pressure), kinesthesia (body position)
6. **Fitts' Law**: Mt = a + b log₂(D/S + 1) – targets large, distances small
7. **STM**: 7±2 chunks, rapid decay (~200ms), rapid access (~70ms)
8. **LTM**: episodic (events) vs semantic (facts), unlimited capacity, slow access (~100ms)
9. **Semantic networks**: inheritance, supports inference
10. **Frames**: slots with fixed/default/variable values
11. **Scripts**: stereotypical situations with entry conditions, props, roles, scenes, tracks
12. **Production rules**: IF condition THEN action
13. **Deduction**: logically necessary conclusion (not necessarily true)
14. **Induction**: generalize from seen to unseen (unreliable but useful)
15. **Abduction**: reasoning from event to cause (unreliable)
16. **Wason's cards**: poor at using negative evidence
17. **Problem space theory**: states, operators, heuristics (means-ends analysis)
18. **Slips**: right intention, wrong action (fix: interface design)
19. **Mistakes**: wrong intention (fix: understanding)
20. **Emotion**: positive affect → creative problem solving; negative → narrow thinking
21. **Affect**: aesthetically pleasing interfaces increase positive affect
22. **Individual differences**: long-term (sex, abilities), short-term (stress, fatigue), changing (age)
