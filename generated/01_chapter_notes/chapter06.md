# Chapter 6: HCI in the Software Process - HCI Notes

## Overview
Chapter 6 covers how HCI fits into the software engineering process: the software lifecycle, waterfall model, usability engineering, iterative design and prototyping, and design rationale.

---

## 1. THE SOFTWARE LIFECYCLE

### Definition
Software engineering is the discipline for understanding the software design process, or life cycle. Designing for usability occurs at all stages of the life cycle, not as a single isolated activity.

### The Waterfall Model
1. **Requirements specification**
2. **Architectural design**
3. **Detailed design**
4. **Coding and unit testing**
5. **Integration and testing**
6. **Operation and maintenance**

### Activities in the Life Cycle

#### Requirements Specification
- Designer and customer try to capture what the system is expected to provide
- Can be expressed in natural language or more precise languages
- Task analysis provides detailed requirements

#### Architectural Design
- High-level description of how the system will provide the services required
- Factor system into major components and how they are interrelated
- Needs to satisfy both functional and non-functional requirements

#### Detailed Design
- Refinement of architectural components and interrelations
- Identify modules to be implemented separately
- Refinement is governed by non-functional requirements

### Verification and Validation
- **Verification**: designing the product right
- **Validation**: designing the right product
- **The formality gap**: validation will always rely to some extent on subjective means of proof
- Management and contractual issues: design in commercial and legal contexts

### Life Cycle for Interactive Systems
- **Cannot assume a linear sequence of activities** as in the waterfall model
- **Lots of feedback!** Multiple feedback loops between all stages

---

## 2. USABILITY ENGINEERING

### Definition
The ultimate test of usability based on measurement of user experience. Demands that specific usability measures be made explicit as requirements.

### Usability Specification
- Usability attribute/principle
- Measuring concept
- Measuring method
- Now level / worst case / planned level / best case

### Example: VCR Usability Specification
**Attribute**: Backward recoverability
- **Measuring concept**: Undo an erroneous programming sequence
- **Measuring method**: Number of explicit user actions to undo current program
- **Now level**: No current product allows such an undo
- **Worst case**: As many actions as it takes to program-in mistake
- **Planned level**: A maximum of two explicit user actions
- **Best case**: One explicit cancel action

### Problems
- Usability specification requires level of detail that may not be possible early in design
- Satisfying a usability specification does not necessarily satisfy usability

### ISO Usability Standard 9241
Adopts traditional usability categories:
- **Effectiveness** – can you achieve what you want to?
- **Efficiency** – can you do it without wasting effort?
- **Satisfaction** – do you enjoy the process?

### Some Metrics from ISO 9241
| Usability objective | Effectiveness measures | Efficiency measures | Satisfaction measures |
|---|---|---|---|
| Suitability for the task | Percentage of goals achieved | Time to complete a task | Rating scale for satisfaction |
| Appropriate for trained users | Number of power features used | Relative efficiency compared with an expert user | Rating scale for satisfaction with power features |
| Learnability | Percentage of functions learned | Time to learn criterion | Rating scale for ease of learning |
| Error tolerance | Percentage of errors corrected successfully | Time spent on correcting errors | Rating scale for error handling |

---

## 3. ITERATIVE DESIGN AND PROTOTYPING

### Why Iterative Design?
Iterative design overcomes inherent problems of incomplete requirements.

### Types of Prototypes
1. **Throwaway** – built quickly, discarded after use
2. **Incremental** – built piece by piece, added to system
3. **Evolutionary** – evolves into final system

### Techniques for Prototyping

#### Storyboards
- Need not be computer-based
- Can be animated
- Visual representation of user interaction flow

#### Limited Functionality Simulations
- Some part of system functionality provided by designers
- Tools like HyperCard are common
- **Wizard of Oz technique** – human simulates computer response

#### Warning About Iterative Design
- Design inertia – early bad decisions stay bad
- Diagnosing real usability problems in prototypes... and not just the symptoms

---

## 4. DESIGN RATIONALE

### Definition
Design rationale is information that explains why a computer system is the way it is.

### Benefits
1. Communication throughout life cycle
2. Reuse of design knowledge across products
3. Enforces design discipline
4. Presents arguments for design trade-offs
5. Organizes potentially large design space
6. Capturing contextual information

### Types of Design Rationale

#### Process-oriented
- Preserves order of deliberation and decision-making

#### Structure-oriented
- Emphasizes post hoc structuring of considered design alternatives

---

## 5. ISSUE-BASED INFORMATION SYSTEM (IBIS)

### Basis
Basis for much of design rationale research. Process-oriented.

### Main Elements
- **Issues** – hierarchical structure with one 'root' issue
- **Positions** – potential resolutions of an issue
- **Arguments** – modify the relationship between positions and issues

### gIBIS (Graphical IBIS)
- **Issue** (central node)
  - **Position** responds to Issue
    - **Argument** supports Position
  - **Position** responds to Issue
    - **Argument** objects to Position
- **Sub-issue** specializes Issue
- **Sub-issue** generalizes Issue
- **Sub-issue** questions Issue

---

## 6. DESIGN SPACE ANALYSIS

### Structure-oriented approach

### QOC (Question-Option-Criterion)
- **Questions** (and sub-questions) – represent major issues of a design
- **Options** – provide alternative solutions to the question
- **Criteria** – the means to assess the options in order to make a choice

### DRL (Design Rationale Language)
- Similar to QOC with a larger language and more formal semantics

---

## 7. PSYCHOLOGICAL DESIGN RATIONALE

- To support task-artefact cycle in which user tasks are affected by the systems they use
- Aims to make explicit consequences of design for users
- Designers identify tasks system will support
- Scenarios are suggested to test task
- Users are observed on system
- Psychological claims of system made explicit
- Negative aspects of design can be used to improve next iteration of design

---

## KEY CONCEPTS FOR EXAM
1. **Software lifecycle**: requirements → architectural design → detailed design → coding → integration → maintenance
2. **Waterfall model**: sequential, but interactive systems need feedback loops
3. **Verification**: designing the product right; **Validation**: designing the right product
4. **Formality gap**: validation relies on subjective proof
5. **Usability engineering**: specific usability measures as requirements
6. **Usability specification**: attribute, measuring concept, method, now/worst/planned/best levels
7. **ISO 9241**: effectiveness, efficiency, satisfaction
8. **Iterative design**: overcomes incomplete requirements
9. **Prototypes**: throwaway, incremental, evolutionary
10. **Storyboards**: visual representation of user interaction
11. **Wizard of Oz**: human simulates computer response
12. **Design rationale**: explains why a system is the way it is
13. **IBIS**: issues, positions, arguments (process-oriented)
14. **gIBIS**: graphical version of IBIS
15. **QOC**: Questions, Options, Criteria (structure-oriented)
16. **DRL**: Design Rationale Language – larger, more formal than QOC
17. **Psychological design rationale**: make consequences of design for users explicit
