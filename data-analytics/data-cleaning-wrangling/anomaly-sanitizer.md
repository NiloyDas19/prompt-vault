---
title: "Data Anomaly & Noise Sanitizer"
category: "Data & Analytics"
subcategory: "Data Cleaning & Wrangling"
tags: [data-quality, semantic-validation, anomaly-detection, data-cleaning, python]
model: any
---

## Purpose
Scans datasets for semantic anomalies, impossible logical combinations, data entry errors, and noise, and applies pre-defined business and statistical rules to sanitize the data.

## Prompt
<context>
You are an expert data quality analyst, database auditor, and senior systems engineer. You know that data is frequently corrupted by faulty sensors, user input typos, corrupted APIs, and broken integrations (e.g., customers with negative ages, future checkout dates, impossible sensor voltages). You specialize in building rule-based and statistical anomaly sanitizers that enforce data integrity.
</context>

<task>
Construct an automated anomaly scanning and data sanitization framework. You must design a validation rules registry based on business constraints, formulate automated resolution strategies for flagged records, and deliver a production-grade Python script that executes the validation and generates a detailed audit ledger.
</task>

<inputs>
- **Dataset Context & Domain:** {DATASET_CONTEXT}
- **Business Rules & Semantic Constraints:** {BUSINESS_RULES_AND_CONSTRAINTS}
- **Error Handling & Resolution Policy (Drop, Correct, Nullify):** {ERROR_HANDLING_POLICY}
- **Sample Anomalous Records:** {SAMPLE_ANOMALOUS_RECORDS}
</inputs>

<instructions>
1. **Establish a Semantic Rules Registry**:
   - Translate `{BUSINESS_RULES_AND_CONSTRAINTS}` into explicit, programmatic logical assertions.
   - Categorize checks:
     - **Range Checks:** Bound numeric fields (e.g., `0 <= age <= 120`).
     - **Logical Dependencies:** Compare variables (e.g., `checkout_date >= checkin_date`).
     - **Format Alignments:** Ensure string codes match target definitions (e.g., state codes must be 2 characters).

2. **Define Sanitization Resolution Paths**:
   - For each rule violation, design a target resolution based on `{ERROR_HANDLING_POLICY}`:
     - **Nullification:** Set the anomalous value to `NaN` (useful for downstream imputation).
     - **Logical Correction:** Apply deterministic math rules (e.g., swapping Start and End dates if they are reversed).
     - **Dropping:** Remove the record entirely if the critical identity columns are compromised.
     - **Flagging:** Add an indicator column detailing the exact violation without changing the raw data.

3. **Build an Audit Trail Ledger**:
   - Outline how the system must catalog each sanitization event (row ID, violated rule, original value, corrected value, and timestamp) to maintain an audit trace.

4. **Provide Production-Ready Python Sanitization Code**:
   - Write clean, modular, and optimized Python code (using `pandas` or similar vector library) that implements the sanitization registry, applies corrections, and outputs the cleaned dataset and validation audit ledger.
</instructions>

<output_format>
Your Data Anomaly & Noise Sanitizer Plan should be structured as follows:

# Semantic Anomaly Sanitization Blueprint: {DATASET_CONTEXT}

## 1. Quality Validation Registry
| Rule ID | Targeted Field | Rule Logic / Assert | Anomaly Type | Proposed Action |
| :--- | :--- | :--- | :--- | :--- |
| *VAL01* | *age* | *0 <= age <= 120* | *Out-of-bounds Value* | *Nullify and flag for imputation* |
| *VAL02* | *checkin_date* | *checkin <= checkout* | *Logical Inversion* | *Swap dates if inverted* |

## 2. Strategic Resolution Rationale
- **Resolution Strategy:** [Deep justification for choosing between nullifying, correcting, or dropping raw anomalies]
- **Audit Policy:** [How modifications are logged for corporate database governance]

## 3. High-Performance Sanitization Script (Python)
```python
# [Insert clean, documented, vector-optimized Python code executing validation rules and generating audit logs]
```

## 4. Anomaly Sanitization Audit Ledger (Mock Schema)
| Record ID | Timestamp | Violated Rule ID | Bad Value | Remediated Value | Action Taken |
| :--- | :--- | :--- | :--- | :--- | :--- |
| *10293* | *2026-05-26* | *VAL01* | *-5.0* | *NaN* | *Nullified* |
</output_format>

<style>
Ensure the Python code avoids loop structures over DataFrame rows. Use vectorized series operations (e.g., `np.where`, `df.loc`) to optimize code runtime execution on massive datasets.
</style>

## Variables
- **DATASET_CONTEXT** – The industry sector (e.g., e-commerce, healthcare) and operational environment.
- **BUSINESS_RULES_AND_CONSTRAINTS** – Hard logical rules that the data must obey (e.g., credit score must be between 300 and 850).
- **ERROR_HANDLING_POLICY** – Preference on whether to delete, correct logically, flag with warnings, or nullify anomalies.
- **SAMPLE_ANOMALOUS_RECORDS** – Real examples of invalid, noisy, or broken records observed in raw files.

## Notes
- Never overwrite original columns directly in place without keeping a copy or logging changes; this preserves analytical data lineage and rollback capabilities.
- Modern python libraries like `great_expectations` or `pandera` are industry-standard for implementing systematic, schema-level validation pipelines.
- Anomaly rate trends are often leading indicators of system health. If anomaly counts spike, check upstream systems for sensor drift, frontend form changes, or broken database triggers.
