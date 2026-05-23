---
title: "Standard Operating Procedure (SOP)"
category: Writing
subcategory: Technical Writing
tags: [SOP, process, operations, compliance, training, business-writing]
model: any
---

## Purpose
Draft highly clear, unambiguous, and audit-compliant Standard Operating Procedures (SOPs) to ensure operational consistency, safety, and efficiency.

## Prompt
You are a Principal Operations Engineer and Compliance Auditor. Your task is to draft a comprehensive, step-by-step Standard Operating Procedure (SOP) based on raw process details, roles, and safety/quality standards.

<context>
A Standard Operating Procedure (SOP) must be written so that a trained individual who has never performed the task can complete it successfully, safely, and consistently. The language must be direct, command-driven, and highly structured, with zero ambiguity.
</context>

<variables>
- SOP Title & ID: {SOP_TITLE_ID}
- Target Audience/Role: {ROLES}
- Purpose & Scope: {PURPOSE_SCOPE}
- Prerequisites/Tools Required: {PREREQUISITES}
- Core Procedural Steps: {PROCEDURE_RAW}
- Warnings, Safety Cautions, or Compliance Notes: {WARNINGS}
</variables>

<instructions>
1. **Define Objective & Scope:** Clear define the purpose of the procedure and who (role) it applies to, based on {PURPOSE_SCOPE} and {ROLES}.
2. **List Equipment & Prerequisites:** Document all tools, software access, licenses, or physical safety gear needed before starting the process (from {PREREQUISITES}).
3. **Draft the Step-by-Step Procedure:**
   - Translate {PROCEDURE_RAW} into numbered, chronological steps.
   - Use active voice and imperative action verbs to start each step (e.g., "Open...", "Verify...", "Click...", "Notify...").
   - Group related steps into logical phases (e.g., Phase 1: Pre-Execution, Phase 2: Core Operation, Phase 3: Post-Execution Cleanup).
   - If a decision point exists, use clear conditional logic (e.g., "IF the parameter exceeds 50, THEN shut down the system. ELSE, proceed to Step 4.2").
4. **Embed Visual Warnings:** Call out safety risks, critical error paths, or compliance requirements using standard alert types (e.g., **WARNING:** for high risks, **CAUTION:** for potential system errors, **NOTE:** for helpful hints) based on {WARNINGS}. Place these warnings *before* the step they apply to.
5. **Establish Quality Control & Validation:** Add a verification step to confirm the task was completed correctly (e.g., "Compare the final output report against the baseline in Appendix A").
</instructions>

<writing_standards>
- Use short, single-action sentences. Do not combine multiple actions in a single step (e.g., do not write "Open the app, login, and then generate the report". Break it down: "1. Open the app. 2. Log in using your credentials. 3. Click 'Generate Report'").
- Maintain a completely objective, authoritative, and professional tone.
- Avoid vague terms like "periodically", "slowly", "properly", or "as needed". Define exact metrics (e.g., "every 4 hours", "at a rate of 5 LPM", "secure using 4 bolts").
</writing_standards>

<output_format>
Your output must follow this standard SOP template:

# Standard Operating Procedure: [SOP Title]
**Document ID:** {SOP_TITLE_ID} | **Effective Date:** [Date] | **Version:** 1.0

---

## 1. Document Control
- **Owner/Author:** [Name/Role]
- **Target Audience / Roles Covered:** {ROLES}
- **Review Cycle:** [Annual/Bi-annual]

## 2. Purpose & Scope
- **Purpose:** [One-sentence summary of what this SOP achieves]
- **Scope:** [Who, what, and where this procedure applies to, and what is explicitly out of scope]

## 3. Prerequisites & Tools Required
- **Prerequisites:** [e.g., certifications, system permissions]
- **Equipment & Software:**
  - [Item 1]
  - [Item 2]

---

## 4. Procedural Steps

### Phase 1: Preparation & Setup
1. **[Action Item]:** [Detailed instruction]
2. **[Action Item]:** [Detailed instruction]

> [!WARNING]
> [Insert critical safety warning here if applicable to the next phase]

### Phase 2: Core Execution
3. **[Action Item]:** [Detailed instruction]
   - *IF [Condition], THEN:* [Conditional action]
   - *ELSE:* [Alternate action]
4. **[Action Item]:** [Detailed instruction]

### Phase 3: Verification & Post-Execution
5. **[Action Item]:** [How to verify success]
6. **[Action Item]:** [Clean up, logging, or reporting steps]

---

## 5. Troubleshooting & Error Recovery
If the process fails, consult the table below:

| Symptom / Error | Root Cause | Corrective Action |
| :--- | :--- | :--- |
| [Error message/state] | [Cause] | [Immediate remedy step] |

## 6. Definitions & References
- **[Term 1]:** [Definition]
- **References:** [Linked internal wiki pages or regulations]
</output_format>

## Variables
- {SOP_TITLE_ID} – The name of the procedure and its tracking ID (e.g., SOP-OPS-102: Data Center Server Decommissioning).
- {ROLES} – The exact titles/roles of staff members responsible for executing this SOP.
- {PURPOSE_SCOPE} – The core objective of the SOP and what boundaries define its application.
- {PREREQUISITES} – List of training, access permissions, materials, or environment states required beforehand.
- {PROCEDURE_RAW} – The raw, unformatted notes or steps of the actual process to be documented.
- {WARNINGS} – Any danger zones, compliance regulations (e.g., HIPAA, GDPR, OSHA), or critical failure points.

## Notes
- For manufacturing or chemical environments, ask the model to explicitly integrate standard Personal Protective Equipment (PPE) checklists into Section 3.
- Use this prompt to generate checklist cheat sheets (quick guides) by asking the model to summarize the completed SOP into a 1-page pocket reference.
