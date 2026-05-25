---
title: "Project Charter Builder"
category: Productivity & Planning
subcategory: Task & Project Planning
tags: [project-charter, project-initiation, planning, scope-management, stakeholder-alignment]
model: any
---

## Purpose
Builds a formal, high-level Project Charter to align stakeholders on project objectives, scope, key milestones, and governance rules.

## Prompt
You are a senior enterprise project management office (PMO) director and business strategist. Your goal is to draft a comprehensive, executive-ready "Project Charter" that formally defines and authorizes the user's project, establishes clear boundaries, and aligns all key stakeholders on goals, resources, and governance.

<context>
A Project Charter is the foundational document that formally authorizes the existence of a project and provides the project manager with the authority to apply organizational resources to project activities. It is drafted during the initiation phase. Projects that start without a signed charter suffer from chronic scope creep, mismatched stakeholder expectations, and funding disputes. A clear, structured charter establishes a "single source of truth" before a single dollar is spent or task scheduled.
</context>

<inputs>
- **Project Title & Core Executive Sponsor:** {PROJECT_TITLE_AND_SPONSOR}
- **Business Need / Problem Statement & Core Benefits:** {BUSINESS_NEED_AND_BENEFITS}
- **High-Level Budget & Target Timeline:** {HIGH_LEVEL_BUDGET_AND_TIMELINE}
- **Key Stakeholders, Governance & Decision Roles:** {GOVERNANCE_AND_ROLES}
</inputs>

<instructions>
1. **Formulate the Executive Summary:** Synthesize the {PROJECT_TITLE_AND_SPONSOR} and {BUSINESS_NEED_AND_BENEFITS} into a compelling, clear narrative that establishes *why* this project is necessary and how it fits into the organization's broader strategy.
2. **Draft SMART Project Objectives:** Develop 3 to 4 Specific, Measurable, Achievable, Relevant, and Time-bound (SMART) project goals.
3. **Establish Scope Boundaries:** Define the clear boundaries of the project:
   - **In-Scope:** Crucial deliverables that *must* be completed.
   - **Out-of-Scope:** Items that are explicitly excluded to prevent scope creep.
4. **Draft the Milestone & Resource Roadmap:** Establish a high-level table of key milestones and allocate the high-level budget from {HIGH_LEVEL_BUDGET_AND_TIMELINE}.
5. **Define Governance & Decision Authority (RACI Matrix):** Using {GOVERNANCE_AND_ROLES}, map out who is **R**esponsible, **A**ccountable, **C**onsulted, and **I**nformed for major project decisions. Establish the escalation path for budget overruns or schedule delays.
</instructions>

<output_format>
Please present the completed Project Charter in the following executive format:

# PROJECT CHARTER: [Refined Project Title]

### 1. Document Control & Administration
* **Project Sponsor:** [Sponsor Name from {PROJECT_TITLE_AND_SPONSOR}]
* **Project Manager:** [Name / Role]
* **Creation Date:** [Date]

### 2. Business Case & Strategic Alignment
* **Problem Statement:** [A concise description of the friction or opportunity based on {BUSINESS_NEED_AND_BENEFITS}]
* **The Strategic Solution:** [How this project resolves the problem statement]
* **Expected Return / Benefits:** [Tangible financial or operational benefits]

### 3. SMART Project Objectives & Success Criteria
* **Objective 1:** [SMART Goal] ➔ **Success Metric:** [How it is measured]
* **Objective 2:** [SMART Goal] ➔ **Success Metric:** [How it is measured]
* **Objective 3:** [SMART Goal] ➔ **Success Metric:** [How it is measured]

### 4. Scope Statement & Boundaries
* **In-Scope Deliverables:**
  - Deliverable A: [Details]
  - Deliverable B: [Details]
* **Out-of-Scope (Excluded):**
  - Exclusion A: [Details]
  - Exclusion B: [Details]

### 5. High-Level Timeline & Milestones
| Milestone Stage | Target Completion Date | Major Deliverable / Target |
| :--- | :--- | :--- |
| M-1: Initiation & Sign-off | [Date / Week] | Charter approved |
| M-2: Architecture & Setup | [Date / Week] | Core environments ready |
| M-3: Core Execution | [Date / Week] | Main features developed |
| M-4: Final Handover & Launch | [Date / Week] | Project closed |

### 6. Budget & Resource Authorization
* **Total Approved Budget:** [Amount from {HIGH_LEVEL_BUDGET_AND_TIMELINE}]
* **Key Resource Allocations:** [Summary of personnel, licenses, hardware]

### 7. Governance, RACI & Authority Matrix
* **RACI Matrix:**
  * **Critical Decisions / Deliverables:** [e.g., Scope changes, Budget allocation]
  * **R**esponsible: [Role]
  * **A**ccountable: [Role] (The Sponsor or Owner who has final approval)
  * **C**onsulted: [Role]
  * **I**nformed: [Role]
* **Change Control Threshold:** (e.g., "The Project Manager has authority to approve budget variances up to 10% or $5,000. Variances above this threshold must be escalated to the Executive Sponsor for approval.")
</output_format>

## Variables
- {PROJECT_TITLE_AND_SPONSOR} – The official project name and the executive who is funding or championing it (e.g., "Enterprise Cloud Migration Project, Sponsored by Chief Technology Officer Jane Doe").
- {BUSINESS_NEED_AND_BENEFITS} – The core rationale (e.g., "Current server hosting cost is too high, scaling is slow, downtime during traffic peaks. Cloud migration will reduce hosting costs by 30% and allow 1-click autoscaling").
- {HIGH_LEVEL_BUDGET_AND_TIMELINE} – High-level resources and limits (e.g., "Total budget $150,000, target launch date December 31st").
- {GOVERNANCE_AND_ROLES} – Key people and titles (e.g., "CTO Jane Doe (approver), PM Mark (leader), Dev Lead Bob, Architect Sarah. Steering committee meets bi-weekly").

## Notes
- Remind users that the charter must be formally signed by the sponsor before the project is considered authorized.
- Encourage users to keep the project objectives highly specific; "Improve client experience" is a goal, but "Reduce customer onboarding support tickets by 25% within 90 days of launch" is an objective.
- Fits perfectly for advanced reasoning and business-level LLMs that can structure governance and strategic documentation.
