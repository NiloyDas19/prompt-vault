---
title: "Logical Argument Reconstruction Parser"
category: Research & Analysis
subcategory: Literature & Source Analysis
tags: [argumentation, formal-logic, logical-fallacies, critical-analysis]
model: any
---

## Purpose
To parse a complex academic argument, extract its core premises and conclusions, reconstruct it into a formal logical structure, and audit it for unstated assumptions and logical fallacies.

## Prompt
<context>
You are an expert formal logician, analytical philosopher, and critical discourse analyst. Your task is to dissect the provided text, stripping away rhetorical flourishes to reveal, map, and evaluate its core logical architecture.
</context>

<instructions>
1. **Analyze the Source Text**: Carefully read the text provided under `<source_text>` to understand the main thesis and the supporting arguments.
2. **Reconstruct the Core Argument**:
   - Identify the primary **Conclusion** (the central claim the author is trying to prove).
   - Identify the explicit **Premises** (the evidence, assertions, or statements supporting the conclusion).
   - State the argument in a formal, step-by-step numbered format (e.g., Premise 1, Premise 2, Conclusion).
3. **Expose Implicit Assumptions**: Identify the hidden, unstated, or taken-for-granted assumptions that must be true for the premises to successfully lead to the conclusion.
4. **Audit for Logical Fallacies & Weaknesses**:
   - Check for formal fallacies (e.g., affirming the consequent) and informal fallacies (e.g., straw man, false dilemma, ad hominem, begging the question).
   - Evaluate the validity (does the conclusion logically follow from the premises?) and soundness (are the premises actually true/supported by empirical evidence?).
5. **Formulate a Structural Map**: Outline the argumentative flow and present the final evaluation in the exact format defined in `<output_format>`.
</instructions>

<source_text>
{SOURCE_TEXT_TO_PARSE}
</source_text>

<output_format>
### Logical Argument Reconstruction & Analysis

#### 1. Core Thesis & Conclusion
- **Primary Claim/Conclusion**: [State the ultimate conclusion in 1-2 clear, precise sentences]
- **Target Audience/Context**: [Briefly describe the rhetorical context of the argument]

#### 2. Formal Argument Reconstruction
- **Premise 1**: [Explicit premise statement]
- **Premise 2**: [Explicit premise statement]
- **Premise 3**: [Explicit premise statement, add more if necessary]
- **Conclusion (C)**: [Therefore, C...]

#### 3. Unstated (Implicit) Assumptions
- **Assumption A**: [State the hidden assumption and explain why the argument depends on it]
- **Assumption B**: [State another hidden assumption, if applicable]
- **Implications**: [What happens to the argument if these assumptions are proven false?]

#### 4. Logical Fallacies & Structural Weaknesses
- **Identified Fallacies**: [List and define any logical fallacies observed in the text, quoting the specific passage]
- **Validity & Soundness Review**:
  - **Validity**: [Does the argument form hold together logically? Yes/No, explain]
  - **Soundness**: [Are the premises empirically and factually robust? Yes/No, explain]
- **Counter-Argument Analysis**: [Formulate the most devastating counter-argument that directly attacks one of the key premises or assumptions]

#### 5. Argumentative Strength Assessment
- **Overall Rating**: [Strong / Moderate / Weak]
- **Summary Critique**: [A concise summary paragraph evaluating the intellectual rigor and persuasive power of the argument]
</output_format>

## Variables
- {SOURCE_TEXT_TO_PARSE} – The specific excerpt, article, essay, or argumentative section of a paper that you want to logically dissect.

## Notes
- This prompt is highly useful for reviewing peer comments, preparing counter-arguments, writing critical essays, and evaluating theoretical foundations of research.
- If the source text contains multiple distinct arguments, instruct the model to parse the *primary* argument first, or specify which sub-argument you want reconstructed.
