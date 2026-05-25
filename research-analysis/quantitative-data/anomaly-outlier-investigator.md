---
title: "Data Anomaly & Outlier Investigator"
category: Research & Analysis
subcategory: Quantitative & Data Analysis
tags: [outlier-detection, anomaly-detection, data-cleaning, data-integrity]
model: any
---

## Purpose
Provides a structured methodology for identifying, investigating, and ethically treating statistical outliers and data anomalies in a dataset, ensuring that data cleaning decisions do not introduce scientific bias.

## Prompt
You are a senior data quality analyst, forensic statistician, and data integrity expert. Your task is to design a comprehensive Anomaly and Outlier Investigation Protocol for a specific dataset, ensuring statistical rigor and preventing analytical bias.

<context>
Outliers can represent two things: either critical, groundbreaking discoveries (e.g., a credit card fraud event, a rare astronomical phenomenon, a hyper-responsive clinical patient) or erroneous noise (e.g., data entry typos, sensor failures, calibration errors). Blindly deleting outliers is a major scientific sin that artificial distorts results, while ignoring them can violate statistical model assumptions. A systematic, forensic auditing approach is required.
</context>

<dataset_anomaly_profile>
- Dataset Context & Domain: {DATASET_CONTEXT}
- Key Quantitative Columns to Audit: {COLUMNS_TO_AUDIT}
- Suspected Source of Anomalies (if known): {SUSPECTED_SOURCES}
- Impact of False Positives vs. False Negatives in Outlier Treatment: {ERROR_IMPACT}
</dataset_anomaly_profile>

<instructions>
Develop a robust data anomaly and outlier investigation protocol. Address the following steps in detail:

1. **Univariate Outlier Detection Protocol**:
   - For continuous columns in {COLUMNS_TO_AUDIT}, establish univariate mathematical criteria for outlier detection.
   - Describe when to use the **Tukey's IQR method** (non-normal distributions) versus the **Z-Score / Modified Z-Score method** (normal distributions).
   - Define the exact thresholds (e.g., $1.5 \times IQR$ vs. $3.0 \times IQR$ for extreme outliers; $Z > 3.0$ or modified $Z > 3.5$).
   - Provide Python code executing these methods and plotting them visually using boxplots and histogram density overlays.

2. **Multivariate Outlier Detection Protocol**:
   - Explain how to detect hidden outliers that only appear anomalous when combining multiple dimensions (e.g., a person who is 5 feet tall weighing 250 lbs is an outlier, but neither 5 feet nor 250 lbs is a univariate outlier on its own).
   - Prescribe advanced detection methods such as **Mahalanobis Distance** (parametric multivariate), **Isolation Forests** (non-parametric machine learning), or **DBSCAN** (density-based clustering).
   - Detail the mathematical concepts behind these multivariate algorithms and explain how to tune their hyper-parameters (e.g., contamination rate in Isolation Forest).

3. **Forensic Investigation & Categorization Framework**:
   - Establish a decision-making framework to classify detected outliers into three categories:
     1. *Data Entry/System Errors* (e.g., negative ages, impossible values, sensor dropouts).
     2. *Genuine Extreme Values* (e.g., high-wealth individuals in income data).
     3. *Interesting Novelties / Discoveries* (e.g., unexpected physical reactions).
   - Outline the diagnostic checks to perform (e.g., checking system logs, interviewing data collectors, cross-referencing other rows) to verify an outlier's source.

4. **Ethical Treatment & Mitigation Strategy**:
   - Detail the exact treatment rules based on the category:
     - When to *Exclude/Drop* the data point (and how to document it to maintain reproducibility).
     - When to *Winsorize (Cap/Floor)* the extreme values and how to calculate the optimal percentiles (e.g., 99th and 1st percentiles).
     - When to *Apply Transformations* (such as log, square root, or robust scaling) to keep the data points while minimizing their influence on parametric models.
     - When to run *Sensitivity Analyses* (reporting model results both with and without the outliers included to demonstrate transparency).
</instructions>

<output_format>
Your output must follow this markdown structure:
- **1. Univariate Outlier Detection Strategy (IQR & Z-Score)**
- **2. Multivariate Outlier Detection Strategy (Algorithms & Setup)**
- **3. Forensic Investigation & Categorization Framework**
- **4. Outlier Treatment Matrix & Ethical Mitigation Rules**
- **5. Python Implementation Code (Pandas, Scikit-Learn, Scipy)**
- **6. Template for an Outlier Audit Log (Documentation Standard)**
</output_format>

<style>
Ensure a clinical, precise, and forensic scientific tone. Focus heavily on avoiding confirmation bias (avoid deleting outliers just because they do not support your hypothesis).
</style>

## Variables
- {DATASET_CONTEXT} – The field of research or industry domain (e.g., medical clinical trials, financial transaction monitoring, IoT industrial sensor telemetry).
- {COLUMNS_TO_AUDIT} – The specific numerical columns that need scanning (e.g., "Transaction_Amount, Age, Heart_Rate, Daily_Active_Minutes").
- {SUSPECTED_SOURCES} – Any known collection issues (e.g., "manual key-entry by hospital staff, potential database integration errors").
- {ERROR_IMPACT} – The consequences of getting it wrong (e.g., "Excluding a true fraud event could cost millions, while keeping a data entry typo will skew our predictive models").

## Notes
- **Model Recommendations**: Best used with advanced reasoning models (Claude 3.5 Sonnet, GPT-4o) which excel at algorithmic explanation and writing clean machine learning code.
- **Sensitivity Analysis**: Encourage the model to emphasize that the gold standard in academic research is performing the analysis *both* with and without outliers, and publishing both sets of results.
