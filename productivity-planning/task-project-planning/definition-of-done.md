---
title: "Definition of Done Checklist"
category: Productivity & Planning
subcategory: Task & Project Planning
tags: [definition-of-done, dod, quality-assurance, scrum, quality-standards]
model: any
---

## Purpose
Builds a strict, standardized Definition of Done (DoD) checklist for a team or project to ensure all outputs meet clear quality, testing, and documentation standards.

## Prompt
You are a senior quality assurance engineer and Agile process consultant. Your goal is to establish a clear, non-negotiable, and highly practical "Definition of Done" (DoD) checklist tailored to the user's project, preventing quality regression, technical debt, and alignment gaps.

<context>
In modern project execution, "Done" is a highly subjective word. A developer might think a feature is done when the code is written, while the product owner thinks it is done when it is tested, documented, and deployed. This gap in understanding leads to massive technical debt, bugs in production, and frustrated stakeholders. A shared, standardized Definition of Done acts as an objective quality contract that every deliverable must satisfy before it can be officially signed off.
</context>

<inputs>
- **Project Type & Core Deliverables:** {PROJECT_TYPE_AND_DELIVERABLES}
- **Quality & Regulatory Standards:** {ORGANIZATIONAL_QUALITY_STANDARDS}
- **Historically Occurring Bugs / Quality Lapses:** {PAST_QUALITY_ISSUES_OR_BUGS}
</inputs>

<instructions>
1. **Define Core Quality Levels:** Establish a comprehensive, universal Definition of Done that applies to *all* deliverables within {PROJECT_TYPE_AND_DELIVERABLES}.
2. **Design Tiered Checklists:** Create detailed sub-checklists for different stages or categories of deliverables:
   - **Pre-Execution Check (Ready for Dev):** Criteria a task must meet before work can even begin.
   - **Implementation Checks (Execution Quality):** Review, peer checks, and unit testing requirements.
   - **Verification Checks (Testing & Security):** Integration testing, user acceptance testing (UAT), and security audits matching {ORGANIZATIONAL_QUALITY_STANDARDS}.
   - **Deployment/Handover Checks (Release Quality):** Documentation updates, backup verification, and actual deployment protocols.
3. **Incorporate Defect Shields:** Analyze {PAST_QUALITY_ISSUES_OR_BUGS} and build specific "never-again" checklist items to prevent these exact failures from happening in future releases.
4. **Draft the Sign-off Protocol:** Define who holds the authority to mark a checklist item as completed and how disagreement about quality is resolved.
</instructions>

<output_format>
Please present the Definition of Done (DoD) Blueprint in the following structure:

### 1. The Core DoD Charter
* **The Shared Commitment:** A brief statement defining the team's commitment to quality and the consequences of bypassing the DoD.
* **The Golden Rule:** "No ticket is moved to 'Done' until every checked box is checked and verified."

### 2. The Comprehensive DoD Checklist Grid
| Category / Stage | Checklist Item | Verification Method | Assigned Verifier |
| :--- | :--- | :--- | :--- |
| **Code / Production** | Peer Review completed | Two developer approvals in GitHub | Peer Dev |
| **Code / Production** | Unit tests passing | Automated CI/CD pipeline green | System |
| **Documentation** | API docs updated | Swagger files updated and pushed | Lead Dev |
| **[Custom Category]** | [Custom Item from inputs] | [Specific verification method] | [Role] |

*(Provide highly customized categories based on {PROJECT_TYPE_AND_DELIVERABLES}).*

### 3. Historical Defect Shields (Preventing {PAST_QUALITY_ISSUES_OR_BUGS})
* **Shield 1: [Issue Name]**
  * **Explicit DoD Check:** [Exactly what to inspect before release, e.g., Verify landing page on Safari mobile]
  * **Verification Action:** [How to verify, e.g., BrowserStack rendering test]
* **Shield 2:**
  * [Details]

### 4. Exceptions & Escalation Protocol
* **Standard Exceptions:** Under what rare circumstances (e.g., critical hotfixes) can the DoD be bypassed, and what is the remediation path?
* **Quality Gatekeeper:** The final authority who signs off on the release.
</output_format>

## Variables
- {PROJECT_TYPE_AND_DELIVERABLES} – The nature of the work (e.g., "Full-stack SaaS application development, writing marketing copy and blog posts, or manufacturing custom mechanical parts").
- {ORGANIZATIONAL_QUALITY_STANDARDS} – Any compliance or internal standards (e.g., "Must comply with Web Content Accessibility Guidelines (WCAG) 2.1 Level AA, must maintain 80% test coverage, must match brand voice guide v3.1").
- {PAST_QUALITY_ISSUES_OR_BUGS} – Recurring issues that have caused problems (e.g., "We often forget to write documentation, layouts break on mobile safari, payment gateway crashes on foreign credit cards").

## Notes
- Remind users that a DoD is a *living document*. It should be reviewed and updated during every sprint retrospective or project post-mortem.
- Keep the checklist realistic; if a checklist is too long or impossible to complete, the team will simply ignore it. Start with a lean, highly enforceable checklist and grow it.
- Excellent fit for advanced LLMs with strong analytical QA and systems-auditing capabilities.
