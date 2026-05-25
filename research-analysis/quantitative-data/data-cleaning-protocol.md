---
title: "Data Cleaning & Preparation Protocol"
category: Research & Analysis
subcategory: Quantitative & Data Analysis
tags: [data-cleaning, pandas, preprocessing, data-wrangling]
model: any
---

## Purpose
Establishes a systematic, reproducible workflow for cleaning, transforming, and preparing raw datasets for downstream statistical analysis or machine learning, ensuring data integrity and preventing bias.

## Prompt
You are an expert data engineer and senior quantitative analyst. Your task is to draft a comprehensive, step-by-step Data Cleaning and Preparation Protocol for a raw dataset based on its schema, issues, and downstream objectives.

<context>
Raw data is rarely ready for statistical analysis or modeling. It often suffers from missing values, inconsistent formatting, outliers, duplicate records, and structural anomalies. To prevent "garbage-in, garbage-out" outcomes, a structured cleaning protocol must be defined, coded, and documented for reproducibility.
</context>

<dataset_profile>
- Dataset Description & Source: {DATASET_DESCRIPTION}
- Data Schema & Data Types: {DATA_SCHEMA}
- Known or Suspected Data Quality Issues: {KNOWN_ISSUES}
- Downstream Analytics/Modeling Goal: {DOWNSTREAM_GOAL}
</dataset_profile>

<instructions>
Based on the dataset profile, create a detailed data cleaning, transformation, and validation protocol. Provide the instructions in structured steps and include executable Python (Pandas/NumPy) code blocks for implementation.

1. **Initial Diagnostic Profile (Exploratory Data Audit)**:
   - Detail the methods for auditing the raw dataset (e.g., checking data types, non-null counts, memory usage, basic descriptive statistics).
   - Provide standard code commands to identify structural errors, duplicate rows, and schema inconsistencies.

2. **Missing Data Handling Strategy**:
   - Establish rules for diagnosing the mechanism of missingness: Missing Completely at Random (MCAR), Missing at Random (MAR), or Missing Not at Random (MNAR).
   - Prescribe specific treatment rules for each column type (e.g., listwise deletion, median/mode imputation, K-Nearest Neighbors (KNN) imputation, or Multiple Imputation by Chained Equations (MICE)).
   - Provide justification for why the chosen imputation strategies minimize statistical bias.

3. **Structural and Formatting Standardization**:
   - Detail rules for standardizing text strings (capitalization, strip white spaces, regex pattern standardizations for emails, phone numbers, or dates).
   - Outline how to handle categorical variables (handling rare classes, resolving spelling variations, consistent label encoding, or one-hot encoding).
   - Explain date/time standardizations (timezone adjustments, extraction of cyclical features like day-of-week or hour).

4. **Outlier and Anomaly Treatment**:
   - Define statistical rules for identifying outliers (e.g., Z-score method for normally distributed columns, Tukey's IQR fence rule for skewed columns, or isolation forests for multivariate datasets).
   - Outline the treatment protocol for verified outliers: Winsorization (capping), transformation (log, Box-Cox), or exclusion, with statistical justifications.

5. **Data Transformation & Feature Engineering (Prep for Analysis)**:
   - Outline scale normalization strategies (MinMax scaling, Standardization / Z-score scaling, Robust scaling).
   - Prescribe transformation rules to resolve skewness (log transformations, square-root, or power transformations) to satisfy downstream statistical assumptions.

6. **Integrity Validation & Reproducibility Audit**:
   - Define a set of assertions or unit tests (e.g., using `great_expectations` framework concepts or simple Pandas assertions) to verify data integrity post-cleaning.
   - Describe how to output a "Cleaning Audit Log" summarizing the percentage of rows modified, missing values resolved, and outliers treated.
</instructions>

<output_format>
Format your output with the following markdown headers:
- **1. Exploratory Data Audit & Diagnostic Plan**
- **2. Systematic Missing Data Protocol**
- **3. Formatting, Typing, & Categorical Standardization**
- **4. Outlier & Anomaly Detection & Mitigation**
- **5. Normalization, Transformations, & Feature Scaling**
- **6. Post-Cleaning Integrity Assertions & Validation Checks**
- **7. Production-Ready Python Cleaning Pipeline Code**
</output_format>

<style>
Maintain an engineering-focused, structured, and highly precise tone. All code snippets must be robust, modular, commented, and handle potential edge cases (such as dividing by zero or empty values).
</style>

## Variables
- {DATASET_DESCRIPTION} – A brief summary of what the dataset contains, its source, size, and format (e.g., 50,000 rows of customer transaction records from SQL server).
- {DATA_SCHEMA} – A list of columns, their intended data types, and brief descriptions (e.g., ID (int), Date (string 'YYYY-MM-DD'), Revenue (float), Segment (categorical)).
- {KNOWN_ISSUES} – Specific issues known in advance (e.g., missing values in 'Revenue' column, date column is stored as string with mixed formats, duplicate IDs).
- {DOWNSTREAM_GOAL} – The ultimate use of the clean dataset (e.g., linear regression modeling, K-means clustering, dashboard visualization).

## Notes
- **Reusability**: The resulting Python code should be structured as a single pipeline function `clean_data(df)` that accepts a raw DataFrame and returns a clean, fully validated DataFrame.
- **Handling Bias**: Emphasize to the model that simply dropping rows with missing values (listwise deletion) is often unacceptable as it introduces selection bias and reduces statistical power.
