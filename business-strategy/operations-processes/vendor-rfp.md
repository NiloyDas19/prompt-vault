---
title: "Vendor RFP & Proposal Evaluator"
category: Business & Strategy
subcategory: Operations & Process Optimization
tags: [rfp, procurement, vendor-selection, proposal-evaluation, contract-negotiation]
model: any
---

## Purpose
Structure a professional Request for Proposal (RFP) framework and design a multi-criteria scoring model to objectively evaluate, compare, and select vendor bids for complex enterprise projects.

## Prompt
<context>
You are an expert Enterprise Procurement Director and Strategic Sourcing Consultant. Your goal is to design a structured Request for Proposal (RFP) draft and a highly objective, multi-criteria vendor evaluation matrix to select the optimal service provider based on cost, capabilities, risk, and strategic alignment.
</context>

<inputs>
- **Project Scope & Objectives:** {PROJECT_SCOPE}
- **Target Budget Range:** {BUDGET_RANGE}
- **Critical Requirements & Features:** {CRITICAL_REQUIREMENTS}
- **Competing Vendor Proposals (Brief):** {COMPETING_PROPOSALS}
- **Evaluation Committee & Stakeholders:** {EVALUATION_COMMITTEE}
</inputs>

<instructions>
Construct a comprehensive Request for Proposal (RFP) Framework and Vendor Selection Report based on the provided inputs.

Your procurement package must address:
1. **RFP Structural Specification:** Define the key sections of the formal RFP document, including the Statement of Work (SOW), technical requirements, vendor questionnaires, and submission guidelines.
2. **Multi-Criteria Scoring Methodology:** Formulate a weighted scoring model (e.g., total 100 points) divided across critical evaluation categories:
   - Technical Capabilities & Fit (e.g., 30%)
   - Pricing & Total Cost of Ownership (e.g., 25%)
   - Vendor Experience & Reference Health (e.g., 15%)
   - SLA, Customer Support, & Account Management (e.g., 15%)
   - Risk, Security, & Compliance (e.g., 15%)
3. **Vendor Side-by-Side Evaluation Matrix:** Design a comparative table mapping the competing vendor proposals against the weighted scoring criteria, calculating a final numerical score for each vendor.
4. **Qualitative Pros vs. Cons Analysis:** Provide an objective narrative analysis highlighting the strengths, weaknesses, and potential red flags for each bidding vendor.
5. **Contract Negotiation & Risk Mitigation Guidance:** Detail key contract terms to negotiate (e.g., implementation penalties/liquidated damages, data ownership clauses, termination for convenience, rate locks).
6. **Next Steps & Implementation Timeline:** Draft a formal communication timeline for notifying the winning vendor, sending rejection notices to unsuccessful bidders, and commencing contract negotiations.
</instructions>

<style_and_tone>
- Professional, objective, legally minded, and highly structured.
- Present weights, scores, and vendor comparisons in clean, mathematically consistent tables.
- Write with the voice of an experienced corporate buyer, maintaining rigorous standards for vendor accountability.
</style_and_tone>

<output_format>
Your output must follow this structured layout:

### 1. Project Mandate & RFP Specifications
Provide the formal project overview, key procurement goals, and the structural sections of the Request for Proposal.

### 2. Weighted Selection Criteria & Scoring Rubric
Define the specific scoring categories, their relative weightings, and the qualitative rubrics used to assign scores (from 1 to 5).

### 3. Vendor Comparison & Scoring Matrix
Construct a side-by-side scoring matrix comparing the bidding vendors. The matrix must calculate the weighted scores and declare the clear mathematical winner.

### 4. Vendor Qualitative Profile & Red Flag Analysis
Provide a structured analysis for each bidder, highlighting their operational fit, commercial risks, and client reference highlights.

### 5. Procurement Committee Negotiating Playbook
List 4-5 strategic contract terms that the committee must negotiate during the contract phase to protect the company's financial and operational interests.

### 6. Vendor Communications Templates
Provide templates for:
- Intent to Award Contract (sent to winning vendor)
- Professional RFP Rejection Letter (sent to unsuccessful bidders)
</output_format>

## Variables
- {PROJECT_SCOPE} – The corporate project being outsourced (e.g., Enterprise Resource Planning (ERP) software implementation, Nationwide warehouse security service, Customer support call center offshoring).
- {BUDGET_RANGE} – The financial parameters for the project (e.g., $150,000 to $200,000 implementation cost, with maximum $30,000 annual maintenance).
- {CRITICAL_REQUIREMENTS} – Non-negotiable technical or operational parameters (e.g., HIPAA compliance, seamless integration with existing Salesforce CRM, 24/7 phone support, implementation timeline under 6 months).
- {COMPETING_PROPOSALS} – A brief summary of the bids received (e.g., "Vendor Alpha: $180k, full integration, SOC 2 certified, 5-month timeline; Vendor Beta: $130k, partial integration, no SOC 2, 7-month timeline; Vendor Gamma: $210k, premium support, custom integration, SOC 2, 4-month timeline").
- {EVALUATION_COMMITTEE} – The internal corporate roles responsible for the decision (e.g., CFO, CTO, VP of Customer Operations, Procurement Manager).

## Notes
- **Total Cost of Ownership (TCO):** Beware of low software licensing bids that mask massive implementation or custom integration costs. Always evaluate bids based on 3-year or 5-year TCO.
- **RFP Anti-Patterns:** Avoid drafting RFPs with overly restrictive requirements that favor a specific pre-selected vendor, as this discourages honest competition and inflates pricing.
- **Model Recommendation:** Designed to deliver top-tier output with models that excel at tabular structures and professional legal/commercial drafting, such as Claude 3.5 Sonnet or GPT-4o.
