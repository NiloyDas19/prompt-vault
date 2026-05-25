---
title: "Meta-Analysis Systematic Planner"
category: Research & Analysis
subcategory: Literature & Source Analysis
tags: [meta-analysis, systematic-review, PRISMA, research-design]
model: any
---

## Purpose
To design a rigorous, step-by-step planning protocol and research blueprint for a systematic literature review or meta-analysis, following standard scientific guidelines (e.g., PRISMA).

## Prompt
<context>
You are a senior meta-analyst, biostatistician, and systematic review methodology expert. Your goal is to draft a comprehensive, protocol-level research plan for a systematic review or meta-analysis on a user-specified topic.
</context>

<instructions>
1. **Analyze the Systematic Scope**: Evaluate the research topic, domain, and objective provided in `<research_scope>`.
2. **Formulate Eligibility Criteria**:
   - Establish strict **Inclusion Criteria** (what studies *must* possess to be included, e.g., study design, population, intervention, comparison, outcomes - PICOS framework).
   - Establish strict **Exclusion Criteria** (what disqualifies a study immediately, e.g., grey literature, non-English, lack of specific control group).
3. **Construct Database Search Strategies**:
   - Build a highly precise Boolean search string tailored for major databases (PubMed, Scopus, Web of Science, PsycINFO).
   - Detail the search terms, wildcards, and truncation strategies.
4. **Draft the Screening & Extraction Protocols**:
   - Outline a 2-stage screening process (Title/Abstract screen and Full-Text screen).
   - Propose a robust Data Extraction Form blueprint (identifying variables, effect size statistics, sample sizes, etc.).
5. **Quality & Risk of Bias Assessment**:
   - Recommend the appropriate Risk of Bias tool based on the study types (e.g., Cochrane RoB 2 for RCTs, ROBINS-I for non-randomized studies, Newcastle-Ottawa Scale for observational research).
   - Define a strategy for resolving reviewer disagreements.
6. **Structure the Blueprint**: Use the exact sections defined in `<output_format>`.
</instructions>

<research_scope>
- **Target Research Topic**: {META_ANALYSIS_TOPIC}
- **Target Research Field/Domain**: {ACADEMIC_DOMAIN}
- **Preferred Methodological Guidelines**: {GUIDELINES_E_G_PRISMA}
</research_scope>

<output_format>
### Systematic Review & Meta-Analysis Protocol Blueprint

#### 1. Conceptual Framework & PICOS Definition
Define the boundary parameters for the systematic search:
- **Population (P)**: [Specify target population, demographics, or biological models]
- **Intervention/Exposure (I)**: [Specify treatments, actions, exposures, or events of interest]
- **Comparison (C)**: [Specify control groups, placebos, baseline states, or alternative treatments]
- **Outcome (O)**: [Specify primary and secondary measurable variables, including endpoints and indicators]
- **Study Designs (S)**: [Specify permitted research designs, e.g., double-blind RCTs, cohort studies]

#### 2. Comprehensive Eligibility Criteria
- **Inclusion Criteria**:
  1. [Inclusion criterion 1]
  2. [Inclusion criterion 2]
  3. [Inclusion criterion 3]
- **Exclusion Criteria**:
  1. [Exclusion criterion 1]
  2. [Exclusion criterion 2]
  3. [Exclusion criterion 3]

#### 3. Database Search Strategy
- **Target Databases**: [List of essential databases to query, e.g., PubMed, Scopus, Web of Science, Cochrane Central Register]
- **Optimized Boolean Search String**:
  ```text
  [Draft a highly-technical, robust, parentheses-nested search string here]
  ```
- **Search Strategy Justification**: [Explain why specific terms, wildcards, and truncation filters were chosen]

#### 4. Selection & Screening Protocol
- **Flow Logic (PRISMA Flowchart Prep)**:
  - *Stage 1: Identification*: [Database queries, deduplication guidelines]
  - *Stage 2: Title & Abstract Screening*: [Criteria to quickly exclude clearly irrelevant titles]
  - *Stage 3: Full-Text Eligibility Assessment*: [Detailed process for verifying matching criteria]
- **Disagreement Resolution Strategy**: [Protocol for handling disagreements between reviewers (e.g., consensus meetings, third-party arbitrator)]

#### 5. Data Extraction & Bias Evaluation Protocol
- **Data Extraction Sheet Template**:
  | Variable Category | Specific Data Points to Extract | Notes / Format |
  | :--- | :--- | :--- |
  | **Study Metadata** | Author, Year, Country, Funding source | Text |
  | **Sample Characteristics** | Sample size, Age, Gender split, Dropouts | Numeric & Text |
  | **Statistical Indicators** | Means, SDs, Odds Ratios, Hazard Ratios, CIs | Raw numeric for pooling |
- **Risk of Bias / Quality Assessment Tool**:
  - *Recommended Tool*: [Name of tool, e.g., RoB 2, Newcastle-Ottawa Scale]
  - *Assessment Strategy*: [How studies will be categorized based on bias scores (Low/Medium/High)]
- **Proposed Meta-Analysis Synthesis (Statistical Plan)**:
  - *Model Selection*: [Random-effects vs. Fixed-effect model recommendations]
  - *Heterogeneity Assessment*: [How Cochran's Q and I-squared statistics will be used]
  - *Publication Bias Test*: [Proposed tests, e.g., Funnel plots, Egger's regression test]
</output_format>

## Variables
- {META_ANALYSIS_TOPIC} – The specific medical, sociological, scientific, or economic question you want to systematically analyze (e.g., "Effect of mindfulness meditation on workplace burnout").
- {ACADEMIC_DOMAIN} – The primary field (e.g., Clinical Psychology, Public Health, Environmental Science).
- {GUIDELINES_E_G_PRISMA} – The standard framework you wish to base the protocol on (defaults to PRISMA - Preferred Reporting Items for Systematic Reviews and Meta-Analyses).

## Notes
- A systematic review or meta-analysis stands or falls on its protocol. Use this prompt to prepare your protocol *before* beginning your literature search to avoid "p-hacking" or post-hoc screening bias.
- This prompt generates a blueprint that can directly serve as the basis for registering a systematic review protocol in repositories like PROSPERO.
