# HCI Heuristics & Principles Reference Guide

> **Course:** NU Applied Human-Computer Interaction
> **Purpose:** Comprehensive reference for usability heuristics, design principles, and cognitive frameworks

---

## Table of Contents

1. [Nielsen's 10 Usability Heuristics](#1-nielsens-10-usability-heuristics)
2. [Shneiderman's 8 Golden Rules](#2-shneidermans-8-golden-rules)
3. [Norman's 7 Principles of Interaction Design](#3-normans-7-principles-of-interaction-design)
4. [ISO 9241 Usability Definition](#4-iso-9241-usability-definition)
5. [Principles of Usability (Chapter 7)](#5-principles-of-usability-chapter-7)
6. [Gestalt Principles](#6-gestalt-principles)
7. [Fitts' Law](#7-fitts-law)
8. [Norman's 7 Stages of Action](#8-normans-7-stages-of-action)

---

## 1. Nielsen's 10 Usability Heuristics

*Jakob Nielsen's heuristics are general rules of thumb for interface design. They are widely used for evaluating usability in heuristic evaluations.*

### 1.1 Visibility of System Status

The system should always keep users informed about what is going on through appropriate feedback within a reasonable time.

- **Key idea:** Users need to know the current state to make informed decisions.
- **Examples:**
  - Download progress bars showing percentage complete
  - Loading spinners during data retrieval
  - "Saving..." indicators in Google Docs
  - Status badges (online/offline) in messaging apps
  - Step indicators in checkout flows ("Step 2 of 4")
- **Violation example:** A form submission with no feedback — user clicks "Submit" and nothing visibly happens.

### 1.2 Match Between System and the Real World

The system should speak the users' language, using words, phrases, and concepts familiar to the user rather than system-oriented terms. Follow real-world conventions, making information appear in a natural and logical order.

- **Key idea:** Reduce cognitive load by using domain-familiar language and metaphors.
- **Examples:**
  - Trash/delete icons resembling physical trash cans
  - Shopping cart icons on e-commerce sites
  - Calendar widgets that mimic physical calendars
  - Using "Compose" instead of "New Record Insertion"
- **Violation example:** Error message "ERR_SQL_CONSTRAINT_VIOLATION_0x8007005" instead of "A user with this email already exists."

### 1.3 User Control and Freedom

Users often choose system functions by mistake and will need a clearly marked "emergency exit" to leave the unwanted state without having to go through an extended process. Support undo and redo.

- **Key idea:** Users make mistakes; the system must allow recovery.
- **Examples:**
  - Undo/redo in text editors (Ctrl+Z / Ctrl+Y)
  - "Cancel" button in multi-step wizards
  - Gmail's "Undo Send" feature
  - Shopping cart item removal before checkout
  - Confirmation dialogs before destructive actions
- **Violation example:** A file manager with no way to undo a delete operation.

### 1.4 Consistency and Standards

Users should not have to wonder whether different words, situations, or actions mean the same thing. Follow platform and industry conventions.

- **Key idea:** Consistency reduces learning time and prevents confusion.
- **Two types:**
  - **Internal consistency:** Within the same application (buttons, colors, terminology)
  - **External consistency:** Across different applications and platforms (Ctrl+S to save)
- **Examples:**
  - Red consistently indicating errors or destructive actions
  - Navigation menus placed in familiar top/left positions
  - Using "OK" and "Cancel" consistently across dialogs
  - Consistent iconography (hamburger menu, gear for settings)
- **Violation example:** Using green for "delete" in one screen and red in another.

### 1.5 Error Prevention

Even better than good error messages is a careful design that prevents problems from occurring in the first place. There are two types of errors: slips and mistakes.

- **Key idea:** Eliminate error-prone conditions or check for them before the user commits.
- **Techniques:**
  - Disable unavailable options (grayed-out buttons)
  - Confirmation dialogs for irreversible actions
  - Input validation with format hints (phone number masks)
  - Confirmation before overwriting files
  - Auto-save features
- **Examples:**
  - Gmail suggesting "Did you forget the attachment?" based on email content
  - Password strength meters
  - "Are you sure you want to delete?" confirmation
  - Date pickers preventing invalid dates
- **Violation example:** Allowing a user to fill out a 20-field form with no validation until final submission.

### 1.6 Recognition Rather Than Recall

Make objects, actions, and options visible. The user should not have to remember information from one part of the dialogue to another. Instructions for use of the system should be visible or easily retrievable whenever appropriate.

- **Key idea:** Recognition is easier than recall; minimize memory demands.
- **Examples:**
  - Recently used files lists in Microsoft Office
  - Auto-complete suggestions in search bars
  - Related product recommendations on Amazon
  - Visible toolbar icons instead of hidden keyboard shortcuts
  - Breadcrumb navigation showing path hierarchy
- **Violation example:** A search interface that doesn't show search history or suggestions.

### 1.7 Flexibility and Efficiency of Use

Accelerators — unseen by the novice user — may often speed up the interaction for the expert user so that the design can cater to both inexperienced and experienced users. Allow users to tailor frequent actions.

- **Key idea:** Support both novice and expert users through adaptive interaction.
- **Examples:**
  - Keyboard shortcuts (Ctrl+C, Ctrl+V) alongside menu options
  - Customizable toolbars (Photoshop, VS Code)
  - Touch gestures alongside button navigation in mobile apps
  - Quick-access shortcuts or pinned items
  - Macro recording for repetitive tasks
- **Violation example:** An application requiring the same multi-click process for frequently performed actions with no shortcut mechanism.

### 1.8 Aesthetic and Minimalist Design

Interfaces should not contain information which is irrelevant or rarely needed. Every extra unit of information in a dialogue competes with the relevant units of information and diminishes their relative visibility.

- **Key idea:** Reduce noise; focus on essential content and functionality.
- **Examples:**
  - Google's homepage (minimal, focused on search)
  - Progressive disclosure hiding advanced options until needed
  - Card-based UI layouts with clear visual hierarchy
  - Calm technology principles in notifications
- **Violation example:** A dashboard cramming 50 metrics into one screen with no visual hierarchy.

### 1.9 Help Users Recognize, Diagnose, and Recover from Errors

Error messages should be expressed in plain language (no error codes), precisely indicate the problem, and constructively suggest a solution.

- **Key idea:** Error messages must be informative, not cryptic.
- **Error message anatomy:**
  1. What went wrong (in user-friendly language)
  2. Why it went wrong (brief explanation)
  3. What to do about it (actionable suggestion)
- **Examples:**
  - "Password must be at least 8 characters with one number" (not "Invalid input")
  - "File not found. Check the file path and try again."
  - Inline form validation: "Email address is missing an '@' symbol"
  - "No results found for 'iphne'. Did you mean 'iPhone'?"
- **Violation example:** "Error 500: Internal Server Error" with no context or guidance.

### 1.10 Help and Documentation

Even though it is better if the system can be used without documentation, it may be necessary to provide help and documentation. Any such information should be easy to search, focused on the user's task, list concrete steps to carry out, and not be too large.

- **Key idea:** Provide context-sensitive, task-focused help when needed.
- **Examples:**
  - Tooltips on icon buttons
  - Interactive walkthroughs for onboarding (e.g., Slack, Notion)
  - Searchable knowledge bases
  - Contextual help links next to complex form fields
  - In-app chatbots for real-time support
- **Violation example:** A 500-page PDF manual as the only form of help.

### Exam Tips — Nielsen's Heuristics

- **Identify violations:** Common exam format — analyze screenshots and map violations to specific heuristics.
- **Distinguish similar heuristics:** Error prevention (#5) vs. Help users recover from errors (#9) — one prevents, the other cures.
- **Remember all 10:** Use mnemonic: **V**ictor **M**ight **U**sher **C**onsistent **E**rror **R**ecognition **F**or **A**ll **H**elpful **D**ocumentation.
- **Provide examples:** For each heuristic, be ready with 2–3 real-world examples.
- **Overlap with other frameworks:** Nielsen's "Consistency" aligns with Shneiderman's "Strive for consistency"; "User control" aligns with "Permit easy reversal."

---

## 2. Shneiderman's 8 Golden Rules

*Ben Shneiderman's golden rules focus on interaction design principles derived from long-standing usage and common sense.*

### 2.1 Strive for Consistency

Consistent sequences of actions should be required in similar situations. Identical terminology should be used in prompts, menus, and help screens. Consistent commands should be employed throughout.

- **Explanation:** Consistency across interface elements (colors, terminology, layouts, workflows) reduces learning time and prevents user confusion. It applies to internal consistency (within the app) and external consistency (with platform norms).
- **Key aspects:**
  - Visual consistency (layout, colors, typography)
  - Functional consistency (same action produces same result)
  - Linguistic consistency (same terms for same concepts)
  - Platform consistency (follow OS conventions)
- **Example:** In Microsoft Office, Ctrl+B always means bold, whether in Word, PowerPoint, or Excel.

### 2.2 Enable Frequent Users to Use Shortcuts

The overhead of penalties is justified for experienced users who gain increased operational speed.

- **Explanation:** As users become proficient, they desire faster ways to accomplish tasks. Shortcuts (keyboard shortcuts, gestures, macros) improve efficiency without hindering novice users.
- **Key aspects:**
  - Keyboard shortcuts for common operations
  - Abbreviated forms (type-ahead)
  - Customizable quick-action buttons
  - Gesture shortcuts in touch interfaces
- **Example:** Gmail provides keyboard shortcuts (C for compose, / for search) that power users rely on daily.

### 2.3 Offer Informative Feedback

For every operator action, there should be some system feedback. For frequent and minor actions, the response can be modest, while for infrequent and major actions, the response should be more substantial.

- **Explanation:** Users need to know their actions were received and processed. Feedback should be proportional to the action's significance — minimal for routine actions, detailed for major ones.
- **Key aspects:**
  - Visual confirmation of actions (button states, highlights)
  - Progress indicators for long operations
  - Success/failure notifications
  - Status updates during processing
- **Example:** When sending an email, Gmail shows "Sending..." then "Message sent" with an undo option.

### 2.4 Design Dialogs to Yield Closure

Sequences of actions should be organized into groups with a beginning, middle, and end. Informative feedback at the completion of a group of actions gives users the satisfaction of accomplishment, a sense of relief, a signal to shed worry about accumulated thoughts, and a indicator that the way is clear to prepare for the next set of actions.

- **Explanation:** Every interaction sequence should have a clear endpoint that signals completion. This provides psychological closure and confidence that the task was accomplished.
- **Key aspects:**
  - Completion messages ("Your order has been placed")
  - Summary screens after multi-step processes
  - Visual closure cues (checkmarks, completion indicators)
  - Clear task boundaries
- **Example:** After submitting a web form, a "Thank you — your application was submitted successfully" page with a confirmation number.

### 2.5 Offer Error Prevention and Simple Error Handling

Design the interface to prevent errors from occurring in the first place. When errors do occur, the system should detect them and provide clear, constructive error messages.

- **Explanation:** Prevention is better than cure. When prevention fails, recovery should be straightforward. This combines both proactive and reactive error management.
- **Techniques:**
  - Input validation and constraints
  - Confirmation dialogs for destructive actions
  - Clear error messages with recovery suggestions
  - Undo mechanisms
- **Example:** A date picker that prevents selecting past dates for a future event, rather than showing an error after submission.

### 2.6 Permit Easy Reversal of Actions

Users often need to reverse their actions. Reversal operations can be at any level — single character, word, field entry, or an entire group of actions. This principle reduces fear of errors and encourages exploration.

- **Explanation:** The ability to undo reduces anxiety and promotes exploratory behavior. Users are more willing to try new things when they know mistakes are reversible.
- **Key aspects:**
  - Undo/redo functionality
  - "Back" navigation in wizards
  - Confirmation before irreversible actions
  - Multiple levels of undo
- **Example:** Photoshop allows multiple levels of undo (Ctrl+Z repeatedly), and Google Docs tracks full revision history.

### 2.7 Support Internal Locus of Control

Experienced users strongly desire the sense that they are in charge of the system and that the system responds to their actions. System actions should be initiated by user commands rather than a mandatory, inconvenient schedule.

- **Explanation:** Users want to feel in control — initiating actions, not being acted upon by the system. The system should respond to user-initiated commands, not force interactions.
- **Key aspects:**
  - User-initiated actions (not system-initiated interruptions)
  - Customizable workflows
  - Flexible interaction sequences
  - Predictable system responses
- **Example:** Users can choose when to check email rather than having pop-ups force attention; customizable notification settings.

### 2.8 Reduce Short-Term Memory Load

Humans have limited short-term memory. Interfaces should be designed to minimize the amount of information that users need to remember.

- **Explanation:** Working memory holds approximately 7±2 items (Miller's Law). Interfaces should reduce cognitive load by making information visible and easily retrievable.
- **Techniques:**
  - Visible controls and labels
  - Contextual information displays
  - Breadcrumb navigation
  - Consistent and predictable layouts
  - Listing options rather than requiring recall
- **Example:** Search engines show recent searches and suggestions rather than requiring users to remember and retype queries.

### Exam Tips — Shneiderman's Golden Rules

- **Memorize the list:** Use mnemonic: **C**onsistent **S**hortcuts **F**eedback **C**losure **E**rror **R**eversal **C**ontrol **M**emory.
- **Overlaps with Nielsen:** Consistency (#1) → Nielsen #4; Error prevention (#5) → Nielsen #5; Reversal (#6) → Nielsen #3.
- **Focus on action-oriented language:** Shneiderman's rules are about what designers should DO.
- **Provide examples:** Be ready with 2–3 concrete examples for each rule.
- **Emphasis on user empowerment:** Rules #3, #4, #6, #7 all center on giving users control and feedback.

---

## 3. Norman's 7 Principles of Interaction Design

*Don Norman's principles focus on making interfaces understandable through visibility, feedback, and conceptual models.*

### 3.1 Use Both Knowledge in the World and Knowledge in the Head

The information needed to complete an action must be available either in the world (external) or in the user's memory (internal). The more knowledge required in the head, the more design effort is needed.

- **Explanation:** Users rely on a combination of external cues (visible labels, icons) and internal knowledge (memorized procedures, mental models). Good design minimizes the need for knowledge in the head by providing sufficient knowledge in the world.
- **Key aspects:**
  - Knowledge in the world: Labels, icons, visible affordances, documentation
  - Knowledge in the head: Memorized shortcuts, learned conventions
  - Balance between the two based on frequency and importance
- **Example:** A calculator app shows both the keypad (knowledge in the world) and users bring math knowledge (knowledge in the head). Icons for operations (+, −, ×, ÷) bridge both.

### 3.2 Simplify the Structure of Tasks

Reduce the complexity of the task. Break complex tasks into smaller, manageable sub-tasks. Make the steps required for a task obvious and well-structured.

- **Explanation:** Complex tasks lead to errors. Designers should decompose tasks, remove unnecessary steps, and provide clear pathways. Chunking, progressive disclosure, and wizard-style flows help.
- **Key aspects:**
  - Chunk information into logical groups
  - Use progressive disclosure for complex workflows
  - Remove unnecessary steps
  - Provide templates and defaults
- **Example:** Online checkout flows break payment into steps: shipping → billing → review → confirm, rather than presenting all fields at once.

### 3.3 Make Things Visible: Bridge the Gulfs of Execution and Evaluation

There are two gulfs between the user and the system:
- **Gulf of Execution:** The gap between the user's goal and the means to execute it
- **Gulf of Evaluation:** The gap between the system's actual state and the user's understanding of that state

Design must bridge both gulfs through visibility and feedback.

- **Explanation:** Users need to see what actions are possible (execution) and understand what happened (evaluation). Visibility of controls, clear feedback, and system status indicators bridge these gulfs.
- **Key aspects:**
  - Visible controls and affordances
  - Clear feedback for every action
  - System status visibility
  - Natural mappings
- **Example:** A physical door with a flat plate says "push" (visible affordance); a door handle says "pull" (different affordance). The design bridges the gulf of execution.

### 3.4 Get the Mappings Right

Natural mapping is the relationship between controls and their effects. Good mapping makes it immediately obvious which control affects which outcome.

- **Explanation:** When the spatial or physical relationship between controls and their effects follows natural conventions, users can operate the system without learning arbitrary rules.
- **Key aspects:**
  - Spatial mapping (stove burner layout matches pot positions)
  - Cultural mapping (right = forward, left = backward)
  - Logical mapping (volume up increases sound)
  - Analogies to physical systems
- **Example:** A car's steering wheel turns right to go right (natural mapping). A thermostat where clockwise increases temperature (standard convention).

### 3.5 Exploit the Power of Constraints

Constraints limit the possible actions. They can be physical, logical, or cultural. Well-designed constraints prevent errors and guide users toward correct actions.

- **Explanation:** Constraints reduce the cognitive load of choosing among options by limiting what is possible. They can be inherent (physical) or added (designed).
- **Types of constraints:**
  - **Physical constraints:** Key shapes, plugs that only fit one way
  - **Logical constraints:** A date field rejecting letters
  - **Cultural constraints:** Red means stop/danger
  - **Semantic constraints:** Meaning limits possible actions
- **Example:** USB-C connectors are reversible (physical constraint preventing wrong insertion). Form fields that only accept numbers for phone inputs.

### 3.6 Design for Error

Errors happen. The goal is not to prevent all errors (impossible) but to minimize their occurrence and make recovery easy. Good designs anticipate likely errors and provide mechanisms to handle them gracefully.

- **Explanation:** Both slips (unconscious errors) and mistakes (conscious errors) must be anticipated. Design should:
  1. Prevent errors where possible
  2. Detect errors early
  3. Allow easy recovery
  4. Minimize consequences
- **Key aspects:**
  - Confirmation dialogs for destructive actions
  - Undo/redo capabilities
  - Clear error messages with recovery guidance
  - Default values to reduce input errors
- **Example:** Auto-save in word processors prevents data loss from crashes. "Are you sure?" dialogs before permanent deletions.

### 3.7 When All Else Fail, Standardize

When design cannot eliminate the need for users to learn new patterns, standardize the approach so that at least users can transfer knowledge from other systems.

- **Explanation:** If a truly unique solution is required, use standard conventions from other systems so users can apply existing knowledge. Standards reduce learning time.
- **Key aspects:**
  - Follow platform guidelines (Material Design, HIG)
  - Use standard icons and terminology
  - Adopt industry-standard keyboard shortcuts
  - Leverage existing mental models
- **Example:** Using a floppy disk icon for "Save" is a standard that persists even though floppy disks are obsolete, because users recognize it.

### Exam Tips — Norman's Principles

- **Understand the Gulfs:** The Gulf of Execution (how do I do it?) and Gulf of Evaluation (what happened?) are central to Norman's framework.
- **Mapping ≠ Constraints:** Mapping is about relationship between controls and effects; constraints are about limiting possible actions.
- **Error design is about recovery:** Norman emphasizes designing FOR error (handling), not just preventing errors.
- **Mnemonic:** **K**nowledge **S**implification **V**isibility **M**apping **C**onstraints **E**rror **S**tandardize.
- **Apply to analysis:** When evaluating a UI, identify each gulf and each principle.

---

## 4. ISO 9241 Usability Definition

*ISO 9241-11 defines usability as the extent to which a product can be used by specified users to achieve specified goals with effectiveness, efficiency, and satisfaction in a specified context of use.*

### Three Components of Usability

| Component | Definition | How Measured |
|-----------|-----------|--------------|
| **Effectiveness** | The accuracy and completeness with which users achieve their goals | Success rate, error rate, completion rate |
| **Efficiency** | The resources expended in relation to the accuracy and completeness of goals achieved | Time on task, number of clicks, steps to completion |
| **Satisfaction** | The freedom from discomfort and positive attitudes towards the use of the product | Likert scales, SUS scores, user surveys (CSAT, NPS) |

### Key Concepts

- **Effectiveness** answers: *Can users accomplish their goals?*
- **Efficiency** answers: *How much effort does it take?*
- **Satisfaction** answers: *How do users feel about the experience?*

### Context of Use

Usability is not absolute — it depends on:
- **Users:** Who are they? What are their skills, experience, and needs?
- **Tasks:** What are they trying to accomplish?
- **Equipment:** What hardware/software are they using?
- **Environment:** Where and under what conditions are they using the product?

### Example Applications

| Scenario | Effectiveness | Efficiency | Satisfaction |
|----------|--------------|------------|-------------|
| Online banking | Can the user complete a transfer? | How many clicks/steps? | Is the experience pleasant? |
| Mobile app | Can the user find a restaurant? | How long does it take? | Does the user enjoy the app? |
| ATM machine | Can the user withdraw cash? | How many button presses? | Is the interface confusing? |

### Relationship Between Components

- High effectiveness + low efficiency = Task accomplished but frustratingly slow
- High efficiency + low effectiveness = Fast but wrong/incomplete results
- Both high + low satisfaction = Functional but unpleasant to use
- All three high = Good usability

### Exam Tips — ISO 9241

- **All three dimensions must be considered:** Usability is not just about one factor.
- **Context matters:** The same system may have different usability in different contexts.
- **Measurable:** Each dimension has specific metrics (time, success rate, satisfaction scores).
- **Related to UX but broader:** ISO 9241 focuses on task-oriented usability; UX includes broader emotional/experiential aspects.

---

## 5. Principles of Usability (Chapter 7)

*These principles organize usability into three categories: Learnability, Flexibility, and Robustness.*

### 5.1 Learnability Principles

*How easily can new users accomplish basic tasks the first time?*

| Principle | Definition | Design Implication |
|-----------|-----------|-------------------|
| **Predictability** | The user can determine what will happen before performing an action | Clear labels, previews, consistent behavior |
| **Synthesizability** | The user can assess the effect of past actions on future interactions | Feedback after each action, visible state changes |
| **Familiarity** | How much prior knowledge applies to new situations | Leverage real-world metaphors, standard conventions |
| **Generalizability** | How much knowledge from one interaction applies to others | Consistent patterns, learnable component behaviors |
| **Consistency** | Similar operations and similar terminology are used throughout | Standardize UI elements, terminology, and workflows |

#### Detailed Explanations

**Predictability**
- Users should be able to anticipate outcomes before acting
- Provide clear labels, icons, and descriptions
- Show previews where possible (e.g., print preview, link previews)
- Example: Hovering over a button shows a tooltip describing what it does

**Synthesizability**
- Users need to understand how their actions affect the system state
- Provide immediate, visible feedback for every action
- Show state changes (loading indicators, progress bars, animation)
- Example: A toggle switch visually changes between on/off states

**Familiarity**
- Leverage what users already know from other systems and the real world
- Use standard icons (gear = settings, house = home)
- Follow platform conventions
- Example: Swipe down to refresh on mobile (matches physical gesture of pulling)

**Generalizability**
- Knowledge learned in one part of the system should transfer to others
- Consistent component behavior across the application
- Learnable interaction patterns
- Example: Once you learn to use a dropdown in one form, you can use all dropdowns

**Consistency**
- Internal consistency: Same app, same patterns
- External consistency: Follow industry/platform standards
- Consistent placement, color coding, terminology
- Example: Red always means "delete" or "danger" throughout the application

### 5.2 Flexibility Principles

*How efficiently can expert users accomplish tasks?*

| Principle | Definition | Design Implication |
|-----------|-----------|-------------------|
| **Dialogue initiative** | The user controls the pace and sequence of interaction | User-driven workflows, no forced sequences |
| **Multithreading** | The user can perform multiple tasks simultaneously | Parallel workflows, split views, multi-window support |
| **Task migratability** | The user can transfer control between manual and automatic execution | Manual overrides, customizable automation |
| **Substitutivity** | The user can use alternative methods to accomplish the same task | Multiple input modalities (voice, touch, keyboard) |
| **Customizability** | The user can modify the interface and interaction to suit their needs | Personalization options, configurable shortcuts |

#### Detailed Explanations

**Dialogue Initiative**
- The system should not force a particular sequence of actions
- Users should be able to jump between tasks
- Provide flexible navigation
- Example: Web browsers allow tab switching mid-browsing; users aren't locked into sequential page loading

**Multithreading**
- Support multiple concurrent activities
- Allow users to switch between tasks without losing progress
- Provide background processing while user works on other tasks
- Example: Video editing software renders in the background while the user edits another clip

**Task Migratability**
- Allow users to shift between manual and automated control
- Provide automatic options with manual override capability
- Example: Spell check runs automatically, but users can manually correct or override suggestions

**Substitutivity**
- Allow equivalent input/output methods
- Support voice, touch, keyboard, and mouse
- Example: A search box can be accessed via typing, voice command, or barcode scanner

**Customizability**
- Let users tailor the interface to their preferences
- Configurable layouts, themes, shortcuts
- Example: IDE settings allow custom keybindings, themes, and panel arrangements

### 5.3 Robustness Principles

*How well does the system handle errors and diverse user needs?*

| Principle | Definition | Design Implication |
|-----------|-----------|-------------------|
| **Observability** | The user can evaluate the internal state of the system from its displays | Visible status, progress indicators, system feedback |
| **Recoverability** | The user can correct errors and undo actions | Undo/redo, error recovery, backup/restore |
| **Responsiveness** | The system responds to user actions within acceptable time limits | Performance optimization, loading indicators, perceived speed |
| **Task conformance** | The system supports the activities required by users in their work | Task-aligned workflows, domain-appropriate features |

#### Detailed Explanations

**Observability**
- Users should always know what the system is doing
- Display system status, progress, and state changes
- Provide meaningful feedback for all operations
- Example: A file upload shows a progress bar with percentage and estimated time remaining

**Recoverability**
- Users must be able to recover from errors and mistakes
- Provide undo/redo at multiple levels
- Allow correction of inputs without starting over
- Example: Gmail's "Undo Send" allows recall of sent emails within a window

**Responsiveness**
- The system should respond quickly to user input
- Provide feedback within 0.1 seconds for direct manipulation
- Use loading indicators for operations > 1 second
- Optimize perceived performance (skeleton screens, progressive loading)
- Example: Google Search provides instant results as you type

**Task Conformance**
- The system should support real-world tasks users need to accomplish
- Align system capabilities with user workflows
- Avoid forcing users into unnatural interaction patterns
- Example: Project management tools (Jira, Trello) mirror real project workflows (to-do → in progress → done)

### Exam Tips — Chapter 7 Principles

- **Three categories, 13 principles:** Learnability (5), Flexibility (5), Robustness (4 — note: some sources list 4, verify with your textbook).
- **Each category has a clear focus:** Learnability = new users; Flexibility = efficiency for all; Robustness = error handling and reliability.
- **Memorize definitions:** Each principle has a precise definition and specific design implication.
- **Apply to scenarios:** Be ready to identify which principles are violated in given interfaces.
- **Mnemonic for Learnability:** **P**redict **S**ynthesize **F**amiliarize **G**eneralize **C**onsistently.
- **Mnemonic for Flexibility:** **D**ialogue **M**ultithreads **T**asks **S**ubstitute **C**ustomize.
- **Mnemonic for Robustness:** **O**bserve **R**ecover **R**espond **T**ask.

---

## 6. Gestalt Principles

*Gestalt principles describe how humans visually organize and perceive elements as unified wholes rather than separate parts.*

### 6.1 Proximity

Elements that are close together are perceived as a group, while elements that are farther apart are perceived as separate.

- **Explanation:** Spatial proximity creates a perceived relationship between elements. The mind groups nearby objects together.
- **Design application:**
  - Group related form fields together with spacing
  - Separate unrelated navigation items with whitespace
  - Group related content in card layouts
  - Use padding and margins to indicate relationships
- **Examples:**
  - Form labels placed close to their input fields
  - Menu items grouped by category with visual separation between groups
  - Contact lists showing name, phone, and email close together per contact
- **Violation:** A form where all labels and inputs are equally spaced with no visual grouping — users cannot tell which label belongs to which input.

### 6.2 Similarity

Elements that share visual characteristics (color, shape, size, texture) are perceived as related, while different-looking elements are perceived as different.

- **Explanation:** The mind groups similar elements together based on shared visual properties.
- **Design application:**
  - Use consistent button styles for the same type of action
  - Color-code related elements (e.g., all error states in red)
  - Use consistent iconography for similar functions
  - Differentiate action types through visual variation
- **Examples:**
  - All clickable links in blue underlined text
  - Warning messages consistently styled with yellow backgrounds
  - Related navigation items sharing the same icon style
  - Different card types (article, video, event) having distinct visual treatments
- **Violation:** Using green for "save," blue for "delete," and red for "cancel" — breaks the similarity expectation for primary actions.

### 6.3 Closure

The mind tends to complete incomplete shapes and figures to perceive a whole object, even when parts are missing.

- **Explanation:** Our brains fill in gaps to perceive complete objects. We prefer complete, whole figures over incomplete ones.
- **Design application:**
  - Logo design using partial shapes that the mind completes (e.g., WWF panda)
  - Progress indicators that form a complete circle
  - Icon design that implies completeness through partial shapes
  - Visual continuity in layout design
- **Examples:**
  - The WWF panda logo (partial outline completed by the mind)
  - Loading spinners where a partial arc implies a full circle
  - The FedEx arrow (hidden arrow formed by negative space closure)
  - Timeline indicators where dots imply a complete path

### 6.4 Continuity

The eye follows lines, curves, and patterns. Elements arranged along a line or curve are perceived as more related than elements not aligned.

- **Explanation:** The mind prefers smooth, continuous paths and follows them naturally. Aligned elements create visual flow.
- **Design application:**
  - Use alignment to create visual flow through content
  - Stepper/wizard designs showing progression along a line
  - Scrollable content arranged along a clear visual path
  - Navigation flows following natural reading patterns
- **Examples:**
  - Timeline visualizations where events follow a continuous line
  - Multi-step forms where the active step is highlighted along a horizontal line
  - Charts and graphs where data points connect along a smooth curve
  - Reading flow in left-to-right layouts following natural eye movement

### Other Gestalt Principles (Supplementary)

| Principle | Description | Example |
|-----------|-------------|---------|
| **Figure-Ground** | The eye separates objects (figure) from their background (ground) | Modal dialogs appearing over a dimmed background |
| **Common Region** | Elements within a shared boundary are perceived as a group | Cards with borders grouping related content |
| **Synchrony** | Elements moving together are perceived as a unit | Animated menu items transitioning simultaneously |
| **Parallelism** | Parallel elements are perceived as similar | Parallel lines in charts indicating related data |

### Exam Tips — Gestalt Principles

- **Four core principles:** Proximity, Similarity, Closure, Continuity (minimum for exams).
- **Apply to visual analysis:** Examine screenshots and identify which Gestalt principles are used or violated.
- **Proximity vs. Similarity:** Proximity = spacing/grouping; Similarity = shared visual properties.
- **Closure is about completion:** The mind fills in gaps; logos and icons leverage this.
- **Continuity creates flow:** Aligned elements guide the eye naturally.
- **Common in every UI:** Every well-designed interface uses Gestalt principles — be ready to point them out.

---

## 7. Fitts' Law

*Fitts' Law is a predictive model of human movement that predicts the time required to move to a target area, as a function of the distance to the target and the size of the target.*

### Formula

```
Mt = a + b × log₂(D/S + 1)
```

Where:
- **Mt** = Movement time (time to reach the target)
- **a** = Intercept time (startup time, device-specific constant)
- **b** = Slope (speed of the device/controller)
- **D** = Distance from the starting point to the center of the target
- **S** = Width (size) of the target in the direction of movement
- **log₂(D/S + 1)** = Index of Difficulty (ID), measured in bits

### Key Insights

1. **Larger targets are faster to hit:** Increasing S (size) reduces Mt
2. **Shorter distances are faster:** Decreasing D (distance) reduces Mt
3. **The relationship is logarithmic:** Doubling the target size doesn't halve the time — the gain diminishes
4. **Edge and corner targets are infinite:** Screen edges and corners have effectively infinite size in one direction (cursor stops at the edge)

### Design Implications

| Implication | Application |
|------------|------------|
| **Make important targets large** | Primary action buttons should be large and prominent |
| **Place frequent targets near the cursor** | Context menus appear near the mouse position |
| **Use screen edges and corners** | Windows taskbar (bottom edge), macOS menu bar (top edge) |
| **Avoid small, distant targets** | Tiny links far from the cursor are slow to reach |
| **Consider touch targets** | Mobile buttons need minimum 44×44px (Apple) or 48×48dp (Android) |
| **Reduce unnecessary movement** | Place related controls close together |

### Examples

- **Screen corners:** The macOS Dock at the bottom uses screen edge (infinite target size). The "hot corners" feature in macOS leverages this — moving to a corner is very fast.
- **Right-click context menus:** Appear exactly where the cursor is, minimizing D to zero.
- **Large buttons in touch interfaces:** Mobile navigation buttons are large (high S) and positioned at the bottom (low D for thumb reach).
- **Avoid "fat finger" problems:** Small, closely spaced buttons on mobile cause accidental taps.

### Index of Difficulty (ID)

```
ID = log₂(D/S + 1)    [in bits]
```

- Higher ID = more difficult movement
- Lower ID = easier movement
- ID = 0 when D = 0 (target is at the starting point)

### Throughput

```
TP = ID / Mt    [in bits/second]
```

- Throughput measures human performance efficiency
- Higher throughput = better performance
- Useful for comparing input devices

### Exam Tips — Fitts' Law

- **Memorize the formula:** Mt = a + b × log₂(D/S + 1) — understand each variable.
- **Know the implications:** Larger targets, shorter distances → faster movement.
- **Application questions:** Given a UI, identify how Fitts' Law applies and suggest improvements.
- **Edge/corner targets:** The infinite target size of screen edges is a key concept.
- **Touch considerations:** Mobile design must account for finger size (larger S needed).
- **Limitations:** Fitts' Law predicts movement time, not accuracy; it assumes point-to-point movement.
- **Related to Fitts' Law:** Hick's Law (decision time increases with choices) and Miller's Law (7±2 items) are often tested together.

---

## 8. Norman's 7 Stages of Action

*Don Norman's model describes the cyclic process users go through when interacting with a system, organized as a "Gulf of Execution" and "Gulf of Evaluation."*

### The Seven Stages

```
Goal → Intention → Specify → Execute → Perceive → Interpret → Evaluate
        ──────────────────────          ──────────────────────────
              GULF OF EXECUTION              GULF OF EVALUATION
```

### Stage-by-Stage Explanation

| Stage | Question | Description |
|-------|----------|-------------|
| **1. Goal** | What do I want to accomplish? | The user forms an objective or desired state |
| **2. Intention** | What kind of action should I take? | The user decides on a general approach to achieve the goal |
| **3. Specify** | What specific action do I perform? | The user determines the precise action sequence |
| **4. Execute** | How do I do it? | The user physically performs the action |
| **5. Perceive** | What happened? | The user observes the system's response |
| **6. Interpret** | What does it mean? | The user makes sense of the observed state |
| **7. Evaluate** | Did it match my goal? | The user compares the outcome with the original goal |

### The Two Gulfs

**Gulf of Execution** (Stages 2–4: from intention to action)
- The gap between what the user wants to do and how the system allows it
- Bridged by: Clear affordances, visible controls, natural mappings, constraints

**Gulf of Evaluation** (Stages 5–7: from action to understanding)
- The gap between the system's output and the user's understanding
- Bridged by: Feedback, visibility of system status, clear status indicators, natural mappings

### Detailed Breakdown

**Goal (Stage 1)**
- The user has a desire or objective
- Goals are typically vague ("I want to find a good restaurant")
- Design implication: Help users clarify goals through suggestions, filters, categories

**Intention (Stage 2)**
- The user forms a plan to achieve the goal
- Intention is more specific than goal ("I'll search for Italian restaurants nearby")
- Design implication: Provide intuitive pathways to common goals

**Specify (Stage 3)**
- The user determines the exact steps needed
- Requires knowledge of the system's capabilities
- Design implication: Clear action options, logical workflow sequences

**Execute (Stage 4)**
- The user performs the action
- Involves physical interaction with the interface
- Design implication: Easy-to-use controls, appropriate input methods, minimal steps

**Perceive (Stage 5)**
- The user observes the system's response
- Requires the system to provide visible feedback
- Design implication: Immediate, clear, proportional feedback

**Interpret (Stage 6)**
- The user makes sense of what they observed
- Requires understanding the relationship between action and result
- Design implication: Clear, meaningful feedback; avoid ambiguous responses

**Evaluate (Stage 7)**
- The user compares the outcome to the original goal
- Determines if the goal was achieved or if more action is needed
- Design implication: Clear indication of completion; allow easy course correction

### Example: Sending an Email

| Stage | User Action |
|-------|------------|
| Goal | "I need to tell my colleague about the meeting" |
| Intention | "I'll send an email" |
| Specify | "I'll click 'Compose,' type their address, write the message, click 'Send'" |
| Execute | Opens email client, types address, writes message, clicks Send |
| Perceive | Sees "Sending..." then "Message sent" confirmation |
| Interpret | Understands that the email was successfully delivered |
| Evaluate | Confirms goal achieved — colleague will receive the message |

### Design Guidelines for Each Stage

| Stage | Design Principle |
|-------|-----------------|
| Goal | Help users formulate clear goals (search suggestions, guided flows) |
| Intention | Provide clear action options that match common intentions |
| Specify | Make action sequences clear and logical |
| Execute | Ensure controls are usable and accessible |
| Perceive | Provide immediate, visible feedback |
| Interpret | Use clear, unambiguous feedback language |
| Evaluate | Show completion status; indicate success or failure clearly |

### Exam Tips — Norman's Stages

- **Memorize all 7 stages in order:** Goal → Intention → Specify → Execute → Perceive → Interpret → Evaluate.
- **Identify the two Gulfs:** Execution (doing) and Evaluation (understanding).
- **Map stages to design:** For each stage, identify what design feature bridges it.
- **Apply to scenarios:** Given an interaction scenario, break it down into the 7 stages.
- **Cyclic nature:** After evaluation, the user may form a new goal or revise the current one — the cycle continues.
- **Relation to other frameworks:** The Gulfs align with Nielsen's "Visibility of System Status" and "Feedback" principles.

---

## Quick Reference: Cross-Framework Comparisons

| Theme | Nielsen | Shneiderman | Norman | ISO 9241 |
|-------|---------|-------------|--------|----------|
| **Feedback** | #1 Visibility of system status | #3 Informative feedback | Bridge Gulf of Evaluation | Effectiveness |
| **Consistency** | #4 Consistency and standards | #1 Strive for consistency | #7 Standardize | — |
| **Error handling** | #5 Error prevention, #9 Recovery | #5 Error prevention | #6 Design for error | Effectiveness, Satisfaction |
| **User control** | #3 User control and freedom | #6 Permit easy reversal | #1 Knowledge in world/head | Efficiency |
| **Simplicity** | #8 Aesthetic/minimalist | #8 Reduce memory load | #2 Simplify structure | Efficiency |
| **Learnability** | #6 Recognition over recall | #2 Shortcuts | #5 Exploit constraints | — |
| **Visibility** | #1 Visibility of system status | #3 Informative feedback | #3 Make things visible | — |

---

## Study Checklist

- [ ] Can list and explain all 10 Nielsen heuristics with examples
- [ ] Can list and explain all 8 Shneiderman golden rules
- [ ] Can list and explain all 7 Norman design principles
- [ ] Can define usability per ISO 9241 (effectiveness, efficiency, satisfaction)
- [ ] Can explain all 13 Chapter 7 principles across three categories
- [ ] Can identify and apply 4 core Gestalt principles
- [ ] Can write and explain Fitts' Law formula and implications
- [ ] Can describe all 7 stages of Norman's action model
- [ ] Can compare across frameworks and identify overlaps
- [ ] Can apply principles to evaluate real-world interfaces

---

*Last updated: 2026-06-03*
