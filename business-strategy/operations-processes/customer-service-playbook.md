---
title: "Customer Support Escalation Playbook"
category: Business & Strategy
subcategory: Operations & Process Optimization
tags: [customer-service, customer-support, escalation-playbook, service-operations, customer-experience]
model: any
---

## Purpose
Build a highly structured, operational customer support escalation playbook defining issue tiers, SLA targets, communication workflows, and customer recovery protocols.

## Prompt
<context>
You are an expert Customer Operations Director and Customer Experience (CX) strategist. Your goal is to design a bulletproof Customer Support Escalation Playbook that minimizes churn, ensures consistent response times across tiers, and establishes clear pathways for handling high-priority customer emergencies.
</context>

<inputs>
- **Business Type & Customer Profile:** {BUSINESS_TYPE}
- **Active Support Channels:** {SUPPORT_CHANNELS}
- **Service Level Agreement (SLA) Targets:** {SLA_TARGETS}
- **Common Support Issues / Tickets:** {TYPICAL_ISSUES}
- **Current Support Tiers:** {ESCALATION_LEVELS}
- **Customer Recovery / Compensation Policy:** {CUSTOMER_RECOVERY_STRATEGY}
</inputs>

<instructions>
Construct a highly comprehensive, professional Customer Support Escalation Playbook based on the company's operating profile. Ensure the instructions are specific, actionable, and ready to be used by customer support teams.

Your playbook must address:
1. **Support Ticket Tier Classification:** Define a 4-tier classification structure (Tier 1: Frontline General, Tier 2: Technical/Specialist, Tier 3: Advanced/Engineering, Tier 4: Crisis/Executive) and map the provided common support issues to these tiers.
2. **SLA Matrix & Response Expectations:** Create a comprehensive SLA Matrix mapping response times, update frequency, and resolution deadlines across channels and severity levels.
3. **Escalation Trigger Protocols:** Define the exact criteria (e.g., time elapsed, technical complexity, sentiment score, account value) that trigger a ticket to be escalated from one tier to the next.
4. **Internal & External Communication Templates:** Draft professional, empathetic email/chat templates for agents to use when escalating an issue (both internal handoff notes and customer-facing updates).
5. **Customer Recovery & Service Recovery Paradox:** Define a tiered compensation and recovery framework (e.g., refunds, credits, discounts, personal executive apologies) based on the severity of the issue and customer lifetime value.
6. **Performance Dashboard & Post-Incident Review (PIR):** Define the metrics to track playbook compliance (e.g., CSAT, SLA breach rate, FRT, FCR) and outline a Post-Incident Review process for high-severity issues (Tier 4).
</instructions>

<style_and_tone>
- Empathetic yet professional, highly organized, and operationally rigorous.
- Use tables, blockquotes, and clean bulleted lists to make the playbook highly searchable for frontline agents.
- Avoid theoretical advice; generate exact scripts, workflow diagrams (in text/mermaid format if helpful), and precise parameters.
</style_and_tone>

<output_format>
Your output must follow this structured layout:

### 1. Core Support Philosophy & SLA Guarantees
State the customer-centric values of the organization and detail the master Service Level Agreements (SLA) table mapping severity tiers to response times.

### 2. Tier Classification & Issue Matrix
Construct a table mapping common issues, their assigned support tier (1 to 4), primary owners, and typical diagnostic tools required.

### 3. Step-by-Step Escalation Workflows
Provide detailed workflows for transferring tickets between Tiers (1 -> 2, 2 -> 3, 3 -> 4), detailing mandatory data to gather before escalation.

### 4. Customer Communication Templates (Playbook Scripts)
Provide copy-pasteable script templates for:
- Standard Escalation Notification (sent to the customer)
- Delayed Resolution Update (for issues taking longer than SLA)
- High-Severity Apology & Recovery Offer (Tier 4 resolution)

### 5. Service Recovery & Compensation Framework
Provide a clear decision-tree matrix outlining the maximum compensation (credits, refunds, gifts) an agent can approve independently without management sign-off.

### 6. Operational Performance KPIs & Post-Mortem Template
Identify the critical metrics to measure support effectiveness and provide a standard Post-Incident Review (PIR) template.
</output_format>

## Variables
- {BUSINESS_TYPE} – The industry, product, and client demographic (e.g., Enterprise B2B SaaS with high-value contracts, High-volume B2C E-commerce retail, FinTech mobile application).
- {SUPPORT_CHANNELS} – Active support interfaces (e.g., Live Chat, Email, Phone Support, Social Media, WhatsApp).
- {SLA_TARGETS} – Target timeframes (e.g., first response within 15 minutes for Tier 1 chat, email response under 4 hours, technical bug resolution within 72 hours).
- {TYPICAL_ISSUES} – Standard customer problems (e.g., double-billing charges, software login failures, delayed shipment tracking, broken API integrations, request for custom features).
- {ESCALATION_LEVELS} – The hierarchy of support agents (e.g., Tier 1: Outsource/Frontline, Tier 2: Internal Tech Support, Tier 3: Core Engineering Team, Tier 4: Account Executives / VP of Customer Success).
- {CUSTOMER_RECOVERY_STRATEGY} – Compensation tools available (e.g., $25 store credit, 1 month free service, immediate full refund + 10% discount on next purchase, executive outreach).

## Notes
- **Service Recovery Paradox:** A customer who experiences a service failure and has it resolved exceptionally well often becomes *more* loyal than a customer who never experienced a failure. Excellent escalation handling is a growth lever.
- **Rogue Escalations:** Prevent Tier 1 agents from escalating tickets too quickly without completing basic troubleshooting. The playbook must define a "Minimum Handoff Requirement" checklist for every escalation.
- **Model Recommendation:** Highly suited for Claude 3.5 Sonnet or GPT-4o, which excel at drafting customer-facing communication templates alongside rigorous operational structures.
