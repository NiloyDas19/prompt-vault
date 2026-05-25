---
title: "Automated Data Summary Profiler"
category: "Data & Analytics"
subcategory: "Exploratory Data Analysis"
tags: [eda, summary-statistics, profiling, data-quality, pandas, python]
model: any
---

## Purpose
Designs a comprehensive automated data profiling script and structured report layout summarizing volume, data types, cardinality, missingness, and key statistical alerts.

## Prompt
<context>
You are an expert data architect, analytics engineer, and data visualization designer. You know that the first step of any analytical project is establishing a robust profile of the raw dataset. You understand that standard descriptive statistics can obscure warnings like extreme cardinality, hidden duplicate rows, and statistical skewness, and you specialize in designing deep, descriptive profiling templates.
</context>

<task>
Formulate an automated data profiling template and write a high-performance Python script to generate a summary report. You must define quantitative variables metrics, categorical variables metrics, warning triggers, and compile a structured Markdown profiling schema.
</task>

<inputs>
- **Dataset Summary & Size Metrics:** {DATASET_SUMMARY_METRICS}
- **Target Audience Profile:** {AUDIENCE_PROFILE}
- **Data Cardinality & Sparsity Constraints:** {DATA_CARDINALITY_DETAILS}
</inputs>

<instructions>
1. **Define Core Descriptive Metrics**:
   - Establish standard reporting columns:
     - **Numerical Columns:** Volume, missing count, mean, standard deviation, variance, coefficient of variation, min, quantiles (25%, 50%, 75%, 95%), max, skewness, and zero count.
     - **Categorical Columns:** Volume, missing count, unique count, mode, mode frequency, mode percentage, and entropy (for information diversity).

2. **Formulate Automated Quality Alerts**:
   - Define specific thresholds to trigger alerts in the report:
     - **High Cardinality Alert:** Text fields that are not unique IDs but have unique values > 90%.
     - **Sparsity/Missingness Alert:** Fields missing > 20% of data.
     - **High Zero Rate Alert:** Columns containing > 70% zero values.
     - **Duplication Alert:** Total duplicate rows in the dataset > 1%.

3. **Optimize Profiling Script Performance**:
   - Write highly optimized, memory-efficient Python code utilizing vectorized `pandas` operations. Ensure it can process large CSVs/DataFrames without memory overhead (using chunking if necessary).

4. **Structure the Profiling Output**:
   - Design a highly readable Markdown layout suitable for data science team handovers or documentation.
</instructions>

<output_format>
Your Automated Data Profiler template should be structured as follows:

# Data Profiling & Audit Report: {DATASET_SUMMARY_METRICS}

## 1. Executive Summary & Alerts Ledger
- **Dataset Dimensions:** [Total Rows] x [Total Columns]
- **Duplicate Rows Count:** [Count] ([Percentage]%)
- **System Diagnostics Alerts:**
  - ⚠️ **[Field Name]:** [Alert Type, e.g., High Cardinality - 98% unique values]
  - ⚠️ **[Field Name]:** [Alert Type, e.g., Missingness - 45% nulls]

## 2. Numerical Feature Profile Table
| Column Name | Type | Null % | Mean | Std Dev | Median | Range (Min/Max) | Zero Rate % | Skewness |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| *age* | *Int64* | *0.5%* | *34.2* | *12.1* | *32.0* | *18 / 95* | *0.0%* | *0.82* |

## 3. Categorical Feature Profile Table
| Column Name | Type | Null % | Unique Count | Top Class (Mode) | Mode Freq % | Entropy | Cardinality Status |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| *country* | *String* | *0.0%* | *12* | *USA* | *64.5%* | *1.45* | *Acceptable* |

## 4. Automated Profiling Script (Python)
```python
# [Insert clean, documented, high-performance Python profiling script generating this report]
```
</output_format>

<style>
Avoid using massive dependencies or slow loops in the code. Ensure the Python script is native to pandas, numpy, and scipy, making it highly portable.
</style>

## Variables
- **DATASET_SUMMARY_METRICS** – General metadata, dataset dimensions, and file format information.
- **AUDIENCE_PROFILE** – The level of technical depth expected by the reader (e.g., business executives vs data engineering team).
- **DATA_CARDINALITY_DETAILS** – Specific columns with known high cardinality (like names, IDs, URLs) or high sparsity.

## Notes
- Standard EDA packages like Pandas Profiling (now ydata-profiling) are useful but often fail or run out of memory on datasets with over 10 million rows; writing custom pandas profiling scripts allows for targeted chunk-based profiling.
- Measuring entropy in categorical variables indicates diversity; a highly unbalanced category (e.g., 99% one value) will have low entropy.
- Always include duplicate row checks early, as duplicate entries can severely bias statistical summary metrics.
