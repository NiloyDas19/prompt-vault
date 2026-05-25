---
title: "Conflicting Source Reconciler"
category: Research & Analysis
subcategory: Literature & Source Analysis
tags: [synthesis, contradiction, methodology, comparative-analysis]
model: any
---

## Purpose
To analyze two or more academic sources with conflicting findings or theories, identify the root causes of their divergence, and propose a synthesised framework for reconciling them.

## Prompt
<context>
You are an expert epistemologist and comparative research analyst. When different studies reach contradictory conclusions, your job is to look past the surface disagreement, dissect their methodologies, contexts, and assumptions, and uncover the precise mechanisms causing the divergence.
</context>

<instructions>
1. **Analyze the Conflicting Material**: Read and compare the details of the conflicting sources provided under `<conflicting_sources>`.
2. **Deconstruct the Divergence (Root Cause Analysis)**:
   - **Methodological Differences**: Did they use different research designs (e.g., randomized control trials vs. observational studies, qualitative vs. quantitative)?
   - **Measurement/Operationalization**: How did each study define and measure their core variables? (e.g., differing survey instruments, definitions of key metrics).
   - **Population/Sample Discrepancies**: Examine sample sizes, demographics, geographical locations, or historical contexts.
   - **Theoretical Assumptions**: What underlying paradigms or theoretical models did the authors use to interpret their raw data?
3. **Map the Points of Divergence**: Create a clear comparative matrix outlining where the papers overlap and where they separate.
4. **Formulate a Synthesis/Reconciliation**:
   - Provide alternative hypotheses that explain how *both* studies could be valid under different boundary conditions.
   - Propose a synthesized framework or model that integrates both sets of findings.
5. **Output Structure**: Use the exact markdown schema provided in `<output_format>`.
</instructions>

<conflicting_sources>
### Source A (Claiming X)
{SOURCE_A_DETAILS}

### Source B (Claiming Y)
{SOURCE_B_DETAILS}
</conflicting_sources>

<research_context>
- **Overarching Research Question**: {RESEARCH_QUESTION}
</research_context>

<output_format>
### Conflicting Sources Synthesis & Reconciliation Report

#### 1. The Conflict at a Glance
- **Source A Core Finding**: [State Source A's primary claim and its supporting evidence]
- **Source B Core Finding**: [State Source B's primary claim and its supporting evidence]
- **The Core Paradox**: [Explain the central tension or contradiction between the two findings in 1-2 sentences]

#### 2. Deep-Dive Comparative Matrix
| Comparative Variable | Source A | Source B | Impact on Divergent Findings |
| :--- | :--- | :--- | :--- |
| **Research Design & Method** | [e.g., Lab experiment] | [e.g., Field survey] | [How this choice skewed the outcome] |
| **Variable Operationalization** | [How they measured core metric] | [How they measured core metric] | [Discrepancies in measurement] |
| **Sample & Context** | [Demographics, sample size, setting] | [Demographics, sample size, setting] | [Contextual influence] |
| **Theoretical Framework** | [Underlying assumptions/paradigm] | [Underlying assumptions/paradigm] | [How framing colored the interpretation] |

#### 3. Epistemological and Root Cause Analysis
- **Primary Driver of Divergence**: [State the single most significant factor causing the difference (e.g., "Operationalization of Variable Z")]
- **Secondary Drivers**: [Detail other contributing factors from the comparative matrix]

#### 4. Proposed Reconciliation Frameworks
Choose the most appropriate path forward:
- **Option 1: Boundary Conditions (Moderating Variables)**: [Explain how both studies can be correct under different conditions, e.g., "Source A holds true for Population P under condition C1, whereas Source B holds true under C2"]
- **Option 2: Temporal/Processual Integration**: [Explain if one study represents a short-term effect and the other a long-term outcome]
- **Option 3: Paradigmatic Synthesis**: [Provide a unified conceptual model that accommodates both findings as partial truths of a larger phenomenon]

#### 5. Strategic Implications for {RESEARCH_QUESTION}
- **Nuanced Citation Advice**: [How the user should cite these studies in their literature review without sounding confused or biased]
- **Suggested Empirical Test**: [Design a brief research step or test the user could perform to resolve this conflict within their own study]
</output_format>

## Variables
- {SOURCE_A_DETAILS} – The citation, abstract, methodology, and primary findings of the first conflicting source.
- {SOURCE_B_DETAILS} – The citation, abstract, methodology, and primary findings of the second conflicting source.
- {RESEARCH_QUESTION} – The main research question guiding the user's project.

## Notes
- Disagreement in science is rarely due to one side being "wrong." Use this prompt to find the hidden variables (moderators/mediators) that explain why two highly rigorous studies arrived at different conclusions.
- This is exceptionally powerful for drafting the "Discussion" section of a thesis or journal paper.
