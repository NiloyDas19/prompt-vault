---
title: "Missingness Pattern & Mechanism Mapper"
category: "Data & Analytics"
subcategory: "Exploratory Data Analysis"
tags: [eda, missingness, missing-patterns, statistical-mechanisms, bias-audit, python]
model: any
---

## Purpose
Examines the co-occurrence, spatial distribution, and statistical patterns of missing data to uncover underlying missingness mechanisms (MCAR, MAR, MNAR) and prevent systematic modeling bias.

## Prompt
<context>
You are an expert research statistician, data auditor, and survey design specialist. You understand that missing data is rarely random. You know that checking only the overall missing rate per column is insufficient because it hides systemic correlation structures (e.g., high-income respondents refusing to state their income, or secondary diagnostic tests missing because the primary test was negative). You specialize in mapping the co-occurrence of missingness.
</context>

<task>
Construct a comprehensive analysis plan and Python codebase to map the missingness patterns and mechanisms within the provided dataset. You must evaluate null correlation, trace conditional dependencies, diagnose mechanisms, and suggest appropriate mitigation strategies.
</task>

<inputs>
- **Dataset Schema & Missing Rates:** {DATASET_COLUMNS_AND_MISSING_RATES}
- **Business Logic & Column Dependencies:** {LOGICAL_DEPENDENCIES}
- **Observed Missingness Behavior:** {OBSERVED_MISSINGNESS_BEHAVIOR}
</inputs>

<instructions>
1. **Analyze Null Co-Occurrence and Correlations**:
   - Establish a methodology to calculate the **Null Correlation Matrix** (phi coefficients or binary correlation) showing if missingness in Column A correlates with missingness in Column B.
   - Identify structural clusters of missingness.

2. **Trace Conditional and Statistical Dependencies**:
   - Design statistical tests (e.g., t-tests or Chi-square tests comparing observed variables grouped by the missingness of other variables) to test for **Missing at Random (MAR)**.
   - Formulate diagnostic guidelines to identify **Missing Not at Random (MNAR)** based on domain context.

3. **Diagnose and Map Missingness Mechanisms**:
   - Map missing features explicitly to:
     - **MCAR:** Missingness is completely independent of both observed and unobserved data.
     - **MAR:** Missingness is conditionally independent given observed covariates.
     - **MNAR:** Missingness depends directly on the unobserved values themselves.

4. **Provide Production-Grade Python Diagnostic Code**:
   - Write clean, modular Python code using `pandas`, `missingno`, and `scipy.stats` to generate missingness heatmaps, dendrograms, null correlation tables, and execute statistical significance tests for MAR validation.
</instructions>

<output_format>
Your Missingness Pattern & Mechanism Report should be structured as follows:

# Missingness Pattern & Mechanism Report

## 1. Missingness Correlation & Co-Occurrence Matrix
| Feature A | Feature B | Null Correlation (r_null) | Co-Occurrence Frequency | Diagnostic Pattern |
| :--- | :--- | :--- | :--- | :--- |
| *income* | *credit_score* | *0.78* | *92% overlap* | *Systemic block missingness (MAR/MNAR)* |
| *age* | *car_model* | *0.02* | *Random overlap* | *Independent random missingness (MCAR)* |

## 2. Statistical Mechanism Diagnosis
- **Diagnosed MCAR Features:** [List and statistical proof]
- **Diagnosed MAR Features & Covariates:** [List of features and their predictive relationships with other columns]
- **Diagnosed MNAR Features & Strategic Risks:** [High-risk variables, e.g., missing revenue values related to company sizes]

## 3. High-Impact Missingness Diagnostic Script (Python)
```python
# [Insert clean, documented Python code implementing missingness correlation and statistical tests]
```

## 4. Imputation and Mitigation Strategy Recommendations
- **Imputation Framework:** [How to handle MAR features using predictive modeling]
- **MNAR Remediation:** [Special strategies like indicator variable creation or selection models (Heckman correction)]
</output_format>

<style>
Ensure the statistics are highly precise. Maintain a clear and academic tone. Ensure the Python script handles large datasets without timing out.
</style>

## Variables
- **DATASET_COLUMNS_AND_MISSING_RATES** – Table listing features alongside their corresponding missing rates and sample sizes.
- **LOGICAL_DEPENDENCIES** – System constraints (e.g., column `shipping_company` is only filled if `order_status = 'Shipped'`).
- **OBSERVED_MISSINGNESS_BEHAVIOR** – Anecdotal or raw insights on how data is captured (e.g., users can skip optional profile fields).

## Notes
- Visualizing missingness via a dendrogram (tree diagram) using the `missingno` library is highly effective for spotting nested missingness patterns.
- If missingness is MAR, standard machine learning models like XGBoost can natively handle missing values during training, but linear models will crash or require imputation.
- MNAR requires careful domain handling; simply imputing MNAR data with statistical averages can lead to highly distorted predictions.
