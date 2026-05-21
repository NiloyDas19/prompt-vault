---
title: "Deal Review & Pipeline Analyzer"
category: Marketing & Sales
subcategory: Sales
tags: [sales, pipeline, deal-review, forecasting, strategy]
model: any
---

## Purpose
Analyze a specific deal or pipeline to identify risks, suggest next steps, and improve deal velocity and win rate.

## Prompt
Help me analyze this deal and develop a strategy to move it forward. Be honest — tell me if this deal is healthy or if I'm wasting my time.

**Deal Information:**
- Prospect: {PROSPECT_COMPANY}
- Contact: {CONTACT_NAME}, {CONTACT_TITLE}
- Deal size: {DEAL_SIZE}
- Product: {PRODUCT}
- Current stage: {PIPELINE_STAGE}
- Days in pipeline: {DAYS_IN_PIPELINE}
- Average deal cycle: {AVERAGE_CYCLE}
- Competitor in the deal: {COMPETITOR}
- Champion identified: {CHAMPION}
- Economic buyer identified: {ECONOMIC_BUYER}
- Next scheduled meeting: {NEXT_MEETING}
- Last meaningful interaction: {LAST_INTERACTION}

### Analysis:

**1. Deal Health Score (1–10)**
- Score the deal based on the information provided
- List the positive signals and red flags
- Compare timeline to average deal cycle — is it on track?

**2. MEDDIC Assessment**
- **Metrics**: Is there a quantified business case?
- **Economic Buyer**: Have you identified and engaged the person who signs the check?
- **Decision Criteria**: Do you know exactly how they'll decide?
- **Decision Process**: Do you know the steps and timeline to close?
- **Identify Pain**: Is the pain urgent and quantified?
- **Champion**: Do you have an internal advocate who is selling for you when you're not in the room?
For each: Red / Yellow / Green assessment with specific recommendation.

**3. Risk Factors**
- What could kill this deal?
- What's the prospect's "do nothing" alternative?
- What haven't you confirmed that you should have?

**4. Recommended Next Steps**
- The single most important action to take this week
- 3 specific steps to advance the deal to the next stage
- Who else at the company should you engage?
- What content, case study, or resource to send?

**5. Closing Strategy**
- Recommended closing approach for this deal type
- Timeline to decision — is there a natural deadline or event to anchor to?
- How to create urgency without being pushy

## Variables
- {PROSPECT_COMPANY} – The company
- {CONTACT_NAME} – Your main contact
- {CONTACT_TITLE} – Their title
- {DEAL_SIZE} – Estimated deal value
- {PRODUCT} – What you're selling
- {PIPELINE_STAGE} – Current stage (e.g., "Discovery", "Proposal Sent", "Negotiation")
- {DAYS_IN_PIPELINE} – How long the deal has been open
- {AVERAGE_CYCLE} – Your typical sales cycle
- {COMPETITOR} – Who you're competing against
- {CHAMPION} – Whether you have an internal champion (yes/no/uncertain)
- {ECONOMIC_BUYER} – Whether you've met the decision-maker (yes/no/uncertain)
- {NEXT_MEETING} – When you're meeting next (or "none scheduled")
- {LAST_INTERACTION} – When you last had a meaningful exchange

## Notes
- If you can't identify a champion and an economic buyer, the deal is at high risk regardless of how positive the conversations feel.
- "No decision" is your biggest competitor. Most lost deals aren't lost to competitors — they're lost to inertia.
- A deal with no next meeting scheduled is a dead deal. Always leave every interaction with the next step calendared.
