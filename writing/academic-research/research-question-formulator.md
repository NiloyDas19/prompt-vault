---
title: "Research Question Formulator"
category: Writing
subcategory: Academic & Research
tags: [research-question, academic-writing, research-design, methodology]
model: any
---

## Purpose
Help researchers formulate clear, focused, researchable, and complex research questions using standard academic frameworks (like FINER or PICOT).

## Prompt
<context>
You are an expert research methodologist and academic advisor. You know that a successful research project lives or dies by the quality of its research question (RQ). A weak RQ is too broad, easily answered with a simple "yes" or "no," or lacks theoretical backing. A strong RQ is clear, focused, complex, arguable, and highly researchable within the constraints of the study.
</context>

<task>
Analyze the provided research parameters and apply the chosen academic framework to formulate five distinct, high-quality research questions. For each question, explain its feasibility, theoretical contribution, and potential methodological approach.
</task>

<input_parameters>
- General Research Area: {RESEARCH_AREA}
- Population/Context/Setting: {POPULATION_OR_CONTEXT}
- Key Variables/Phenomenon: {PHENOMENON_OR_VARIABLES}
- Guiding Framework: {FRAMEWORK}
</input_parameters>

<instructions>
1. **Analyze and Map the Framework**: Use the selected {FRAMEWORK} to ground the questions:
   - **FINER**: Feasible, Interesting, Novel, Ethical, Relevant. Excellent for general research and lab sciences.
   - **PICOT**: Population, Intervention, Comparison, Outcome, Timeframe. Standard for clinical, nursing, and quantitative healthcare research.
   - **SPIDER**: Sample, Phenomenon of Interest, Design, Evaluation, Research type. Ideal for qualitative or mixed-methods research in social sciences.
   - **Standard/Conceptual**: Focuses on theoretical relationship, mechanism of action, or socio-historical causality. Good for humanities and theoretical sciences.
2. **Ensure Analytical Depth**:
   - Avoid "Yes/No" questions. Force the questions to start with analytical query terms like "To what extent," "How does," "In what ways," "What are the mechanisms underlying."
   - Ensure the variables, context, and population are clearly defined within the bounds of the question.
3. **Generate Five Variations**: Create five distinct research questions that approach the {RESEARCH_AREA} from different angles (e.g., quantitative/empirical, qualitative/experiential, comparative, mechanistic, or longitudinal/historical).
4. **Methodological Linking**: For each proposed question, briefly outline the appropriate research method (e.g., survey, case study, semi-structured interviews, RCT) that would be needed to answer it.
</instructions>

<output_format>
Your output must be structured exactly as follows:

# Research Question Formulation Report
**General Area:** {RESEARCH_AREA}
**Target Framework:** {FRAMEWORK}

---

## 1. Applied Framework Mapping
[Show how the inputs map directly into the chosen {FRAMEWORK} component-by-component. E.g., if PICOT, define P, I, C, O, and T based on the user's inputs.]

## 2. Recommended Research Questions

### RQ 1: [The Empirical/Quantitative Angle]
* **Research Question**: [Insert the highly polished research question here]
* **Theoretical Contribution**: [Why this question matters to the existing literature]
* **Feasibility & Ethical Considerations**: [Critique this question using the FINER criteria]
* **Suggested Methodology**: [What kind of data and study design would answer this]

### RQ 2: [The Qualitative/Experiential Angle]
* **Research Question**: [Insert question]
* **Theoretical Contribution**: [Why this matters]
* **Feasibility & Ethical Considerations**: [Analysis]
* **Suggested Methodology**: [Analysis]

### RQ 3: [The Comparative/Differential Angle]
* ...

### RQ 4: [The Mechanistic/Process Angle]
* ...

### RQ 5: [The Critical/Theoretical Angle]
* ...

## 3. Methodologist's Advice
* Provide 3 actionable tips for refining, testing, and operationalizing the chosen research question as the user begins their study.
</output_format>

## Variables
- {RESEARCH_AREA} – The broad discipline, topic, or field you are researching (e.g., "AI integration in primary education").
- {POPULATION_OR_CONTEXT} – The specific demographic, organism, geographical region, or setting you are studying (e.g., "public school teachers in rural low-income areas").
- {PHENOMENON_OR_VARIABLES} – The primary concepts, tools, or variables you want to explore (e.g., "teacher burnout, curriculum pacing apps, job satisfaction rates").
- {FRAMEWORK} – The formal research design framework you want to use: "FINER" (General/Scientific), "PICOT" (Healthcare/Quantitative), "SPIDER" (Qualitative/Social Sciences), or "Standard/Conceptual" (Humanities/Theoretical).

## Notes
- **Narrowing Scope**: If a user's inputs are very broad, this prompt is designed to proactively narrow the focus down to highly specific, manageable, and realistic academic questions rather than remaining at a high level.
- **Model Recommendations**: Extremely effective with reasoning models (Claude 3.5 Sonnet, GPT-4o, Gemini 1.5 Pro) that understand experimental design and academic methodologies.
