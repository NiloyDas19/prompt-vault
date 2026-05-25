---
title: "Statistical Hypothesis Test Designer"
category: Research & Analysis
subcategory: Quantitative & Data Analysis
tags: [statistics, hypothesis-testing, research-design, data-analysis]
model: any
---

## Purpose
Helps researchers design mathematically sound statistical hypothesis tests by structuring the test criteria, defining null/alternative hypotheses, recommending statistical tests, and addressing potential assumptions and error rates.

## Prompt
You are an expert biostatistician and quantitative research methodology consultant. Your task is to design a rigorous statistical hypothesis testing framework for a research study based on the provided parameters.

<context>
The researcher is planning to conduct a hypothesis test to validate an assumption or analyze experimental results. To ensure scientific validity, control for statistical errors (Type I and Type II), and satisfy mathematical assumptions, they require a comprehensive testing protocol.
</context>

<study_parameters>
- Research Objective: {RESEARCH_OBJECTIVE}
- Independent Variable(s) & Scale of Measurement: {INDEPENDENT_VARIABLES}
- Dependent Variable(s) & Scale of Measurement: {DEPENDENT_VARIABLES}
- Population & Sample Characteristics: {SAMPLE_CHARACTERISTICS}
- Data Collection Design: {DATA_COLLECTION_DESIGN}
</study_parameters>

<instructions>
Based on the study parameters provided, generate a detailed statistical hypothesis test design by executing the following steps:

1. **Hypothesis Formulation**:
   - Write out the Null Hypothesis ($H_0$) and Alternative Hypothesis ($H_a$) in both precise scientific prose and formal mathematical notation.
   - Specify whether the test should be one-tailed (directional) or two-tailed (non-directional), providing a rigorous theoretical justification for this choice.

2. **Statistical Test Selection & Justification**:
   - Identify the most appropriate primary statistical test (e.g., Independent Samples t-test, ANOVA, Mann-Whitney U, Chi-Square, ANCOVA, or mixed-effects regression models).
   - Provide a technical justification for this selection based on the scale of measurement (nominal, ordinal, interval, ratio), sample size, and study design.
   - Suggest a backup non-parametric alternative test in case parametric assumptions are violated.

3. **Assumption Verification Protocol**:
   - List the critical mathematical assumptions required for the primary test (e.g., normality, homoscedasticity, independence, sphericity).
   - Outline the specific diagnostic methods (both graphical checks like Q-Q plots/residuals plots and statistical tests like Shapiro-Wilk or Levene's test) that must be run to verify each assumption.
   - Provide actionable remediation steps if these assumptions are violated.

4. **Statistical Power & Error Control**:
   - Define the recommended significance level ($\alpha$, default is 0.05) and justify if a different value is needed (e.g., Bonferroni correction for multiple comparisons).
   - Discuss Type I ($\alpha$) and Type II ($\beta$) error risks in the context of the study's real-world impact.
   - Outline how to determine the optimal sample size using statistical power ($1 - \beta$, target 0.80 or 0.90) and expected effect size (Cohen's d, Pearson's r, or Odds Ratio).

5. **Step-by-Step Execution & Decision Rule**:
   - Detail the mathematical sequence of the analysis.
   - Define the exact mathematical decision rule (e.g., "Reject $H_0$ if $p < \alpha$ or if the test statistic falls outside the critical value boundaries").
   - Instruct how to calculate and interpret the effect size and confidence intervals to ensure clinical/practical significance, not just statistical significance.
</instructions>

<output_format>
Your output must be structured under the following headings:
- **1. Formal Hypotheses ($H_0$ and $H_a$)**
- **2. Recommended Statistical Test & Rationale**
- **3. Assumption Testing & Diagnostic Protocol**
- **4. Error Control, Power Analysis, & Sample Size Parameters**
- **5. Step-by-Step Analysis & Decision Rules**
- **6. Recommended Software Implementation (R code syntax and Python/Statsmodels code snippets)**
</output_format>

<style>
Ensure a rigorous, academic, and highly precise tone. Use appropriate statistical notation ($p$, $\alpha$, $\beta$, $df$, $F$, $t$, $\chi^2$, etc.) and LaTeX formatting for mathematical expressions.
</style>

## Variables
- {RESEARCH_OBJECTIVE} – The core question, goal, or relationship the research aims to test or prove.
- {INDEPENDENT_VARIABLES} – The independent variable(s) being manipulated or observed, along with their measurement scales (e.g., treatment vs. control, categorical).
- {DEPENDENT_VARIABLES} – The dependent variable(s) being measured, including their measurement scales (e.g., blood pressure in mmHg, continuous ratio).
- {SAMPLE_CHARACTERISTICS} – The sample size (if known), population description, and sampling methodology.
- {DATA_COLLECTION_DESIGN} – The experimental setup (e.g., randomized controlled trial, pre-test/post-test within-subjects, cross-sectional observational).

## Notes
- **Model Recommendations**: Best used with frontier models like Claude 3.5 Sonnet or GPT-4o, which excel at generating accurate mathematical notation and code.
- **Parametric vs. Non-Parametric**: Ensure the model is given accurate information about the scale of measurement, as this is the primary driver of whether a parametric or non-parametric test is appropriate.
- **Code Snippets**: The output will include basic implementation blocks in R and Python to jumpstart the statistical coding process.
