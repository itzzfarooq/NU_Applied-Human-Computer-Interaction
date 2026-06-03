Course: Applied Human-Computer Interaction

Objective

Transform the provided course materials into a high-efficiency exam preparation system optimized for a final exam occurring tomorrow.

Source Materials

All source materials are located in:

/resources

This directory contains:

* Lecture slides
* Reference textbook
* Any supplementary course material relevant to the syllabus

Scope

Only cover syllabus content corresponding to Chapters 1 through 9.

Ignore material beyond Chapter 9 unless it is required to understand concepts that appear within Chapters 1–9.

Priorities

Optimize for:

1. Coverage completeness
2. Exam relevance
3. Active recall
4. Retrieval speed
5. Identification of subtle concepts
6. Identification of common misconceptions and exam traps

Process Requirements

Before generating any study artifacts:

1. Analyze all materials in /resources.
2. Extract and organize all topics covered in Chapters 1–9.
3. Construct a complete topic hierarchy.
4. Cross-reference lecture slides and textbook coverage.
5. Identify:

   * Core concepts
   * Repeated themes
   * Foundational ideas
   * Frequently emphasized topics
   * Terminology likely to appear in exams
6. Verify that no syllabus topic has been omitted.

Artifact Generation

Create all outputs inside:

/generated

Required Deliverables

1. /generated/01_knowledge_map.md

A hierarchical map of all concepts and topics covered in Chapters 1–9.

2. /generated/02_topic_priority_matrix.md

A prioritization matrix containing:

* Topic
* Importance
* Difficulty
* Exam risk
* Recommended study priority

3. /generated/03_concept_sheets/

One concept sheet per major topic containing:

* Definition
* Purpose
* Key principles
* Relationships to other concepts
* Common mistakes
* Exam-focused notes

4. /generated/04_active_recall_bank.md

A comprehensive active-recall question bank covering all examinable content.

Questions should include:

* Definitions
* Comparisons
* Applications
* Scenario-based reasoning
* Conceptual understanding

5. /generated/05_worked_examples.md

Worked examples and case analyses relevant to Applied Human-Computer Interaction.

Focus on:

* Design evaluation
* Usability analysis
* Human factors reasoning
* Interface critique
* Scenario-based problem solving

6. /generated/06_confusion_map.md

Commonly confused concepts, including:

* Similar terminology
* Contrasting theories
* Frequent student mistakes
* Exam traps

7. /generated/07_reference_sheet.md

A compressed reference document containing:

* Key definitions
* Models
* Frameworks
* Principles
* Terminology
* High-yield comparisons

8. /generated/08_final_rapid_review.md

A high-density review sheet intended for use during the final 30–60 minutes before the exam.

Include only the most important material.

9. /generated/09_coverage_checklist.md

A checklist verifying complete coverage of all topics from Chapters 1–9.


10. /generated/10_chapter_notes/

Create one file per chapter:

/generated/10_chapter_notes/ch01.md
/generated/10_chapter_notes/ch02.md
...
/generated/10_chapter_notes/ch09.md

With a required structure:

- Chapter Overview
- Learning Objectives
- Core Concepts
- Key Definitions
- Important Models / Frameworks / Principles
- Detailed Explanations
- Relationships to Other Topics
- Examples and Applications
- Common Misconceptions
- Frequently Confused Concepts
- Potential Exam Questions
- Active Recall Questions
- Chapter Summary

Quality Requirements

* Maximize exam performance per hour studied.
* Prefer compressed, high-signal content over lengthy explanations.
* Favor retrieval-oriented formats over passive summaries.
* Preserve important details, nuances, and subtle distinctions.
* Explicitly identify likely exam traps and misconceptions.
* Maintain consistency between all generated artifacts.

Epistemic Constraints

* Do not invent content not supported by the provided materials.
* Do not assume topics are examinable unless supported by the course materials.
* When uncertainty exists, explicitly label it.
* If slides and textbook disagree, document the discrepancy.

Chapter Notes Requirements

- Serve as the primary learning resource.
- Be comprehensive enough that a student could learn the chapter from the notes alone.
- Preserve important nuances, caveats, and instructor-emphasized details.
- Include examples whenever helpful.
- Highlight concepts likely to appear in examinations.
- Explicitly connect related concepts across chapters.
- Prefer structured explanations over long prose.
- Use tables where comparisons improve clarity.

Success Criterion

A student should be able to study only the contents of /generated and achieve comprehensive, exam-focused coverage of all material from Chapters 1–9 with minimal wasted effort.

Focus on extraction and emphasize **definitions, models, principles, heuristics, comparisons between frameworks, usability concepts, design methodologies, and case-study reasoning**, since HCI exams are often more conceptual than computational.
