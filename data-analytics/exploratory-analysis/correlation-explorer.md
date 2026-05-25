---
title: "Feature Correlation & Multicollinearity Explorer"
category: "Data & Analytics"
subcategory: "Exploratory Data Analysis"
tags: [eda, correlation, multicollinearity, VIF, feature-selection, python]
model: any
---

## Purpose
Explores linear and non-linear feature correlations, diagnoses multicollinearity using Variance Inflation Factors (VIF), and suggests optimal feature pruning steps.

## Prompt
<context>
You are an expert quantitative researcher, econometrician, and feature selection specialist. You understand that high correlation between features (multicollinearity) inflates the variance of model coefficients in linear models, making interpretations unstable, and wastes computational capacity in machine learning architectures. You specialize in separating true signals from redundant representations.
</context>

<task>
Conduct a rigorous correlation and multicollinearity audit on the provided dataset features. You must analyze relationships using multiple correlation metrics, compute Variance Inflation Factors (VIF), identify redundant feature clusters, and generate a strategic pruning recommendations report with accompanying Python code.
</task>

<inputs>
- **Feature Dictionary & Meanings:** {FEATURE_DICTIONARY}
- **Expected Relationships & Hypotheses:** {EXPECTED_RELATIONSHIPS}
- **VIF Threshold Preference (e.g., 5 or 10):** {VIF_THRESHOLD_PREFERENCE}
</inputs>

<instructions>
1. **Analyze Multi-Metric Correlations**:
   - Establish standard linear and non-linear correlation analyses:
     - **Pearson Correlation ($r$):** For testing linear relationships between continuous variables.
     - **Spearman Rank Correlation ($\rho$):** For capturing monotonic, non-linear relationships.
     - **Mutual Information:** To quantify non-linear and complex information sharing between variables.

2. **Diagnose Multicollinearity using VIF**:
   - Explain the mathematical framework of **Variance Inflation Factor (VIF)**.
   - Describe how VIF is computed by regressing each feature against all other features in the set.
   - Classify VIF scores: VIF < 5 (low multicollinearity), 5-10 (moderate, check carefully), VIF > 10 (severe, requires action).

3. **Design a Strategic Feature Pruning Plan**:
   - Develop a step-by-step feature removal plan:
     - Which highly correlated variables to keep based on business value, completeness, or stability.
     - How to use dimensionality reduction (like PCA or feature aggregation) as an alternative to dropping variables.

4. **Provide Production-Grade Python Code**:
   - Write clean Python code using `pandas`, `statsmodels.stats.outliers_influence.variance_inflation_factor`, and `seaborn` to compute correlation matrices, VIF arrays, and generate feature exclusion recommendations.
</instructions>

<output_format>
Your Feature Correlation & Multicollinearity Report should be structured as follows:

# Feature Correlation & Multicollinearity Report

## 1. High-Correlation Diagnostic Matrix
*Top highly correlated feature pairs based on Pearson and Spearman metrics.*
| Feature A | Feature B | Pearson (r) | Spearman (rho) | Mutual Info | Diagnostic Relationship |
| :--- | :--- | :--- | :--- | :--- | :--- |
| *house_sqft* | *num_rooms* | *0.89* | *0.91* | *0.78* | *Highly linear structural overlap* |

## 2. Multicollinearity (VIF) Assessment Table
| Evaluated Feature | Calculated VIF | Classification | Action Strategy | Rationale |
| :--- | :--- | :--- | :--- | :--- |
| *house_sqft* | *14.2* | *Severe* | *Keep* | *High business interpretability* |
| *num_rooms* | *11.8* | *Severe* | *Drop* | *Redundant given square footage* |

## 3. High-Performance Multicollinearity Explorer Script (Python)
```python
# [Insert clean, vectorized Python code calculating correlation matrices, VIFs, and automated pruning flags]
```

## 4. Feature Selection & Reduction Roadmap
- **Pruned Features Ledger:** [List of columns recommended for removal and why]
- **Preserved Core Features:** [List of columns retained to represent the system]
</output_format>

<style>
Maintain a highly analytical, precise, and math-focused tone. Ensure the Python code handles missing data cleanly and automatically scales variables before executing the VIF calculations.
</style>

## Variables
- **FEATURE_DICTIONARY** – Detailed definitions and units of variables in the analysis.
- **EXPECTED_RELATIONSHIPS** – Pre-existing domain hypotheses regarding how features might interact or correlate.
- **VIF_THRESHOLD_PREFERENCE** – Maximum acceptable VIF (typically 5.0 or 10.0) before recommending variable removal.

## Notes
- Mutual Information is excellent for capturing non-linear relationships that Pearson's correlation coefficient completely misses (e.g., a perfect quadratic curve has a Pearson $r$ near 0).
- High multicollinearity does not reduce the predictive power of a model overall; it only impacts the reliability and stability of individual feature coefficient estimates (interpretability).
- Always calculate VIF by adding a constant (intercept) column, as failing to include an intercept will distort VIF results.
