---
title: "Record Deduplication & Duplicate Resolver"
category: "Data & Analytics"
subcategory: "Data Cleaning & Wrangling"
tags: [deduplication, record-linkage, fuzzy-matching, data-cleaning, pandas]
model: any
---

## Purpose
Identifies and resolves both exact duplicates and fuzzy, near-duplicate records across single or merged datasets using similarity metrics, blocking rules, and consensus-based field merging.

## Prompt
<context>
You are an expert in data warehousing, entity resolution, and record linkage. You know that duplicates are rarely exact matches; they are usually spread across variations in spellings, typos, changing addresses, and incomplete fields. You understand the risk of double-counting in analytical aggregations and the critical need for preserving clean record lineages during merging.
</context>

<task>
Construct a highly accurate record deduplication and duplicate resolution strategy. You must design a system that handles exact matching, implements fuzzy string matching using blocking techniques to manage computational complexity, applies domain-specific merging rules, and generates a robust Python deduplication workflow.
</task>

<inputs>
- **Dataset Sample & Schema:** {DATASET_SAMPLE_SCHEMA}
- **Key Identity Columns (e.g., Name, Email, Address):** {KEY_IDENTIFIER_COLUMNS}
- **Fuzzy Matching Thresholds & Metrics:** {FUZZY_MATCHING_THRESHOLD}
- **Conflict Resolution & Merging Rules:** {DUPLICATE_RESOLUTION_RULES}
</inputs>

<instructions>
1. **Define Deduplication Architecture**:
   - Establish **Exact Matching** protocols for high-fidelity identifiers (e.g., UUIDs, standard emails).
   - Outline **Fuzzy Matching** strategies using algorithms like Levenshtein distance, Jaro-Winkler, or TF-IDF cosine similarity for text columns with typos.
   - Implement **Blocking Keys** (e.g., grouping by first letter of last name, or postal prefix) to reduce the quadratic complexity $O(N^2)$ of comparing every record to every other record.

2. **Design the Conflict Resolution Engine**:
   - Define custom merging rules when combining duplicate records into a single "golden record" based on `{DUPLICATE_RESOLUTION_RULES}`:
     - **Latest Record Wins** (based on timestamp).
     - **Completeness First** (merge fields to maximize non-null values).
     - **Consensus Vote** (majority value across duplicates).
     - **Hierarchical Trust** (trust Source A over Source B).

3. **Establish Lineage and Audit Trail**:
   - Describe how the deduplication system should store the mapping of old IDs to new golden IDs to allow tracking and rollback of automated merges.

4. **Provide Production-Ready Code**:
   - Deliver a robust Python script using `pandas` and fuzzy string comparison (such as `rapidfuzz` or `difflib`) that implements blocking, scoring, and merging.
</instructions>

<output_format>
Your Duplicate Resolution & Deduplication Plan should be structured as follows:

# Record Entity Resolution & Deduplication Strategy

## 1. Blocking and Matching Strategy
- **Blocking Key Definition:** [Explain how you will group records before fuzzy comparison to optimize performance]
- **Matching Rules Matrix:**
  | Target Feature | Match Metric | Threshold | Justification |
  | :--- | :--- | :--- | :--- |
  | *Name* | *Jaro-Winkler* | *0.88* | *Forgives minor spelling typos and abbreviation changes* |

## 2. Conflict Resolution & Merging Policy
*Detailed rules explaining how conflicts are resolved when fields in duplicate records mismatch.*
- **Policy 1 (Completeness):** [Explanation]
- **Policy 2 (Temporal Priority):** [Explanation]

## 3. High-Performance Deduplication Workflow (Python)
```python
# [Insert clean, documented, modular Python script using blocking and fuzzy matching to resolve duplicates]
```

## 4. Entity Lineage Tracking Schema
- **Mapping Table Structure:** [Describe the structure of the lineage audit table]
</output_format>

<style>
Ensure the code is optimized for performance, using vectorized pandas operations and indexing wherever possible. Avoid nested for-loops over large DataFrames.
</style>

## Variables
- **DATASET_SAMPLE_SCHEMA** – Columns, data types, and typical values in the target dataset.
- **KEY_IDENTIFIER_COLUMNS** – Features that uniquely identify individuals, entities, or transactions.
- **FUZZY_MATCHING_THRESHOLD** – Degree of similarity required to trigger a match (e.g., 0.85 Jaro-Winkler).
- **DUPLICATE_RESOLUTION_RULES** – Pre-defined business preferences for merging columns and deciding which values to keep.

## Notes
- To avoid $O(N^2)$ comparisons on huge datasets, blocking is absolutely mandatory. For example, blocking on `zip_code` only compares records within the same geographical zone.
- RapidFuzz is highly recommended in python as it is implemented in C++ and is significantly faster than standard FuzzyWuzzy.
- Always preserve an `original_record_ids` list inside the consolidated golden record to ensure analytical traceability.
