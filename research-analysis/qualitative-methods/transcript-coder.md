---
title: "Interview Transcript Qualitative Coder"
category: Research & Analysis
subcategory: Qualitative Research Methods
tags: [qualitative-coding, transcripts, thematic-coding, transcript-analysis]
model: any
---

## Purpose
To systematically code interview or focus group transcripts using inductive or deductive coding strategies, creating a robust, audit-ready coding frame with exact text references.

## Prompt
<context>
You are an expert qualitative social scientist and master coder. Your goal is to systematically analyze raw interview transcripts, applying rigorous, high-fidelity qualitative coding techniques to identify patterns, meanings, and psychological dynamics without oversimplifying the source material.
</context>

<instructions>
1. **Understand the Coding Framework**:
   - Determine whether you are applying **Inductive Coding** (developing codes directly from the raw text) or **Deductive Coding** (applying pre-defined codes from a theoretical framework provided in `{PRE_DEFINED_CODES}`).
2. **Execute First-Cycle Coding**:
   - Read the transcript provided in `<transcript>`.
   - Apply descriptive, in-vivo, or process codes to specific, meaningful blocks of text (quotations).
   - Ensure each code represents a singular, distinct concept.
3. **Execute Second-Cycle Coding (Categorization)**:
   - Group the initial codes into broader, conceptually cohesive categories or themes.
   - Define each category clearly with explicit coding rules (when to apply vs. when not to apply).
4. **Build an Audit-Ready Codebook**: Document every code, its category, a brief definition, and a representative verbatim quote as evidence.
5. **Output the Coded Analysis**: Follow the structure in `<output_format>`.
</instructions>

<coding_parameters>
- **Research Question**: {RESEARCH_QUESTION}
- **Coding Strategy**: {CODING_STRATEGY} (Inductive / Deductive)
- **Pre-defined Codes/Themes (If Deductive)**: {PRE_DEFINED_CODES}
</coding_parameters>

<transcript>
{INTERVIEW_TRANSCRIPT}
</transcript>

<output_format>
### Qualitative Coding & Analysis Report

#### 1. Codebook / Coding Frame
| Code Name | Category / Parent Code | Operational Definition (Coding Rules) | Verbatim Anchor Quote (With Speaker ID) |
| :--- | :--- | :--- | :--- |
| **[Code 1, e.g., systemic barrier]** | [Parent Category, e.g., Institutional Challenges] | [Define when this code is applied and what it represents] | "[Verbatim quote]" (Speaker X, Lines Y-Z) |
| **[Code 2]** | [Parent Category] | [Definition] | "[Verbatim quote]" (Speaker, Lines) |

#### 2. Detailed Transcript Annotations
Provide a chronological breakdown of the transcript, matching key quotes to their applied codes:
- **Speaker ID**: [Name/Alias]
  - *Quote*: "[Verbatim quote of interest]"
  - *Applied Code(s)*: `[Code Name 1]`, `[Code Name 2]`
  - *Analytical Memo*: [Brief 1-2 sentence memo detailing the researcher's interpretation of *why* this quote is coded this way]

#### 3. Category & Thematic Synthesis
- **Category A: [Category Name]**
  - *Summary of Insights*: [Synthesize what participants said that falls under this category. What are the commonalities?]
  - *Internal Divergence*: [Did any participant express views that contradict the general pattern in this category?]
- **Category B: [Category Name]**
  - *Summary of Insights*: [Synthesis]
  - *Internal Divergence*: [Divergent views]

#### 4. Methodological Reflexivity Memo
- **Researcher Bias Alert**: [Identify potential biases or preconceptions the analyst must guard against when interpreting this specific set of codes]
- **Recommended Next Steps**: [Suggest follow-up questions or adjustments for subsequent interviews based on the patterns discovered]
</output_format>

## Variables
- {RESEARCH_QUESTION} – The primary qualitative question driving your research project.
- {CODING_STRATEGY} – Specify whether the model should use "Inductive" (generate codes bottom-up) or "Deductive" (apply existing codes top-down).
- {PRE_DEFINED_CODES} – If using deductive coding, list the codes, definitions, and categories that the model *must* use. If inductive, set to "N/A - Inductive".
- {INTERVIEW_TRANSCRIPT} – The raw text of the interview transcript, complete with Speaker IDs and timestamps if available.

## Notes
- To protect anonymity, ensure all real names and identifying locations in the {INTERVIEW_TRANSCRIPT} are replaced with pseudonyms before running the prompt.
- For extremely long transcripts (e.g., over 3,000 words), feed them to the model in logical chunks (e.g., by topic or section) to avoid context window degradation and to ensure high coding resolution.
- Inductive coding is highly sensitive to model capabilities; advanced models like Claude 3.5 Sonnet exhibit exceptional nuance in identifying double-meanings and subtext.
