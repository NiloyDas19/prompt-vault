---
title: "Customer Feedback Loop Architect"
category: Business & Strategy
subcategory: Product & Innovation Strategy
tags: [customer-experience, product-management, feedback-loop, voc, nps]
model: any
---

## Purpose
Design a comprehensive, closed-loop customer feedback collection and analysis system that translates raw user input into actionable product roadmap decisions.

## Prompt
<context>
You are an expert Voice of the Customer (VoC) Architect and Customer Experience (CX) Strategist. Your goal is to construct a scalable customer feedback ecosystem that captures insights at key touchpoints, structures qualitative data, integrates feedback into the development workflow, and closes the loop by communicating updates back to the customer.
</context>

<instructions>
Using the business model and customer journey inputs, design a production-ready closed-loop feedback architecture.

Please formulate the following components:
1. **Journey Touchpoint & Collection Protocol**:
   - Identify 4-5 critical touchpoints in the customer journey (e.g., onboarding, checkout, feature adoption, support, churn).
   - For each touchpoint, specify:
     - **Feedback Mechanism**: Survey type (NPS, CSAT, CES), in-app prompt, email, or interviews.
     - **Timing & Trigger Logic**: Exactly when the feedback request is fired.
     - **Core Questions**: Specific, high-response phrasing.
2. **Data Classification & Sentiment Engine Design**:
   - Design a tagging taxonomy to categorize incoming feedback (e.g., UI/UX, Performance/Bugs, Feature Requests, Pricing/Billing, Customer Service).
   - Create a triage methodology to automatically filter and flag high-impact feedback (e.g., high churn risk, enterprise accounts, safety/security issues).
3. **Internal Triaging & Workflow Integration**:
   - Detail how feedback flows from the customer-facing tools (Intercom, Zendesk, Salesforce) into product management and engineering environments (Jira, Productboard, Notion).
   - Define a cross-functional rhythm (e.g., weekly backlog triage, monthly VoC review) and establish roles/responsibilities.
4. **Closing the Loop (Internal & External Protocols)**:
   - **Internal Protocol**: How to share insights across Sales, Marketing, and Engineering to build alignment.
   - **External Protocol (Close-the-Loop)**:
     - **For Promoters/Satisfied Users**: How to leverage them for referrals, reviews, case studies, or beta tests.
     - **For Detractors/Dissatisfied Users**: A detailed, step-by-step outreach template for customer success to resolve issues within 24 hours.
     - **Mass Communication (Public Changelog)**: Outline a strategy to communicate "We heard you, so we built this" to the general user base.
5. **Key Metrics & ROI Tracker**:
   - Establish KPIs to monitor the feedback loop’s effectiveness (e.g., feedback response rates, CSAT improvement, time-to-close feedback loops, churn reduction).
</instructions>

<business_context>
- **Product & Business Model**: {BUSINESS_MODEL}
- **Primary Customer Journey Steps**: {CUSTOMER_JOURNEY}
- **Current Tech Stack**: {FEEDBACK_TECH_STACK}
- **Core Customer Pain Points**: {KNOWN_PAIN_POINTS}
</business_context>

<style_and_tone>
Maintain a highly structured, analytical, user-empathic, and execution-oriented tone. Use tables, step-by-step workflows, and ready-to-use communication templates.
</style_and_tone>

<output_format>
Your output must be organized as follows:
1. **Executive Framework Summary**: High-level map of the feedback loop.
2. **Touchpoint Collection Map**: A detailed table highlighting Stage, Trigger, Tool, Mechanism, and Phrasing.
3. **Classification & Sentiment Tagging Taxonomy**: Standardized list of tags and categories.
4. **Internal Workflow & Alignment Blueprint**: Workflow diagram/description showing how data moves through the organization.
5. **Closing-the-Loop Playbook**: Includes active outreach templates for detractors and promoter escalation.
6. **Program KPI Dashboard**: Core metrics for measuring program success.
</output_format>

## Variables
- {BUSINESS_MODEL} – The type of business (e.g., B2B Enterprise SaaS, High-Volume E-commerce, Consumer Mobile Game, Marketplace).
- {CUSTOMER_JOURNEY} – The primary stages a user goes through (e.g., Sign-up -> Initial Setup -> Core Value Realization -> Renewal).
- {FEEDBACK_TECH_STACK} – Tools currently used (e.g., Slack, Jira, Zendesk, HubSpot, Typeform, UserVoice).
- {KNOWN_PAIN_POINTS} – Top complaints or historical issues that need immediate structural feedback loops.

## Notes
- **Closed-Loop Focus**: Avoid just collecting data; the prompt heavily emphasizes "closing the loop" by responding to detractors and updating promoters.
- **Micro-surveys**: Recommends short, high-context prompts over long annual surveys to increase response rates and accuracy.
- **Model Recommendation**: Highly suited for Claude 3.5 Sonnet or GPT-4o to write clear templates and structured data-flow protocols.
