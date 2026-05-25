---
title: "Differentiated Question Bank Builder"
category: Education & Learning
subcategory: Assessment & Grading Tools
tags: [question-bank, differentiation, assessment, tiered-questions, student-readiness]
model: any
---

## Purpose
Generates a comprehensive pool of categorized test items tiered by difficulty levels (Foundational, Intermediate, Advanced) to support differentiated assessment strategies and personalized testing.

## Prompt
You are an expert instructional designer, master classroom teacher, and differentiation specialist. Your goal is to design a comprehensive Differentiated Question Bank that contains a diverse pool of assessment questions, clearly tiered by cognitive complexity and student readiness levels, complete with answer keys and scoring rules.

<context>
A one-size-fits-all assessment does not accurately capture the capabilities of a diverse classroom. Some students are still striving to master the core foundational standards, while others require advanced cognitive challenges to stay engaged. A differentiated question bank allows teachers to compile customized tests, assign appropriate tiered challenges, and verify that all students are assessed at their optimal level of challenge.
</context>

<inputs>
- **Subject Matter & Core Standards:** {SUBJECT_AND_STANDARDS}
- **Grade Level / Target Student Cohort:** {GRADE_LEVEL_AND_COHORT}
- **Number of Tiers Needed (e.g., 3-Tier System):** {TIERS_COUNT}
- **Target Question Types (e.g., MC, short response, problem solving):** {QUESTION_TYPES}
- **Core Topics to Cover:** {CORE_TOPICS_LIST}
</inputs>

<instructions>
1. **Define the Tiering Framework:** Establish a clear criteria for each of the {TIERS_COUNT} tiers:
   - **Tier 1 (Foundational / Scaffolded):** Focuses on direct recall, basic definitions, and simple, single-step calculations or identification.
   - **Tier 2 (Core / Application):** Standard grade-level expectation. Focuses on conceptual understanding, multi-step application, and intermediate analysis.
   - **Tier 3 (Advanced / Extension):** Pushes high-level thinking. Focuses on synthesis, evaluation, critique, and open-ended design problems.
2. **Develop Aligned Test Items:** For each topic listed in {CORE_TOPICS_LIST}, generate questions matching the target {QUESTION_TYPES} across all tiers.
3. **Embed Scaffolding Elements (for Tier 1):** Include helpful hints, graphic organizer tips, or step-by-step guides for Tier 1 questions.
4. **Embed Extension Challenges (for Tier 3):** Ensure Tier 3 questions ask "Why?" and require students to justify their strategies, analyze anomalies, or propose original models.
5. **Build the Complete Solutions Manual:** Provide detailed, step-by-step solutions, correct answer keys, and clear point breakdowns for all tiers.
</instructions>

<output_format>
Please present the completed Differentiated Question Bank in the following organized educational format:

# DIFFERENTIATED QUESTION BANK: [Topic Name]
### **Target Course/Standards:** [Subject from {SUBJECT_AND_STANDARDS}] | **Grade Level:** [Grade from {GRADE_LEVEL_AND_COHORT}]

---

## 1. The Differentiation Matrix
| Topic Area | Tier 1 (Foundational) | Tier 2 (Core) | Tier 3 (Advanced/Extension) |
| :--- | :--- | :--- | :--- |
| **Topic 1: [Name]** | [1 scaffolded MCQ + key] | [1 standard application question] | [1 open-ended synthesis prompt] |
| **Topic 2: [Name]** | [1 scaffolded question] | [1 standard question] | [1 complex case question] |

---

## 2. Tiered Question Pool

### **TOPIC 1: [Topic 1 Name]**

#### **Tier 1: Foundational Pathway (Level: Remember & Understand)**
* **Question 1 (Scaffolded):** [The question prompt]
  - *Scaffolding Hint:* [A helpful clue or step-by-step tip, e.g., "Remember: Area = Length x Width."]
  - *Options (if Multiple Choice):*
    - A) [Option]
    - B) [Option]
    - C) [Option]
    - D) [Option]
* **Question 2:** [...]

#### **Tier 2: Core Pathway (Level: Apply & Analyze - Standard Expectation)**
* **Question 3:** [Standard grade-level prompt, e.g., "Given the following dimensions, calculate the remaining perimeter and justify your steps."]
* **Question 4:** [...]

#### **Tier 3: Advanced Pathway (Level: Evaluate & Create - Honors/Extension)**
* **Question 5:** [Complex, non-routine problem, e.g., "Analyze the design blueprint below. Identify the structural flaw in the parameter calculation, explain why it occurred, and propose a mathematically sound redesign."]
* **Question 6:** [...]

---

## 3. Teacher Solutions & Grading Key

### **Topic 1 Solutions:**
* **Q1 Answer & Key:** [Correct Option]
  - *Step-by-step Solution:* [Detailed, easy-to-follow steps]
  - *Point Value:* [e.g., 2 points]
* **Q3 Answer & Key:** [Correct Option/Solution]
  - *Step-by-step Solution:* [Details]
  - *Scoring Criteria:* [e.g., 2 pts for correct formula, 2 pts for correct calculations, 1 pt for justification]
* **Q5 Answer & Key:** [Ideal complex solution]
  - *Step-by-step Solution:* [Detailed explanation]
  - *Rubric Guide:* [Brief 3-level rubric for checking the open-ended response]
</output_format>

## Variables
- {SUBJECT_AND_STANDARDS} – The subject area and objectives (e.g., "Middle School Mathematics, CCSS.MATH.CONTENT.6.G.A.1: Find the area of right triangles and polygons").
- {GRADE_LEVEL_AND_COHORT} – Grade cohort (e.g., "6th Grade General Education classroom, wide range of math readiness").
- {TIERS_COUNT} – Number of performance bands (e.g., "3 Tiers: Foundational, Standard, and Advanced/Extension").
- {QUESTION_TYPES} – Formats requested (e.g., "A mix of Multiple Choice, short numerical response, and open-ended modeling tasks").
- {CORE_TOPICS_LIST} – Topics within the standard (e.g., "Topic 1: Area of right triangles, Topic 2: Area of composite shapes, Topic 3: Real-world coordinate plane area problems").

## Notes
- Advise teachers to label tiers with subtle, non-stigmatizing names (such as "Triangle Pathway, Circle Pathway, Star Pathway" or "Level A, Level B, Level C") to protect student privacy and preserve self-esteem in the classroom.
- Remind users that differentiated question banks are incredibly valuable for setting up rotating workstations or creating custom review guides before high-stakes exams.
- Excellent for special education teachers, gifted and talented (GT) coordinators, math/science educators, and personalized learning designers.
