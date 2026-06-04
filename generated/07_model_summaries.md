# Comprehensive Models & Architectures Summary
## HCI Course — Chapters 1-9

---

## Table of Contents
1. [Norman's Execution/Evaluation Loop](#1-normans-executionevaluation-loop-ch3)
2. [Abowd & Beale Framework](#2-abowd--beale-framework-ch3)
3. [Semantic Network Model](#3-semantic-network-model-ch1)
4. [Frames Model](#4-frames-model-ch1)
5. [Scripts Model](#5-scripts-model-ch1)
6. [Production Rules](#6-production-rules-ch1)
7. [Waterfall Model](#7-waterfall-model-ch6)
8. [Iterative Design Model](#8-iterative-design-model-ch6)
9. [Seeheim Model](#9-seeheim-model-ch8)
10. [Arch/Slinky Model](#10-archslinky-model-ch8)
11. [MVC Model](#11-mvc-model-ch8)
12. [PAC Model](#12-pac-model-ch8)
13. [IBIS Model](#13-ibis-model-ch6)
14. [QOC Model](#14-qoc-model-ch6)
15. [Client-Server Architecture](#15-client-server-architecture-ch8)
16. [X Windows Architecture](#16-x-windows-architecture-ch8)
17. [GOMS Model](#17-goms-model-ch9)
18. [Keystroke-Level Model (KLM)](#18-keystroke-level-model--klm-ch9)
19. [Nielsen's Severity Rating Scale](#19-nielsens-severity-rating-scale-ch9)
20. [8-Factor Evaluation Method Selection](#20-8-factor-evaluation-method-selection-ch9)

---

## 1. Norman's Execution/Evaluation Loop (Ch3)

### Overview
Don Norman's model describes how users interact with systems through a cyclical process of executing actions and evaluating results.

### The 7 Stages

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                    EXECUTION                EVALUATION          │
    │                                                                 │
    │  ┌─────────────┐                    ┌─────────────┐           │
    │  │ 1. FORM     │                    │ 7. COMPARE  │           │
    │  │ GOAL        │                    │ OUTCOME TO  │           │
    │  │             │                    │ GOAL        │           │
    │  └──────┬──────┘                    └──────▲──────┘           │
    │         │                                  │                   │
    │         ▼                                  │                   │
    │  ┌─────────────┐                    ┌─────────────┐           │
    │  │ 2. FORM     │                    │ 6. PERCEIVE │           │
    │  │ INTENTION   │                    │ STATE OF    │           │
    │  │             │                    │ WORLD       │           │
    │  └──────┬──────┘                    └──────▲──────┘           │
    │         │                                  │                   │
    │         ▼                                  │                   │
    │  ┌─────────────┐                    ┌─────────────┐           │
    │  │ 3. SPECIFY  │                    │ 5. EVALUATE │           │
    │  │ ACTION      │────────────────────▶│ OUTCOME     │           │
    │  │ SEQUENCE    │   (GULF OF          │             │           │
    │  │             │    EXECUTION)       │             │           │
    │  └──────┬──────┘                    └──────▲──────┘           │
    │         │                                  │                   │
    │         ▼                                  │                   │
    │  ┌─────────────┐                    ┌─────────────┐           │
    │  │ 4. PERFORM  │                    │ (GULF OF    │           │
    │  │ ACTION      │────────────────────▶│ EVALUATION) │           │
    │  │             │                    │             │           │
    │  └─────────────┘                    └─────────────┘           │
    │                                                                 │
    │              ┌────────────────────────────────────┐           │
    │              │        WORLD                       │           │
    │              │  ┌──────────────────────────────┐  │           │
    │              │  │    SYSTEM STATE               │  │           │
    │              │  └──────────────────────────────┘  │           │
    │              └────────────────────────────────────┘           │
    └─────────────────────────────────────────────────────────────────┘
```

### Key Concepts

| Concept | Description |
|---------|-------------|
| **Gulf of Execution** | Gap between user's intention and system's execution capability |
| **Gulf of Evaluation** | Gap between system's actual state and user's understanding |
| **Circular Flow** | Process is iterative; evaluation feeds back to new goals |
| **7 Stages** | Form goal → Form intention → Specify action → Perform action → Evaluate outcome → Perceive state → Compare to goal |

### Gulfs Explained

**Gulf of Execution** (User → System):
- Does the system support what the user wants to do?
- Are controls accessible and understandable?
- Is the mapping between intention and action clear?

**Gulf of Evaluation** (System → User):
- Can the user see what happened?
- Is feedback immediate and clear?
- Is the system state perceivable?

### 7 Stages Detail

1. **Form Goal** — User wants to achieve something (e.g., send an email)
2. **Form Intention** — User forms a specific plan (e.g., click "Send" button)
3. **Specify Action Sequence** — User determines steps (e.g., click button, wait)
4. **Perform Action** — User executes the physical action (e.g., mouse click)
5. **Evaluate Outcome** — User assesses what happened (e.g., "Did it send?")
6. **Perceive State** — User observes system state (e.g., "Message sent" notification)
7. **Compare to Goal** — User compares result to original goal (e.g., "Email sent successfully")

### Exam Tips
- **Common question**: "Explain the gulfs of execution and evaluation"
- **Key insight**: Good design minimizes both gulfs
- **Application**: Use this model to analyze usability problems
- **Remember**: The loop is circular — evaluation leads to new goals

---

## 2. Abowd & Beale Framework (Ch3)

### Overview
Framework for analyzing human-computer interaction through four languages and translation processes between them.

### The Framework

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                     FOUR LANGUAGES                            │
    │                                                                 │
    │   ┌──────────────┐         ┌──────────────┐                   │
    │   │   USER'S     │         │   USER'S     │                   │
    │   │   LANGUAGE    │         │   LANGUAGE    │                   │
    │   │   (UL)        │         │   (UL)        │                   │
    │   └──────┬───────┘         └──────▲───────┘                   │
    │          │                         │                            │
    │          ▼                         │                            │
    │   ┌──────────────┐         ┌──────────────┐                   │
    │   │  SEMANTIC    │         │  SEMANTIC    │                   │
    │   │  LANGUAGE    │         │  LANGUAGE    │                   │
    │   │  (SL)        │         │  (SL)        │                   │
    │   └──────┬───────┘         └──────▲───────┘                   │
    │          │                         │                            │
    │          ▼                         │                            │
    │   ┌──────────────┐         ┌──────────────┐                   │
    │   │  SYNTACTIC   │         │  SYNTACTIC   │                   │
    │   │  LANGUAGE    │         │  LANGUAGE    │                   │
    │   │  (SynL)      │         │  (SynL)      │                   │
    │   └──────┬───────┘         └──────▲───────┘                   │
    │          │                         │                            │
    │          ▼                         │                            │
    │   ┌──────────────┐         ┌──────────────┐                   │
    │   │  DEVICE      │         │  DEVICE      │                   │
    │   │  LANGUAGE    │         │  LANGUAGE    │                   │
    │   │  (DL)        │         │  (DL)        │                   │
    │   └──────────────┘         └──────────────┘                   │
    │                                                                 │
    │          │                         ▲                            │
    │          ▼                         │                            │
    │   ┌──────────────────────────────────────┐                    │
    │   │           USER                        │                    │
    │   └──────────────────────────────────────┘                    │
    │   ┌──────────────────────────────────────┐                    │
    │   │           COMPUTER                    │                    │
    │   └──────────────────────────────────────┘                    │
    └─────────────────────────────────────────────────────────────────┘
```

### Four Languages

| Language | Level | Description | Example |
|----------|-------|-------------|---------|
| **User Language (UL)** | Highest | User's conceptual model and goals | "I want to send an email" |
| **Semantic Language (SL)** | High | System's semantic representation | "compose_email(to, subject, body)" |
| **Syntactic Language (SynL)** | Low | Input/output syntax and grammar | "click button, type text" |
| **Device Language (DL)** | Lowest | Physical device signals | "key press, mouse coordinates" |

### Translation Processes

| Translation | Direction | Process |
|-------------|-----------|---------|
| **UL → SL** | User to System | Mapping user goals to system capabilities |
| **SL → SynL** | Semantic to Syntactic | Mapping operations to input/output syntax |
| **SynL → DL** | Syntactic to Device | Mapping syntax to physical device actions |
| **DL → SynL** | Device to Syntactic | Interpreting device signals as syntax |
| **SynL → SL** | Syntactic to Semantic | Interpreting syntax as semantic operations |
| **SL → UL** | System to User | Mapping system response to user understanding |

### Key Features
- **Bidirectional**: Translation happens both ways (user→system and system→user)
- **Multiple Mappings**: One UL can map to multiple SLs; one SL can have multiple SynLs
- **Design Implications**: Poor translations cause usability problems

### Design Implications
- **UL → SL**: System must support user's conceptual model
- **SL → SynL**: Interface must provide clear syntax for operations
- **SynL → DL**: Input devices must support required syntax
- **DL → SynL**: Output must be perceivable and interpretable

### Exam Tips
- **Common question**: "Explain the four languages and their relationships"
- **Key insight**: Design problems occur at translation boundaries
- **Application**: Use to analyze where breakdowns occur in interaction
- **Remember**: Each translation can introduce errors or confusion

---

## 3. Semantic Network Model (Ch1)

### Overview
Knowledge representation using nodes (concepts) and edges (relationships). Used to model how people organize and retrieve knowledge.

### Structure

```
                         ┌─────────────┐
                         │   ANIMAL    │
                         └──────┬──────┘
                                │
              ┌─────────────────┼─────────────────┐
              │                 │                 │
              ▼                 ▼                 ▼
       ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
       │   MAMMAL    │  │   BIRD      │  │   REPTILE   │
       └──────┬──────┘  └──────┬──────┘  └──────┬──────┘
              │                │                │
      ┌───────┼───────┐       │                │
      │       │       │       │                │
      ▼       ▼       ▼       ▼                ▼
┌─────────┐ ┌─────────┐ ┌─────────┐      ┌─────────┐
│  DOG    │ │  CAT    │ │ EAGLE   │      │ SNAKE   │
└─────────┘ └─────────┘ └─────────┘      └─────────┘
    │           │           │                │
    ▼           ▼           ▼                ▼
┌─────────┐ ┌─────────┐ ┌─────────┐      ┌─────────┐
│ BARKS   │ │ MEOWS   │ │ FLIES   │      │ CRAWLS  │
│ (prop)  │ │ (prop)  │ │ (prop)  │      │ (prop)  │
└─────────┘ └─────────┘ └─────────┘      └─────────┘
```

### Key Components

| Component | Description | Example |
|-----------|-------------|---------|
| **Nodes** | Concepts or entities | ANIMAL, DOG, BARKS |
| **Edges** | Relationships between nodes | IS-A, HAS-A, CAN |
| **Inheritance** | Properties inherited from parent nodes | DOG inherits from MAMMAL |
| **Instances** | Specific examples of concepts | "Rex" is instance of DOG |

### Relationship Types

| Relationship | Meaning | Example |
|--------------|---------|---------|
| **IS-A** | Class inheritance | DOG IS-A MAMMAL |
| **HAS-A** | Part-whole | DOG HAS-A TAIL |
| **CAN** | Capability | DOG CAN BARK |
| **PART-OF** | Component relationship | TAIL PART-OF DOG |

### Properties

| Property | Description |
|-----------|-------------|
| **Inheritance** | Child nodes inherit properties from parent nodes |
| **Default Values** | Assumed properties unless overridden |
| **Multiple Inheritance** | Node can inherit from multiple parents |
| **Spreading Activation** | Activation of one node activates related nodes |

### Applications in HCI
- **Menu Design**: Hierarchical menu structures
- **Information Architecture**: Website organization
- **User Modeling**: Representing user knowledge
- **Hypertext**: Linking related concepts

### Exam Tips
- **Common question**: "How do semantic networks represent knowledge?"
- **Key insight**: Inheritance allows efficient knowledge storage
- **Application**: Use to design menu hierarchies and navigation
- **Remember**: Multiple inheritance can create ambiguity

---

## 4. Frames Model (Ch1)

### Overview
Knowledge representation using structured templates (frames) with slots that hold specific information about concepts.

### Structure

```
┌─────────────────────────────────────────────────────────────────┐
│                        FRAME: RESTAURANT                        │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  SLOT: Type          │ DEFAULT: "restaurant"            │   │
│  ├──────────────────────┼──────────────────────────────────┤   │
│  │  SLOT: Location      │ VARIABLE: [specific location]   │   │
│  ├──────────────────────┼──────────────────────────────────┤   │
│  │  SLOT: Food Type     │ DEFAULT: "varies"                │   │
│  ├──────────────────────┼──────────────────────────────────┤   │
│  │  SLOT: Price Range   │ FIXED: "$-$$"                    │   │
│  ├──────────────────────┼──────────────────────────────────┤   │
│  │  SLOT: Hours         │ DEFAULT: "11am-10pm"             │   │
│  ├──────────────────────┼──────────────────────────────────┤   │
│  │  SLOT: Payment       │ FIXED: "cash, credit"            │   │
│  └──────────────────────┴──────────────────────────────────┘   │
│                                                                 │
│  INHERITANCE: Is-a → BUSINESS                                  │
└─────────────────────────────────────────────────────────────────┘
```

### Slot Types

| Slot Type | Description | Example |
|-----------|-------------|---------|
| **Fixed** | Always has the same value | Payment: "cash, credit" |
| **Default** | Has typical value, can be overridden | Hours: "11am-10pm" |
| **Variable** | Value depends on instance | Location: [specific] |

### Frame Structure

```
FRAME NAME: RESTAURANT
├── Slots
│   ├── Type: fixed = "restaurant"
│   ├── Location: variable = [specific location]
│   ├── Food Type: default = "varies"
│   ├── Price Range: fixed = "$-$$"
│   ├── Hours: default = "11am-10pm"
│   └── Payment: fixed = "cash, credit"
├── Inheritance
│   └── Is-a: BUSINESS
└── Constraints
    └── Must have: MENU, SEATING, KITCHEN
```

### Key Concepts

| Concept | Description |
|---------|-------------|
| **Slots** | Attributes or properties of the frame |
| **Fillers** | Values that occupy slots |
| **Inheritance** | Frames inherit from parent frames |
| **Defaults** | Typical values that can be overridden |
| **Constraints** | Restrictions on slot values |
| **Procedures** | Attached procedures that execute when slot is accessed |

### Applications in HCI
- **Dialog Design**: Conversation scripts
- **Menu Design**: Hierarchical menu structures
- **Form Design**: Data entry templates
- **Object-Oriented Design**: Class hierarchies

### Exam Tips
- **Common question**: "Explain the three types of slots in frames"
- **Key insight**: Defaults make frames flexible yet predictable
- **Application**: Use to design consistent interface elements
- **Remember**: Frames can have attached procedures (demons)

---

## 5. Scripts Model (Ch1)

### Overview
Structured representation of stereotypical sequences of events in a particular context. Based on frames but focuses on event sequences.

### Structure

```
┌─────────────────────────────────────────────────────────────────┐
│                      SCRIPT: RESTAURANT                         │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ENTRY CONDITIONS:                                              │
│  ├── Customer is hungry                                         │
│  ├── Customer has money                                         │
│  └── Restaurant is open                                         │
│                                                                 │
│  PROPS:                                                         │
│  ├── Tables, chairs                                            │
│  ├── Menus                                                      │
│  ├── Tableware                                                  │
│  └── Food                                                       │
│                                                                 │
│  ROLES:                                                         │
│  ├── Customer                                                   │
│  ├── Waiter                                                     │
│  └── Cook                                                       │
│                                                                 │
│  SCENES:                                                        │
│  ├── 1. Entry                                                   │
│  │   └── Customer enters, waits for host                       │
│  ├── 2. Seating                                                 │
│  │   └── Host seats customer, gives menu                       │
│  ├── 3. Ordering                                                │
│  │   └── Customer reads menu, waiter takes order               │
│  ├── 4. Eating                                                  │
│  │   └── Food is served, customer eats                         │
│  └── 5. Exit                                                    │
│      └── Customer pays, leaves                                 │
│                                                                 │
│  TRACKS:                                                        │
│  ├── Happy path (normal sequence)                              │
│  ├── Problem path (wrong order, slow service)                  │
│  └── Special path (dietary restrictions)                       │
└─────────────────────────────────────────────────────────────────┘
```

### Components

| Component | Description | Example |
|-----------|-------------|---------|
| **Entry Conditions** | Prerequisites for script execution | Hungry, has money, restaurant open |
| **Props** | Physical objects involved | Tables, menus, food |
| **Roles** | Actors in the script | Customer, waiter, cook |
| **Scenes** | Sequences of events | Entry, ordering, eating |
| **Tracks** | Variations of the script | Happy path, problem path |

### Scene Flow

```
┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐
│  ENTRY  │───▶│ SEATING │───▶│ ORDERING│───▶│ EATING  │───▶│  EXIT   │
└─────────┘    └─────────┘    └─────────┘    └─────────┘    └─────────┘
     │              │              │              │              │
     ▼              ▼              ▼              ▼              ▼
┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐    ┌─────────┐
│ Enter   │    │ Host    │    │ Read    │    │ Food    │    │ Pay     │
│ Wait    │    │ Seat    │    │ Menu    │    │ Served  │    │ Leave   │
│ Look    │    │ Give    │    │ Order   │    │ Eat     │    │         │
│ around  │    │ Menu    │    │ Wait    │    │ Enjoy   │    │         │
└─────────┘    └─────────┘    └─────────┘    └─────────┘    └─────────┘
```

### Applications in HCI
- **Dialog Systems**: Conversation flow design
- **Wizard Interfaces**: Guided task completion
- **Training Systems**: Step-by-step procedures
- **User Manuals**: Task documentation

### Exam Tips
- **Common question**: "How do scripts differ from frames?"
- **Key insight**: Scripts focus on event sequences, frames on static knowledge
- **Application**: Use to design predictable user interactions
- **Remember**: Tracks allow for variations and error handling

---

## 6. Production Rules (Ch1)

### Overview
IF-THEN rules that specify conditions and actions. Used to model user knowledge, system behavior, and interface logic.

### Structure

```
┌─────────────────────────────────────────────────────────────────┐
│                    PRODUCTION RULE SYSTEM                       │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  RULE 1:                                                        │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  IF user clicks "Save" button                           │   │
│  │  THEN save current document                             │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  RULE 2:                                                        │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  IF document is modified                                │   │
│  │  THEN enable "Save" button                              │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  RULE 3:                                                        │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  IF user selects text                                   │   │
│  │  THEN show formatting options                           │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  KNOWLEDGE BASE:                                                │
│  ├── Current state: document modified                          │
│  ├── User action: clicked "Save"                               │
│  └── System state: save in progress                            │
│                                                                 │
│  CONFlict RESOLUTION:                                           │
│  ├── Priority ordering                                         │
│  ├── Recency                                                   │
│  └── Specificity                                               │
└─────────────────────────────────────────────────────────────────┘
```

### Rule Structure

| Component | Description | Example |
|-----------|-------------|---------|
| **Condition** | IF part - specifies when rule applies | "IF user clicks 'Save'" |
| **Action** | THEN part - specifies what to do | "THEN save document" |
| **Knowledge Base** | Current facts and state | Document modified, user clicked Save |
| **Conflict Resolution** | How to choose between competing rules | Priority, recency, specificity |

### Rule Types

| Type | Description | Example |
|------|-------------|---------|
| **Context-Free** | No conditions on context | Always show menu bar |
| **Context-Sensitive** | Conditions depend on context | Show save option if modified |
| **Complex** | Multiple conditions | IF modified AND has permission THEN enable save |

### Conflict Resolution Strategies

| Strategy | Description |
|----------|-------------|
| **Priority** | Higher priority rules fire first |
| **Recency** | More recently activated rules take precedence |
| **Specificity** | More specific rules override general ones |
| **Random** | Random selection among conflicting rules |

### Applications in HCI
- **Menu Enabling/Disabling**: Context-sensitive menu items
- **Dialog Systems**: Response generation
- **Expert Systems**: Knowledge-based interfaces
- **User Modeling**: Predicting user behavior

### Exam Tips
- **Common question**: "How do production rules model user knowledge?"
- **Key insight**: Rules capture procedural knowledge (how to do things)
- **Application**: Use to design context-sensitive interfaces
- **Remember**: Conflict resolution is important when multiple rules match

---

## 7. Waterfall Model (Ch6)

### Overview
Linear sequential software development process where each phase must be completed before the next begins.

### Structure

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                      WATERFALL MODEL                            │
    │                                                                 │
    │  ┌─────────────┐                                               │
    │  │ REQUIREMENTS│                                               │
    │  │ ANALYSIS    │                                               │
    │  └──────┬──────┘                                               │
    │         │                                                       │
    │         ▼                                                       │
    │  ┌─────────────┐                                               │
    │  │  SYSTEM     │                                               │
    │  │  DESIGN     │                                               │
    │  └──────┬──────┘                                               │
    │         │                                                       │
    │         ▼                                                       │
    │  ┌─────────────┐                                               │
    │  │ IMPLEMENTA- │                                               │
    │  │ TION        │                                               │
    │  └──────┬──────┘                                               │
    │         │                                                       │
    │         ▼                                                       │
    │  ┌─────────────┐                                               │
    │  │ TESTING     │                                               │
    │  └──────┬──────┘                                               │
    │         │                                                       │
    │         ▼                                                       │
    │  ┌─────────────┐                                               │
    │  │ DEPLOYMENT  │                                               │
    │  └──────┬──────┘                                               │
    │         │                                                       │
    │         ▼                                                       │
    │  ┌─────────────┐                                               │
    │  │MAINTENANCE  │                                               │
    │  └─────────────┘                                               │
    │                                                                 │
    │  ─────────────────────────────────────────────────────────     │
    │  Time ─────────────────────────────────────────────────▶      │
    └─────────────────────────────────────────────────────────────────┘
```

### Phases

| Phase | Activities | Deliverables |
|-------|------------|--------------|
| **Requirements Analysis** | Gather and document requirements | Requirements document |
| **System Design** | Architectural and detailed design | Design specifications |
| **Implementation** | Code development | Source code |
| **Testing** | Verification and validation | Test reports |
| **Deployment** | Installation and rollout | Working system |
| **Maintenance** | Bug fixes and updates | Updated system |

### Problems for Interactive Systems

| Problem | Description |
|---------|-------------|
| **Late User Involvement** | Users don't see system until late stages |
| **No Feedback Loops** | Can't go back to fix problems easily |
| **Assumes Complete Requirements** | Requirements can be fully known upfront |
| **No Prototyping** | No early validation of design decisions |
| **Rigid Process** | Can't adapt to changing requirements |

### Variants

| Variant | Description |
|---------|-------------|
| **V-Model** | Adds verification and validation at each phase |
| **Incremental Waterfall** | Breaks project into smaller waterfalls |
| **Document-Driven** | Emphasizes documentation at each phase |

### Exam Tips
- **Common question**: "Why is Waterfall problematic for HCI?"
- **Key insight**: HCI requires user feedback; Waterfall doesn't provide it
- **Application**: Compare with iterative models
- **Remember**: Waterfall works better for stable, well-understood requirements

---

## 8. Iterative Design Model (Ch6)

### Overview
Design process that repeats cycles of design, implementation, and evaluation, incorporating user feedback at each iteration.

### Structure

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                    ITERATIVE DESIGN MODEL                       │
    │                                                                 │
    │                    ┌─────────────┐                              │
    │         ┌─────────│   DESIGN    │─────────┐                    │
    │         │         └─────────────┘         │                    │
    │         │                                 │                    │
    │         ▼                                 │                    │
    │  ┌─────────────┐                   ┌─────────────┐            │
    │  │  ANALYZE    │                   │  EVALUATE   │            │
    │  │  USERS &    │◀──────────────────│  WITH USERS │            │
    │  │  TASKS      │                   │             │            │
    │  └──────┬──────┘                   └──────▲──────┘            │
    │         │                                 │                    │
    │         ▼                                 │                    │
    │  ┌─────────────┐                   ┌─────────────┐            │
    │  │  PROTOTYPE  │──────────────────▶│ IMPLEMENT   │            │
    │  │             │                   │             │            │
    │  └─────────────┘                   └─────────────┘            │
    │                                                                 │
    │  ITERATION 1: Low-fidelity prototype                          │
    │  ITERATION 2: Medium-fidelity prototype                       │
    │  ITERATION 3: High-fidelity prototype                         │
    │  ITERATION 4: Final system                                    │
    │                                                                 │
    │  ─────────────────────────────────────────────────────────     │
    │  Time ─────────────────────────────────────────────────▶      │
    └─────────────────────────────────────────────────────────────────┘
```

### Key Activities

| Activity | Description | Methods |
|----------|-------------|---------|
| **Analyze** | Understand users and tasks | Task analysis, user interviews |
| **Design** | Create interface solutions | Sketches, mockups |
| **Prototype** | Build testable versions | Paper, Wizard of Oz, coded |
| **Evaluate** | Test with users | Usability testing, heuristic evaluation |
| **Implement** | Build production system | Software development |

### Prototype Fidelity Levels

| Fidelity | Description | Tools |
|----------|-------------|-------|
| **Low** | Paper sketches, basic mockups | Paper, cardboard, sticky notes |
| **Medium** | Interactive but limited functionality | PowerPoint, Keynote, Balsamiq |
| **High** | Nearly functional, interactive | HTML/CSS, coded prototypes |
| **Production** | Fully functional system | Full development |

### Feedback Loops

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                    FEEDBACK LOOPS                               │
    │                                                                 │
    │  DESIGN ──▶ PROTOTYPE ──▶ EVALUATE ──▶ ANALYZE ──▶ DESIGN     │
    │     ▲                                              │           │
    │     │                                              │           │
    │     └──────────────────────────────────────────────┘           │
    │                                                                 │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │  LOOP 1: Can users understand the interface?            │   │
    │  │  LOOP 2: Can users complete tasks efficiently?          │   │
    │  │  LOOP 3: Is the interface satisfying to use?            │   │
    │  │  LOOP 4: Does the system meet all requirements?         │   │
    │  └─────────────────────────────────────────────────────────┘   │
    └─────────────────────────────────────────────────────────────────┘
```

### Advantages Over Waterfall

| Advantage | Description |
|-----------|-------------|
| **Early User Feedback** | Users involved from the beginning |
| **Risk Reduction** | Problems found early when cheaper to fix |
| **Flexibility** | Can adapt to changing requirements |
| **Validation** | Design decisions validated with users |
| **Learning** | Team learns from each iteration |

### Exam Tips
- **Common question**: "Compare iterative design with Waterfall"
- **Key insight**: Iterative design embraces change; Waterfall resists it
- **Application**: Use iterative design for HCI projects
- **Remember**: Each iteration should be testable with users

---

## 9. Seeheim Model (Ch8)

### Overview
Layered architectural model for interactive systems with three main components and a control mechanism.

### Structure

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                      SEEHEIM MODEL                              │
    │                                                                 │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                  PRESENTATION                            │   │
    │  │          (Input/Output Management)                       │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Input:   Sensing, Formatting, Filtering        │    │   │
    │  │  │  Output:  Formatting, Synthesizing, Displaying  │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │              DIALOGUE CONTROL                            │   │
    │  │          (Input/Output Sequencing)                       │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Manages dialogue state                          │    │   │
    │  │  │  Enforces sequencing constraints                 │    │   │
    │  │  │  Routes messages between Presentation & Func.    │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │               FUNCTIONALITY                             │   │
    │  │          (Application Logic)                            │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Domain-specific operations                      │    │   │
    │  │  │  Data processing                                 │    │   │
    │  │  │  Business rules                                  │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └─────────────────────────────────────────────────────────┘   │
    │                                                                 │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                     SWITCH                               │   │
    │  │          (Control Mechanism)                             │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Routes control between layers                   │    │   │
    │  │  │  Manages layer activation                        │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └─────────────────────────────────────────────────────────┘   │
    └─────────────────────────────────────────────────────────────────┘
```

### Components

| Component | Responsibility | Key Features |
|-----------|----------------|--------------|
| **Presentation** | Input/Output management | Sensing, formatting, filtering, display |
| **Dialogue Control** | Sequencing control | State management, message routing |
| **Functionality** | Application logic | Domain operations, data processing |
| **Switch** | Control mechanism | Routes control between layers |

### Data Flow

```
INPUT:  User → Presentation → Dialogue Control → Functionality
OUTPUT: Functionality → Dialogue Control → Presentation → User
CONTROL: Switch manages activation of each layer
```

### Key Features

| Feature | Description |
|---------|-------------|
| **Separation of Concerns** | Each layer has distinct responsibilities |
| **Layered Communication** | Layers communicate only with adjacent layers |
| **Switch Mechanism** | Central control for layer activation |
| **Unidirectional Flow** | Input flows down, output flows up |

### Advantages & Disadvantages

| Advantages | Disadvantages |
|------------|---------------|
| Clear separation of concerns | Limited flexibility |
| Easy to understand | Switch can become bottleneck |
| Modular design | Layers may not map to real needs |
| Good for simple systems | Complex for large systems |

### Exam Tips
- **Common question**: "Explain the role of the Switch in Seeheim"
- **Key insight**: Switch manages control flow between layers
- **Application**: Use as reference for layered architectures
- **Remember**: Seeheim is a reference model, not implementation guide

---

## 10. Arch/Slinky Model (Ch8)

### Overview
Architectural model that adds a "Dialogue" layer between Presentation and Functionality, with an adaptor layer.

### Structure

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                      ARCH/SLINKY MODEL                          │
    │                                                                 │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                PHYSICAL LAYER                            │   │
    │  │          (Devices, I/O Hardware)                         │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Keyboard, Mouse, Screen, Speakers              │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │               LEXICAL LAYER                             │   │
    │  │          (Input/Output Processing)                      │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Input:  Character recognition, filtering       │    │   │
    │  │  │  Output: Character generation, formatting       │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │               DIALOGUE LAYER                            │   │
    │  │          (Interaction Management)                       │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Manages interaction sequences                   │    │   │
    │  │  │  Enforces dialogue constraints                   │    │   │
    │  │  │  Routes messages                                 │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │        FUNCTIONAL CORE ADAPTOR                          │   │
    │  │          (Interface to Functionality)                   │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Translates between dialogue and functionality   │    │   │
    │  │  │  Manages data format conversions                 │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │            FUNCTIONAL CORE                              │   │
    │  │          (Application Logic)                            │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Domain operations, data processing              │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └─────────────────────────────────────────────────────────┘   │
    └─────────────────────────────────────────────────────────────────┘
```

### Components

| Component | Responsibility | Key Features |
|-----------|----------------|--------------|
| **Physical** | Device hardware | Keyboard, mouse, screen |
| **Lexical** | Input/output processing | Character recognition, formatting |
| **Dialogue** | Interaction management | Sequence control, message routing |
| **Functional Core Adaptor** | Interface to functionality | Format translation, data conversion |
| **Functional Core** | Application logic | Domain operations, business rules |

### Comparison with Seeheim

| Feature | Seeheim | Arch/Slinky |
|---------|---------|-------------|
| **Layers** | 3 + Switch | 5 layers |
| **Dialogue** | Dialogue Control | Dialogue Layer |
| **Adaptor** | None | Functional Core Adaptor |
| **Physical** | Part of Presentation | Separate Physical Layer |
| **Flexibility** | Less flexible | More flexible |

### Key Features

| Feature | Description |
|---------|-------------|
| **More Granular** | Finer separation of concerns |
| **Adaptor Pattern** | Explicit interface to functionality |
| **Physical Layer** | Explicit handling of I/O devices |
| **Better for Complex Systems** | More layers for more complexity |

### Exam Tips
- **Common question**: "How does Arch/Slinky improve on Seeheim?"
- **Key insight**: More layers allow better separation of concerns
- **Application**: Use for complex interactive systems
- **Remember**: Adaptor layer is key innovation over Seeheim

---

## 11. MVC Model (Ch8)

### Overview
Model-View-Controller pattern that separates application data (Model) from presentation (View) and user interaction (Controller).

### Structure

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                      MVC MODEL                                  │
    │                                                                 │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                    USER                                  │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                 CONTROLLER                               │   │
    │  │          (Handles User Input)                           │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Processes user actions                         │    │   │
    │  │  │  Updates Model based on input                   │    │   │
    │  │  │  Selects View to display                        │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │              ┌────────────┴────────────┐                      │
    │              │                         │                      │
    │              ▼                         ▼                      │
    │  ┌─────────────────────┐   ┌─────────────────────┐          │
    │  │       MODEL         │   │       VIEW           │          │
    │  │  (Application Data) │   │  (Presentation)      │          │
    │  │                     │   │                      │          │
    │  │  ┌───────────────┐  │   │  ┌───────────────┐  │          │
    │  │  │ Domain Data   │  │   │  │ Display       │  │          │
    │  │  │ Business Rules│  │   │  │ Formatting    │  │          │
    │  │  │ State         │  │   │  │ Rendering     │  │          │
    │  │  └───────────────┘  │   │  └───────────────┘  │          │
    │  └──────────┬──────────┘   └──────────┬──────────┘          │
    │             │                         │                      │
    │             └────────────┬────────────┘                      │
    │                          │                                   │
    │                          ▼                                   │
    │  ┌─────────────────────────────────────────────────────────┐ │
    │  │                    DATA FLOW                             │ │
    │  │                                                          │ │
    │  │  User → Controller → Model → View → User                │ │
    │  │                                                          │ │
    │  │  Controller updates Model                               │ │
    │  │  Model notifies View of changes                         │ │
    │  │  View updates display                                   │ │
    │  │  User sees updated display                              │ │
    │  └─────────────────────────────────────────────────────────┘ │
    └─────────────────────────────────────────────────────────────────┘
```

### Components

| Component | Responsibility | Key Features |
|-----------|----------------|--------------|
| **Model** | Application data and logic | Domain data, business rules, state management |
| **View** | Presentation and display | Rendering, formatting, display management |
| **Controller** | User input handling | Input processing, action dispatching |

### Data Flow

```
1. User performs action (e.g., clicks button)
2. Controller processes action
3. Controller updates Model
4. Model notifies View of changes
5. View updates display
6. User sees updated display
```

### Observer Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                    OBSERVER PATTERN                              │
│                                                                 │
│  MODEL (Subject)                                                │
│  ├── observers[] (list of Views)                               │
│  ├── attach(observer)                                           │
│  ├── detach(observer)                                           │
│  └── notify()                                                   │
│       │                                                         │
│       ├──▶ VIEW 1 (Observer)                                   │
│       │    └── update()                                         │
│       │                                                         │
│       ├──▶ VIEW 2 (Observer)                                   │
│       │    └── update()                                         │
│       │                                                         │
│       └──▶ VIEW 3 (Observer)                                   │
│            └── update()                                         │
└─────────────────────────────────────────────────────────────────┘
```

### Variations

| Variation | Description |
|-----------|-------------|
| **MVP** | Model-View-Presenter: Presenter mediates between Model and View |
| **MVVM** | Model-View-ViewModel: ViewModel provides data binding |
| **PAC** | Presentation-Abstraction-Control: Hierarchical version |

### Issues

| Issue | Description |
|-------|-------------|
| **Tight Coupling** | Views directly depend on Model |
| **Update Overhead** | Frequent updates can be expensive |
| **Complex State** | Managing state across components is difficult |
| **Testing** | Hard to unit test due to dependencies |

### Exam Tips
- **Common question**: "Explain the Observer pattern in MVC"
- **Key insight**: Model notifies View of changes, not vice versa
- **Application**: Use MVC for separating data from presentation
- **Remember**: Controller handles user input, not View

---

## 12. PAC Model (Ch8)

### Overview
Hierarchical version of MVC with Presentation, Abstraction, and Control components at multiple levels.

### Structure

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                      PAC MODEL                                  │
    │                                                                 │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                    TOP LEVEL                             │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  P: Top-level presentation                       │    │   │
    │  │  │  A: Overall system abstraction                   │    │   │
    │  │  │  C: Top-level control                            │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │            ┌──────────────┼──────────────┐                    │
    │            │              │              │                    │
    │            ▼              ▼              ▼                    │
    │  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐          │
    │  │  LEVEL 1    │  │  LEVEL 1    │  │  LEVEL 1    │          │
    │  │  ┌───────┐  │  │  ┌───────┐  │  │  ┌───────┐  │          │
    │  │  │ P     │  │  │  │ P     │  │  │  │ P     │  │          │
    │  │  ├───────┤  │  │  ├───────┤  │  │  ├───────┤  │          │
    │  │  │ A     │  │  │  │ A     │  │  │  │ A     │  │          │
    │  │  ├───────┤  │  │  ├───────┤  │  │  ├───────┤  │          │
    │  │  │ C     │  │  │  │ C     │  │  │  │ C     │  │          │
    │  │  └───────┘  │  │  └───────┘  │  │  └───────┘  │          │
    │  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘          │
    │         │                │                │                    │
    │         ▼                ▼                ▼                    │
    │  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐          │
    │  │  LEVEL 2    │  │  LEVEL 2    │  │  LEVEL 2    │          │
    │  │  (More      │  │  (More      │  │  (More      │          │
    │  │   detail)   │  │   detail)   │  │   detail)   │          │
    │  └─────────────┘  └─────────────┘  └─────────────┘          │
    └─────────────────────────────────────────────────────────────────┘
```

### Components

| Component | Responsibility | Key Features |
|-----------|----------------|--------------|
| **Presentation (P)** | User interface | Visual display, input handling |
| **Abstraction (A)** | Domain model | Data, operations, business logic |
| **Control (C)** | Coordination | Mediates between P and A, manages communication |

### Hierarchical Structure

```
┌─────────────────────────────────────────────────────────────────┐
│                    HIERARCHICAL PAC                              │
│                                                                 │
│  TOP LEVEL                                                      │
│  ├── P: Main window                                            │
│  ├── A: Application state                                      │
│  └── C: Application control                                    │
│       │                                                         │
│       ├── LEVEL 1 (Major components)                           │
│       │   ├── P: Menu bar                                       │
│       │   ├── A: Document model                                 │
│       │   └── C: Document control                               │
│       │                                                         │
│       ├── LEVEL 1 (Major components)                           │
│       │   ├── P: Toolbar                                        │
│       │   ├── A: Tool settings                                  │
│       │   └── C: Tool control                                   │
│       │                                                         │
│       └── LEVEL 1 (Major components)                           │
│           ├── P: Content area                                   │
│           ├── A: Content model                                  │
│           └── C: Content control                                │
│                │                                                │
│                └── LEVEL 2 (Sub-components)                     │
│                    ├── P: Text editor                           │
│                    ├── A: Text model                            │
│                    └── C: Text control                          │
└─────────────────────────────────────────────────────────────────┘
```

### Comparison with MVC

| Feature | MVC | PAC |
|---------|-----|-----|
| **Structure** | Flat | Hierarchical |
| **Components** | 3 | 3 × N levels |
| **Control** | Single Controller | Multiple Controllers |
| **Communication** | Direct | Through Control |
| **Scalability** | Limited | Better for large systems |

### Key Features

| Feature | Description |
|---------|-------------|
| **Hierarchical** | Multiple levels of detail |
| **Separation** | Clear separation at each level |
| **Coordination** | Control component mediates communication |
| **Scalability** | Can handle complex systems |

### Exam Tips
- **Common question**: "How does PAC differ from MVC?"
- **Key insight**: PAC is hierarchical; MVC is flat
- **Application**: Use PAC for large, complex interactive systems
- **Remember**: Each level has its own P, A, and C components

---

## 13. IBIS Model (Ch6)

### Overview
Issue-Based Information System for structured deliberation and decision-making. Used for design rationale.

### Structure

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                      IBIS MODEL                                 │
    │                                                                 │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                      ISSUE                               │   │
    │  │          (Question or Problem)                           │   │
    │  │                                                          │   │
    │  │  "How should we design the login screen?"               │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │            ┌──────────────┼──────────────┐                    │
    │            │              │              │                    │
    │            ▼              ▼              ▼                    │
    │  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐          │
    │  │ POSITION 1  │  │ POSITION 2  │  │ POSITION 3  │          │
    │  │             │  │             │  │             │          │
    │  │ Use simple  │  │ Use OAuth   │  │ Use biomet- │          │
    │  │ password    │  │ login       │  │ ric auth    │          │
    │  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘          │
    │         │                │                │                    │
    │    ┌────┴────┐      ┌────┴────┐      ┌────┴────┐            │
    │    │         │      │         │      │         │            │
    │    ▼         ▼      ▼         ▼      ▼         ▼            │
    │  ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐          │
    │  │ARG+ │ │ARG- │ │ARG+ │ │ARG- │ │ARG+ │ │ARG- │          │
    │  │Easy │ │Inse-│ │Fam- │ │Com- │ │Sec- │ │Cost │          │
    │  │to    │ │cure │ │iliar│ │plex │ │ure  │ │     │          │
    │  │impl-│ │     │ │     │ │     │ │     │ │     │          │
    │  │ement│ │     │ │     │ │     │ │     │ │     │          │
    │  └─────┘ └─────┘ └─────┘ └─────┘ └─────┘ └─────┘          │
    └─────────────────────────────────────────────────────────────────┘
```

### Components

| Component | Description | Example |
|-----------|-------------|---------|
| **Issue** | Question or problem to be resolved | "How should we design the login screen?" |
| **Position** | Possible answer or solution | "Use simple password authentication" |
| **Argument** | Support or反对 for a position | "Easy to implement" (pro), "Insecure" (con) |

### Relationship Types

| Relationship | Description |
|--------------|-------------|
| **responds-to** | Position responds to an Issue |
| **supports** | Argument supports a Position |
| **objectsto** | Argument objects to a Position |
| **questions** | Position questions another Position |

### gIBIS (Graphical IBIS)

```
┌─────────────────────────────────────────────────────────────────┐
│                      gIBIS NOTATION                              │
│                                                                 │
│  ┌─────────────────┐    ┌─────────────────┐                    │
│  │    ISSUE        │    │    POSITION     │                    │
│  │  ┌───────────┐  │    │  ┌───────────┐  │                    │
│  │  │ Question  │  │    │  │ Solution  │  │                    │
│  │  └───────────┘  │    │  └───────────┘  │                    │
│  └────────┬────────┘    └────────┬────────┘                    │
│           │                      │                              │
│           │    ┌─────────────────┼─────────────────┐          │
│           │    │                 │                 │          │
│           ▼    ▼                 ▼                 ▼          │
│    ┌─────────────────┐    ┌─────────────────┐                │
│    │    ARGUMENT     │    │    ARGUMENT     │                │
│    │    (pro)        │    │    (con)        │                │
│    └─────────────────┘    └─────────────────┘                │
└─────────────────────────────────────────────────────────────────┘
```

### Applications

| Application | Description |
|-------------|-------------|
| **Design Rationale** | Document design decisions and reasoning |
| **Meeting Support** | Structured discussion and decision-making |
| **Requirements Engineering** | Explore design alternatives |
| **Knowledge Management** | Capture and organize design knowledge |

### Exam Tips
- **Common question**: "How does IBIS support design rationale?"
- **Key insight**: IBIS structures deliberation around issues, positions, and arguments
- **Application**: Use to document design decisions
- **Remember**: gIBIS is graphical notation for IBIS

---

## 14. QOC Model (Ch6)

### Overview
Questions, Options, and Criteria model for representing design rationale. More structured than IBIS.

### Structure

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                      QOC MODEL                                  │
    │                                                                 │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                    QUESTION                               │   │
    │  │          (Design Decision to Make)                        │   │
    │  │                                                          │   │
    │  │  "What navigation structure should we use?"             │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │            ┌──────────────┼──────────────┐                    │
    │            │              │              │                    │
    │            ▼              ▼              ▼                    │
    │  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐          │
    │  │  OPTION 1   │  │  OPTION 2   │  │  OPTION 3   │          │
    │  │             │  │             │  │             │          │
    │  │ Hierarchical│  │   Tabbed    │  │  Search-    │          │
    │  │   menus     │  │ interface   │  │  based      │          │
    │  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘          │
    │         │                │                │                    │
    │    ┌────┴────┐      ┌────┴────┐      ┌────┴────┐            │
    │    │         │      │         │      │         │            │
    │    ▼         ▼      ▼         ▼      ▼         ▼            │
    │  ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐ ┌─────┐          │
    │  │CRIT+ │ │CRIT-│ │CRIT+ │ │CRIT-│ │CRIT+ │ │CRIT-│          │
    │  │Fam-  │ │Deep │ │Over- │ │Simp-│ │Flex-│ │Com- │          │
    │  │iliar │ │nav- │ │view  │ │licity│ │ible │ │plex │          │
    │  │      │ │est- │ │      │ │      │ │     │ │     │          │
    │  │      │ │ing  │ │      │ │      │ │     │ │     │          │
    │  └─────┘ └─────┘ └─────┘ └─────┘ └─────┘ └─────┘          │
    └─────────────────────────────────────────────────────────────────┘
```

### Components

| Component | Description | Example |
|-----------|-------------|---------|
| **Question** | Design decision to be made | "What navigation structure should we use?" |
| **Option** | Possible answer to the question | "Hierarchical menus", "Tabbed interface" |
| **Criteria** | Standards for evaluating options | "Familiarity", "Simplicity", "Flexibility" |

### QOC Diagram Notation

```
┌─────────────────────────────────────────────────────────────────┐
│                    QOC NOTATION                                  │
│                                                                 │
│  ┌─────────────────┐                                            │
│  │    QUESTION     │  (Rectangle)                               │
│  └────────┬────────┘                                            │
│           │                                                      │
│    ┌──────┴──────┐                                              │
│    │             │                                              │
│    ▼             ▼                                              │
│  ┌─────┐      ┌─────┐                                          │
│  │OPT 1│      │OPT 2│  (Oval)                                  │
│  └──┬──┘      └──┬──┘                                          │
│     │             │                                              │
│  ┌──┴──┐      ┌──┴──┐                                          │
│  │     │      │     │                                          │
│  ▼     ▼      ▼     ▼                                          │
│ ┌───┐ ┌───┐ ┌───┐ ┌───┐                                        │
│ │C+ │ │C- │ │C+ │ │C- │  (Diamond)                             │
│ └───┘ └───┘ └───┘ └───┘                                        │
│                                                                 │
│  ─── support relationship                                       │
│  - - - oppose relationship                                      │
│  ─ · ─ evaluation relationship                                  │
└─────────────────────────────────────────────────────────────────┘
```

### Evaluation Matrix

| Option | Criterion 1 | Criterion 2 | Criterion 3 | Score |
|--------|-------------|-------------|-------------|-------|
| Hierarchical menus | +Familiar | -Deep nesting | +Overview | 2-1=1 |
| Tabbed interface | +Simplicity | -Overview | +Flexibility | 2-1=1 |
| Search-based | +Flexibility | -Complex | +Overview | 2-1=1 |

### Comparison with IBIS

| Feature | IBIS | QOC |
|---------|------|-----|
| **Structure** | Less structured | More structured |
| **Components** | Issue, Position, Argument | Question, Option, Criteria |
| **Notation** | Graphical (gIBIS) | Diagrammatic |
| **Focus** | Deliberation | Evaluation |
| **Use** | Meeting support | Design rationale |

### Applications

| Application | Description |
|-------------|-------------|
| **Design Rationale** | Document design decisions |
| **Evaluation** | Compare design alternatives |
| **Communication** | Explain design rationale to stakeholders |
| **Education** | Teach design thinking |

### Exam Tips
- **Common question**: "How does QOC differ from IBIS?"
- **Key insight**: QOC is more structured and evaluation-focused
- **Application**: Use to systematically evaluate design alternatives
- **Remember**: Criteria can be positive (+) or negative (-)

---

## 15. Client-Server Architecture (Ch8)

### Overview
Distributed architecture where clients request services from a server. Common in networked interactive systems.

### Structure

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                  CLIENT-SERVER ARCHITECTURE                     │
    │                                                                 │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                     CLIENTS                              │   │
    │  │                                                          │   │
    │  │  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐   │   │
    │  │  │ CLIENT  │  │ CLIENT  │  │ CLIENT  │  │ CLIENT  │   │   │
    │  │  │    1    │  │    2    │  │    3    │  │    4    │   │   │
    │  │  └────┬────┘  └────┬────┘  └────┬────┘  └────┬────┘   │   │
    │  │       │            │            │            │         │   │
    │  │       ▼            ▼            ▼            ▼         │   │
    │  │  ┌─────────────────────────────────────────────────┐   │   │
    │  │  │           ABSTRACT TERMINALS                    │   │   │
    │  │  │     (Virtual representations of clients)       │   │   │
    │  │  └─────────────────────────────────────────────────┘   │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                     SERVER                               │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Application Logic                               │    │   │
    │  │  │  Data Management                                 │    │   │
    │  │  │  Session Management                              │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                   DEVICE DRIVER                         │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Hardware abstraction                            │    │   │
    │  │  │  I/O management                                  │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └─────────────────────────────────────────────────────────┘   │
    └─────────────────────────────────────────────────────────────────┘
```

### Components

| Component | Responsibility | Key Features |
|-----------|----------------|--------------|
| **Client** | User interface, local processing | Handles user interaction |
| **Abstract Terminal** | Virtual client representation | Decouples client from server |
| **Server** | Application logic, data management | Centralized processing |
| **Device Driver** | Hardware abstraction | Handles I/O devices |

### Communication Patterns

| Pattern | Description | Example |
|---------|-------------|---------|
| **Request-Response** | Client sends request, server responds | HTTP requests |
| **Publish-Subscribe** | Server pushes updates to clients | Real-time updates |
| **Peer-to-Peer** | Clients communicate directly | File sharing |

### Types of Client-Server

| Type | Description | Example |
|------|-------------|---------|
| **Thick Client** | Most logic on client | Desktop applications |
| **Thin Client** | Most logic on server | Web applications |
| **Hybrid** | Logic distributed | Modern web apps |

### Issues

| Issue | Description |
|-------|-------------|
| **Latency** | Network delays affect responsiveness |
| **Scalability** | Server must handle multiple clients |
| **Security** | Data transmission and access control |
| **State Management** | Maintaining session state across requests |

### Exam Tips
- **Common question**: "Explain the role of abstract terminals"
- **Key insight**: Abstract terminals decouple clients from server implementation
- **Application**: Use client-server for networked interactive systems
- **Remember**: Thick vs. thin client is important design decision

---

## 16. X Windows Architecture (Ch8)

### Overview
Window system for networked graphical user interfaces. Implements client-server model for window management.

### Structure

```
    ┌─────────────────────────────────────────────────────────────────┐
    │                    X WINDOWS ARCHITECTURE                        │
    │                                                                 │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                     CLIENTS                              │   │
    │  │                                                          │   │
    │  │  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐   │   │
    │  │  │ X Client│  │ X Client│  │ X Client│  │ X Client│   │   │
    │  │  │   App   │  │   App   │  │   App   │  │   App   │   │   │
    │  │  └────┬────┘  └────┬────┘  └────┬────┘  └────┬────┘   │   │
    │  │       │            │            │            │         │   │
    │  │       ▼            ▼            ▼            ▼         │   │
    │  │  ┌─────────────────────────────────────────────────┐   │   │
    │  │  │              X PROTOCOL                         │   │   │
    │  │  │     (Communication between client & server)     │   │   │
    │  │  └─────────────────────────────────────────────────┘   │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                     X SERVER                             │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Window Management                               │    │   │
    │  │  │  Input Management                                │    │   │
    │  │  │  Graphics Output                                 │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │              WINDOW MANAGER                              │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Window placement and decoration                 │    │   │
    │  │  │  User interaction with windows                   │    │   │
    │  │  │  Application launching                           │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └────────────────────────┬────────────────────────────────┘   │
    │                           │                                    │
    │                           ▼                                    │
    │  ┌─────────────────────────────────────────────────────────┐   │
    │  │                DISPLAY HARDWARE                          │   │
    │  │                                                          │   │
    │  │  ┌─────────────────────────────────────────────────┐    │   │
    │  │  │  Screen, keyboard, mouse                        │    │   │
    │  │  └─────────────────────────────────────────────────┘    │   │
    │  └─────────────────────────────────────────────────────────┘   │
    └─────────────────────────────────────────────────────────────────┘
```

### Components

| Component | Responsibility | Key Features |
|-----------|----------------|--------------|
| **X Client** | Application programs | Sends requests to X server |
| **X Protocol** | Communication protocol | Network-transparent communication |
| **X Server** | Manages display | Handles window operations, input |
| **Window Manager** | User interaction | Window placement, decoration |
| **Display Hardware** | Physical output | Screen, keyboard, mouse |

### X Protocol

```
┌─────────────────────────────────────────────────────────────────┐
│                    X PROTOCOL                                    │
│                                                                 │
│  CLIENT ──────────────────────────────────────────▶ SERVER      │
│                                                                 │
│  Requests:                                                      │
│  ├── CreateWindow                                              │
│  ├── MapWindow                                                  │
│  ├── DrawLine                                                   │
│  ├── FillRectangle                                              │
│  └── GetInput                                                   │
│                                                                 │
│  Events:                                                        │
│  ├── KeyPress                                                   │
│  ├── ButtonPress                                                │
│  ├── Expose                                                     │
│  └── ConfigureNotify                                            │
│                                                                 │
│  Replies:                                                       │
│  ├── GetGeometry                                                │
│  ├── QueryFont                                                  │
│  └── GetImage                                                   │
└─────────────────────────────────────────────────────────────────┘
```

### Key Features

| Feature | Description |
|---------|-------------|
| **Network Transparency** | Client and server can run on different machines |
| **Device Independence** | Applications work on any X-compatible display |
| **Extensible** | Can add new features through extensions |
| **Window Management** | Separated from application logic |

### Window Manager Examples

| Window Manager | Description |
|----------------|-------------|
| **twm** | Tab Window Manager (basic) |
| **fvwm** | F Virtual Window Manager |
| **GNOME** | GNU Network Object Model Environment |
| **KDE** | K Desktop Environment |

### Issues

| Issue | Description |
|-------|-------------|
| **Complexity** | X protocol is complex and verbose |
| **Performance** | Network latency can affect responsiveness |
| **Security** | Limited built-in security features |
| **Modern Alternatives** | Wayland replaces X for many systems |

### Comparison with Modern Systems

| Feature | X Windows | Wayland |
|---------|-----------|---------|
| **Architecture** | Client-server | Direct rendering |
| **Security** | Limited | Better |
| **Performance** | Network overhead | Better |
| **Complexity** | High | Lower |

### Exam Tips
- **Common question**: "Explain the X Protocol"
- **Key insight**: X Protocol enables network-transparent window management
- **Application**: Use X Windows as example of client-server window system
- **Remember**: Window Manager is separate from X Server

---

## 17. GOMS Model (Ch9)

### Overview
Goals, Operators, Methods, Selection — a model-based evaluation approach that **predicts user performance** with a particular interface. Used to filter design options before implementation.

### Components

| Component | Definition | Example |
|-----------|-----------|---------|
| **Goals** | What the user wants to achieve | "Send an email" |
| **Operators** | Primitive physical/mental actions | Keystrokes, mouse clicks, pointing, mental operators |
| **Methods** | Sequences of operators that accomplish a goal | Open compose → type address → type subject → click send |
| **Selection rules** | Choose between alternative methods when multiple exist | If attachment → use "attach then send"; otherwise → "direct send" |

### When to Use
- **Comparing interface designs** by predicting task completion times
- **Filtering design options** early in the process — before implementation
- For **repetitive, well-defined tasks** where operator sequences are clear

### Exam Tips
- **Key insight**: GOMS provides quantitative predictions without user testing
- **Application**: Use to compare Design A vs Design B by calculating predicted execution times

---

## 18. Keystroke-Level Model — KLM (Ch9)

### Overview
Lower-level variant of GOMS that provides **quantitative time predictions** for low-level physical tasks. Breaks interaction into primitive operators with measured durations.

### Operator Table

| Operator | Symbol | Description | Typical Time |
|----------|--------|-------------|-------------|
| **Keystroke** | K | Pressing a key or clicking a button | ~0.2–0.3s |
| **Pointing** | P | Pointing to a target with mouse/pointer | ~1.1s |
| **Mental preparation** | Mh | Mental hesitation before acting | ~1.35s |
| **Home (hand to device)** | H | Moving hand between keyboard and mouse | ~0.4s |
| **Draw (hand to screen)** | D | Moving hand to draw on tablet/screen | Varies |
| **System response** | Rc | Waiting for system response | Varies |
| **Write (handwriting)** | Wb | Writing by hand on tablet | ~1.5s/char |
| **Browse button** | Bb | Pressing button to browse/scroll | ~0.2s |

**Total time** = Σ(time for each operator) + mental operators for preparation

### When to Use
- **Comparing interface designs** by calculating predicted task times before implementation
- For **low-level physical tasks** (keystrokes, mouse movements)
- When you need **quantitative predictions** without user testing

### Limitations
- Best for low-level physical tasks; doesn't capture higher-level cognitive processes
- Doesn't model learning effects or error recovery well

---

## 19. Nielsen's Severity Rating Scale (Ch9)

### Overview
0–4 scale for rating usability problem severity during heuristic evaluation. Helps **prioritize fixes** and communicate urgency to stakeholders.

### The Scale

| Rating | Label | Description | Action |
|--------|-------|-------------|--------|
| **0** | Not a usability problem | Not an issue | Ignore |
| **1** | Cosmetic | Fix only if extra time available | Low priority |
| **2** | Minor | Low priority, minor inconvenience | Fix when possible |
| **3** | Major | High priority, important to fix | Fix before release |
| **4** | Catastrophe | Usability emergency, blocks users | Must fix before release |

### When to Use
- During **heuristic evaluation** to rate each discovered violation
- To **prioritize** which problems to fix first
- For **communicating** problem severity to development teams and stakeholders

### Exam Tips
- **Key insight**: 3–5 evaluators find ~75% of usability problems; each rates severity independently
- **Application**: Use with heuristic evaluation — rate every violation on this scale

---

## 20. 8-Factor Evaluation Method Selection (Ch9)

### Overview
Eight dimensions for choosing the right evaluation method based on your stage, needs, and resources. No single "best" method — the right choice depends on context.

### The 8 Factors

| Factor | Options / Considerations |
|--------|------------------------|
| **1. Stage in cycle** | Design stage (quick, cheap, analytic) vs. Implementation stage (comprehensive, user-based) |
| **2. Style** | Laboratory (controlled, specialist equipment) vs. Field (natural context, real behavior) |
| **3. Objectivity** | Subjective (evaluator-dependent — walkthrough, think aloud) vs. Objective (repeatable — experiments) |
| **4. Measures** | Quantitative (numeric, statistical) vs. Qualitative (non-numeric, detailed) |
| **5. Information level** | Low-level (specific decisions — "which font?") vs. High-level (overall — "is it usable?") |
| **6. Immediacy** | Immediate (during interaction — think aloud) vs. Post-hoc (after event — walkthrough) |
| **7. Intrusiveness** | Obtrusive (user aware, alters behavior) vs. Unobtrusive (automatic logging) |
| **8. Resources** | Time, money, equipment, participants, expertise, context access |

### When to Use
- When **deciding which evaluation method** to apply at a given project stage
- To **match methods** to available resources, expertise, and evaluation goals
- For **justifying method choice** in reports and exam answers

### Exam Tips
- **Key insight**: Different methods serve different purposes — expert analysis for early designs, user testing for implementations
- **Application**: Use these 8 factors to systematically justify your method selection

---

## Comparative Summary

### Models Comparison Table

| Model | Type | Key Concept | Best For |
|-------|------|-------------|----------|
| **Norman's Loop** | Interaction | 7 stages, gulfs | Analyzing usability |
| **Abowd & Beale** | Framework | 4 languages, translation | Understanding translations |
| **Semantic Network** | Knowledge | Nodes, inheritance | Menu hierarchies |
| **Frames** | Knowledge | Slots, defaults | Form design |
| **Scripts** | Knowledge | Event sequences | Dialog design |
| **Production Rules** | Knowledge | IF-THEN rules | Context-sensitive UI |
| **Waterfall** | Process | Linear phases | Stable requirements |
| **Iterative Design** | Process | Feedback loops | HCI projects |
| **Seeheim** | Architecture | 3 layers + switch | Simple systems |
| **Arch/Slinky** | Architecture | 5 layers | Complex systems |
| **MVC** | Architecture | Model-View-Controller | Separating concerns |
| **PAC** | Architecture | Hierarchical MVC | Large systems |
| **IBIS** | Rationale | Issues, positions | Design decisions |
| **QOC** | Rationale | Questions, options | Design evaluation |
| **Client-Server** | Distributed | Clients, server | Networked systems |
| **X Windows** | Window | Client-server, protocol | Window management |
| **GOMS** | Performance | Goals, operators, methods, selection | Predicting task times |
| **KLM** | Performance | Operator time table | Comparing physical tasks |
| **Severity Scale** | Evaluation | 0–4 severity rating | Prioritizing usability fixes |
| **8-Factor Selection** | Methodology | 8 evaluation dimensions | Choosing evaluation method |

### Architecture Comparison

| Architecture | Layers | Control | Scalability | Complexity |
|--------------|--------|---------|-------------|------------|
| **Seeheim** | 3 | Switch | Low | Low |
| **Arch/Slinky** | 5 | Distributed | Medium | Medium |
| **MVC** | 3 | Observer | Medium | Medium |
| **PAC** | N×3 | Hierarchical | High | High |
| **Client-Server** | 4 | Centralized | High | Medium |

---

## Exam Preparation

### Common Exam Questions

1. **Norman's Loop**: Explain the gulfs of execution and evaluation
2. **Abowd & Beale**: How do the four languages relate?
3. **Knowledge Models**: Compare semantic networks, frames, and scripts
4. **Waterfall vs. Iterative**: Why is Waterfall problematic for HCI?
5. **Seeheim vs. Arch/Slinky**: What are the differences?
6. **MVC**: Explain the Observer pattern
7. **PAC**: How does PAC differ from MVC?
8. **IBIS vs. QOC**: Compare design rationale models
9. **Client-Server**: Explain the role of abstract terminals
10. **X Windows**: Describe the X Protocol
11. **GOMS**: Define Goals, Operators, Methods, Selection rules
12. **KLM**: Calculate predicted task time using operator table
13. **Severity Scale**: Rate usability problem severity (0–4)
14. **8-Factor Selection**: Justify evaluation method choice using 8 dimensions

### Key Relationships

```
KNOWLEDGE MODELS:           ARCHITECTURES:          PROCESS MODELS:
Semantic Network            Seeheim                 Waterfall
     │                          │                      │
     ▼                          ▼                      ▼
Frames                    Arch/Slinky              Iterative Design
     │                          │
     ▼                          ▼
Scripts                    MVC
                               │
                               ▼
                           PAC
```

### Study Tips

1. **Understand Relationships**: Know how models relate to each other
2. **Compare and Contrast**: Be able to explain differences between similar models
3. **Apply to Examples**: Use real-world examples to illustrate concepts
4. **Know Pros/Cons**: Understand advantages and disadvantages of each model
5. **Practice Diagrams**: Be able to draw and explain diagrams

---

*Generated for NU Applied Human-Computer Interaction Course*
*Covers Chapters 1-9: 20 Models and Frameworks*
