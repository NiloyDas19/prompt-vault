---
title: "Sample Size & Statistical Power Planner"
category: Research & Analysis
subcategory: Quantitative & Data Analysis
tags: [sample-size, statistical-power, research-design, power-analysis]
model: any
---

## Purpose
Helps researchers determine the mathematically optimal sample size needed for a study to ensure sufficient statistical power, control statistical errors, and justify the research budget and timeline.

## Prompt
You are a senior statistical consultant and research design expert. Your task is to develop a comprehensive Sample Size and Statistical Power Plan for a proposed quantitative study, based on the study design, desired error rates, and expected effect size.

<context>
Running a study with too few participants (underpowered) leads to a high probability of Type II errors (failing to detect a real effect). Conversely, oversampling (overpowered) wastes resources, budgets, and raises ethical concerns (e.g., exposing too many human subjects to experimental trials). Calculating the exact sample size needed, factoring in expected attrition and non-compliance, is critical for project planning.
</context>

<study_parameters>
- Statistical Test Type: {STATISTICAL_TEST_TYPE}
- Expected Effect Size (e.g., Cohen's d, f2, w, Pearson's r): {EXPECTED_EFFECT_SIZE}
- Significance Level (Alpha, α): {ALPHA}
- Desired Statistical Power (1 - Beta, 1-β): {TARGET_POWER}
- Expected Attrition/Drop-out Rate (%): {ATTRITION_RATE}
- Allocation Ratio (e.g., Treatment to Control ratio): {ALLOCATION_RATIO}
</study_parameters>

<instructions>
Based on the provided study parameters, construct a rigorous sample size and power planning document. Execute the following steps:

1. **Power Analysis Calculations**:
   - Provide the mathematical formula or algorithm used to estimate the sample size for this specific {STATISTICAL_TEST_TYPE}.
   - Calculate the precise minimum required sample size for an idealized scenario (assuming 100% compliance and zero attrition).
   - If the study is multi-armed, calculate both the sample size required per arm and the total sample size across all arms.

2. **Adjustments for Real-World Factors (Attrition & Design Effects)**:
   - Apply the {ATTRITION_RATE} adjustment using the standard mathematical correction formula: $N_{adjusted} = N / (1 - d)^2$ or $N / (1 - d)$ where $d$ is the drop-out proportion.
   - Adjust the sample size if there is a clustering or design effect (e.g., sampling classrooms, clinics, or zip codes instead of randomized individuals).
   - Provide the final, inflation-adjusted minimum target sample size for recruitment.

3. **Power Curve & Sensitivity Analysis**:
   - Detail a sensitivity analysis showing how the required sample size fluctuates if the expected effect size is smaller or larger than predicted. Offer a 3-tier scenario matrix:
     - Optimistic (Large effect size)
     - Baseline (Expected effect size)
     - Pessimistic (Small effect size)
   - Explain how varying the target power (e.g., from 0.80 to 0.90) impacts the necessary sample size.

4. **Justification & Ethics Statement**:
   - Write a formal, academic-grade "Sample Size Justification" statement that the researcher can directly copy-paste into an IRB (Institutional Review Board) application or grant proposal.
   - Explain why this sample size represents an ethical balance between scientific validity and subject exposure.
</instructions>

<output_format>
Your output must be structured under these markdown headings:
- **1. Mathematical Formula & Model Framework**
- **2. Idealized Sample Size Calculations (No Attrition)**
- **3. Real-World Adjustments (Attrition & Design Effects)**
- **4. Sensitivity Matrix (Effect Size vs. Sample Size Table)**
- **5. Academic Sample Size Justification Statement**
- **6. Executable Implementation Code (Python statsmodels / R pwr package syntax)**
</output_format>

<style>
Maintain a highly technical, rigorous, and advisory tone. Use standard LaTeX notation for mathematical equations and formal scientific terms throughout.
</style>

## Variables
- {STATISTICAL_TEST_TYPE} – The exact test planned (e.g., Two-sample independent t-test, One-way ANOVA with 3 groups, Chi-square test of independence, Multiple linear regression with 5 predictors).
- {EXPECTED_EFFECT_SIZE} – The estimated strength of the relationship (e.g., Cohen's $d = 0.5$ (medium), Pearson's $r = 0.3$, or Odds Ratio $= 2.0$), ideally based on prior pilot studies or literature.
- {ALPHA} – The probability of committing a Type I error (e.g., 0.05, 0.01, 0.005).
- {TARGET_POWER} – The probability of correctly rejecting the null hypothesis when a true effect exists (e.g., 0.80 or 0.90).
- {ATTRITION_RATE} – The expected percentage of subjects who will drop out, lose contact, or fail to complete the study (e.g., 15%, 20%).
- {ALLOCATION_RATIO} – The ratio of sample sizes in different groups (e.g., 1:1 for equal treatment/control groups, 2:1 for unbalanced trials).

## Notes
- **Model Recommendations**: Best used with GPT-4, Gemini 1.5 Pro, or Claude 3.5 Sonnet, as they can accurately perform statistical arithmetic and generate functional code.
- **Reference Values**: If the user is unsure of the effect size, standard benchmarks (Cohen's rules of thumb for small, medium, large effects) should be explicitly detailed by the model in the sensitivity section.
