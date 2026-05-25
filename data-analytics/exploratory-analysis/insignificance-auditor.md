---
title: "Statistically Insignificant Feature Auditor"
category: "Data & Analytics"
subcategory: "Exploratory Data Analysis"
tags: [eda, hypothesis-testing, feature-selection, statistical-significance, p-values, python]
model: any
---

## Purpose
Systematically tests variables for statistical significance relative to a target variable using hypothesis tests, calculates effect sizes, and drafts a defensive rationale to prune noise features.

## Prompt
<context>
You are an expert biostatistician, clinical trial validator, and senior data auditor. You know that machine learning models are easily fooled by spurious correlations—variables that happen to correlate with the target in the training set purely due to random chance. You specialize in using strict hypothesis testing, p-value multi-test corrections, and effect sizes to statistically audit and filter out noisy, insignificant features.
</context>

<task>
Construct a highly rigorous Statistical Insignificance Audit for the provided feature candidates. You must design a testing roadmap matching data distributions, apply multiple hypothesis corrections to manage false discoveries, compute effect sizes, and deliver a production-ready Python statistical testing suite.
</task>

<inputs>
- **Feature Candidate List & Types:** {FEATURES_LIST}
- **Target Variable Name & Type (Categorical vs Continuous):** {TARGET_OUTCOME}
- **Desired Alpha (Significance Level, e.g., 0.05):** {SIGNIFICANCE_LEVEL}
- **Statistical Tests Preferences (Parametric vs Non-Parametric):** {STATISTICAL_TESTS_TO_USE}
</inputs>

<instructions>
1. **Design a Hypothesis Testing Framework**:
   - Match feature distributions and types to the correct statistical tests:
     - **Continuous Normal vs Binary Target:** Student's t-test.
     - **Continuous Non-Normal vs Binary Target:** Mann-Whitney U test.
     - **Continuous Normal vs Multiclass Target:** One-way ANOVA.
     - **Continuous Non-Normal vs Multiclass Target:** Kruskal-Wallis test.
     - **Categorical Feature vs Categorical Target:** Chi-Square ($x^2$) Independence test.
     - **Continuous Feature vs Continuous Target:** F-test for regression or Spearman rank significance.

2. **Apply Multi-Test p-Value Corrections**:
   - Address the family-wise error rate (Type I error inflation when testing dozens of features).
   - Detail the implementation of **Bonferroni Correction** or the **Benjamini-Hochberg False Discovery Rate (FDR)**.

3. **Compute and Analyze Effect Sizes**:
   - Emphasize that p-values only state *if* a relationship exists, not *how strong* it is.
   - Outline metrics for effect size calculation: **Cohen's d** (for t-tests), **Cramér's V** (for Chi-Square), or **Eta-squared** (for ANOVA).

4. **Provide Production-Grade Python Audit Code**:
   - Write modular, readable Python code using `scipy.stats` and `statsmodels.stats.multitest.multipletests` to run appropriate hypothesis tests, calculate p-values, apply Benjamini-Hochberg corrections, compute effect sizes, and flag non-significant features for deletion.
</instructions>

<output_format>
Your Statistical Insignificance Audit Report should be structured as follows:

# Statistical Significance Feature Audit Registry

## 1. Hypothesis Testing Matrix
| Feature Name | Feature Type | Selected Test | Test Statistic | Raw p-value | Corrected p-value (BH) | Effect Size (d/V) | Decision |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| *age* | *Continuous* | *Mann-Whitney U* | *14502.5* | *0.001* | *0.004* | *0.32 (Medium)* | *RETAIN* |
| *noise_val* | *Continuous* | *Mann-Whitney U* | *20300.0* | *0.420* | *0.680* | *0.01 (Negligible)*| *EXCLUDE* |

## 2. Statistical Audit Methodology & Rationale
- **Multi-Test Correction Choice:** [Justification for Bonferroni vs Benjamini-Hochberg]
- **Effect Size Thresholding:** [Cut-off values used to determine if a statistically significant feature is practically important]

## 3. High-Performance Statistical Auditing Suite (Python)
```python
# [Insert clean, documented, modular Python statistical testing suite script]
```

## 4. Exclusion Ledger & Defensive Rationale
- **Feature Exclusion List:** [List of features flagged for removal]
- **Defensive Arguments:** [Ready-to-use justification for internal compliance or peer reviews explaining why these variables were dropped]
</output_format>

<style>
Maintain a highly rigorous, formal, and scientifically defensive tone. Ensure the Python code handles missing data automatically and validates testing assumptions (e.g., Shapiro-Wilk checks before student t-tests).
</style>

## Variables
- **FEATURES_LIST** – Names, scales, distributions, and sample sizes of candidate predictors.
- **TARGET_OUTCOME** – Target variable name and its quantitative type.
- **SIGNIFICANCE_LEVEL** – Cut-off alpha threshold (default 0.05) for rejecting null hypotheses.
- **STATISTICAL_TESTS_TO_USE** – Preference for parametric (assumes normal distributions) vs non-parametric (distribution-free) tests.

## Notes
- Bonferroni correction is extremely conservative and can increase Type II error rate (missing true relationships). Benjamini-Hochberg is generally preferred in machine learning feature selection.
- Spurious correlations are common when testing small sample sizes against high dimensions ($P > N$).
- Always verify that target categories are independent when running Chi-Square tests to ensure testing validity.
