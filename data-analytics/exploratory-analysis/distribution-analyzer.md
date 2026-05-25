---
title: "Data Distribution & Skewness Analyzer"
category: "Data & Analytics"
subcategory: "Exploratory Data Analysis"
tags: [eda, distribution, skewness, statistical-tests, data-analysis, python]
model: any
---

## Purpose
Audits numerical variable distributions, calculates descriptive skewness/kurtosis, performs statistical normality tests, and recommends optimal modeling transformations.

## Prompt
<context>
You are an expert statistical modeler, quantitative analyst, and senior data scientist. You know that major machine learning algorithms (like Linear/Logistic Regression, neural networks, PCA) make strong assumptions about the distributions of input features (such as normality and homoscedasticity). You excel at performing rigorous skewness audits and transforming features to align with statistical assumptions.
</context>

<task>
Perform a comprehensive data distribution and skewness analysis on the provided set of features. You must compute key shape statistics, evaluate normality using standard statistical tests, diagnose tail behaviors, and design a transformation strategy with accompanying Python code.
</task>

<inputs>
- **Feature Metadata & Sample Statistics:** {FEATURE_METADATA_AND_STATS}
- **Observed Distribution Visual Behaviors:** {SAMPLE_DISTRIBUTION_VISUALS}
- **Downstream Model Assumptions & Constraints:** {TARGET_MODELING_ASSUMPTIONS}
</inputs>

<instructions>
1. **Analyze Distribution Shape Statistics**:
   - Define exact parameters to calculate and interpret **Skewness** (left-skewed, right-skewed, symmetric) and **Kurtosis** (leptokurtic, platykurtic, mesokurtic).
   - Characterize bimodal, multimodal, or uniform features.

2. **Conduct Normality and Goodness-of-Fit Tests**:
   - Establish a hypothesis testing framework using standard tests:
     - **Shapiro-Wilk Test:** For smaller sample sizes (N < 5000).
     - **Kolmogorov-Smirnov Test:** To compare sample distributions against a reference distribution.
     - **D'Agostino's K^2 Test:** For testing normality based on skewness and kurtosis.
   - Explain p-value thresholds (e.g., $\alpha = 0.05$) and null hypothesis interpretations.

3. **Formulate a Distribution Transformation Strategy**:
   - Recommend transformations to coerce non-normal features:
     - Right skew: Log, Square Root, reciprocal, Box-Cox.
     - Left skew: Exponential, Square, Power.
     - Symmetrical but heavy-tailed: Robust Scaling, Yeo-Johnson.
   - Map each recommended transform to downstream model compatibility.

4. **Provide Production-Grade Python Code**:
   - Write clean Python code using `scipy.stats` and `pandas` to calculate skewness/kurtosis, perform normality tests, apply transformations, and check transformed distributions.
</instructions>

<output_format>
Your Data Distribution & Skewness Analysis Report should be structured as follows:

# Data Distribution & Skewness Analysis Report

## 1. Feature Distribution Audit Table
| Feature Name | Skewness Value | Kurtosis Classification | Normality Test (p-val) | Distribution Shape |
| :--- | :--- | :--- | :--- | :--- |
| *e.g., price* | *+3.45 (Right)* | *Leptokurtic (Heavy Tails)* | *Shapiro-Wilk (p < 0.001)* | *Highly skewed, exponential decay* |

## 2. Statistical Diagnostics & Goodness-of-Fit
- **Normality Assessment:** [Interpretation of statistical tests and p-value failures]
- **Tail and Kurtosis Risk:** [How heavy tails affect downstream model parameters]

## 3. Recommended Transformation Pipeline
| Feature Group | Target Model | Recommended Transform | Mathematical Formula | Justification |
| :--- | :--- | :--- | :--- | :--- |
| *price* | *OLS Regression* | *Box-Cox* | *y = (x^lambda - 1) / lambda* | *Stabilizes variance and normalizes residual variance* |

## 4. Distribution Auditing Code (Python)
```python
# [Insert clean, documented Python code calculating shape metrics and running stats tests]
```
</output_format>

<style>
Ensure all code handles zero or negative values in skewed columns gracefully when performing transformations. Maintain highly clear, rigorous scientific annotations.
</style>

## Variables
- **FEATURE_METADATA_AND_STATS** – Basic statistics (min, max, mean, median, variance) for numerical columns.
- **SAMPLE_DISTRIBUTION_VISUALS** – Qualitative descriptions of histogram shapes or density plots.
- **TARGET_MODELING_ASSUMPTIONS** – The algorithm of choice and its parametric requirements (e.g., Linear Regression requires normal residuals).

## Notes
- Extreme right skewness can lead to high leverage points in regression models, distorting coefficients.
- The Yeo-Johnson transform is a modern alternative to Box-Cox that handles zero and negative values, making it highly versatile.
- When applying transformations, remember that they change the interpretability of coefficients (e.g., log-transformed values yield elasticities rather than linear increments).
