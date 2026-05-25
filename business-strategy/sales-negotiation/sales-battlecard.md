---
title: "B2B Sales Battlecard Designer"
category: Business & Strategy
subcategory: Sales Strategy & Negotiation
tags: [sales-enablement, competitor-analysis, b2b-sales, sales-battlecard]
model: any
---

## Purpose
Creates a highly tactical B2B sales battlecard comparing your product/service with a key competitor to empower sales reps in live conversations.

## Prompt
```markdown
You are an expert product marketing manager and B2B sales enablement strategist. Your task is to design a highly tactical, battle-tested Sales Battlecard that empowers sales representatives to successfully position {PRODUCT_NAME} against our direct competitor, {COMPETITOR_NAME}. 

To do this, analyze the provided context, structure the battlecard using clean markdown, and ensure every section is immediately actionable during high-pressure sales calls.

<context>
- Our Product/Service: {PRODUCT_NAME}
- Our Core Value Proposition: {PRODUCT_VALUE_PROP}
- Target Audience/ICP: {TARGET_AUDIENCE}
- Key Competitor: {COMPETITOR_NAME}
- Known Competitor Strengths: {COMPETITOR_STRENGTHS}
- Known Competitor Weaknesses: {COMPETITOR_WEAKNESSES}
- Common Objection to Overcome: {COMMON_OBJECTIONS}
</context>

<instructions>
Construct the sales battlecard by adhering to the following structure and strategic principles:

1. **Quick Pitch & Hook**: Craft a 30-second conversational hook that immediately highlights {PRODUCT_NAME}'s unique advantage over {COMPETITOR_NAME} without sounding overly defensive or aggressive.
2. **Competitor Profile & Landmines**: Explain how {COMPETITOR_NAME} positions themselves, and detail 3-4 "landmines" (probing questions) that our sales reps can ask prospects to subtly expose the competitor's technical or operational weaknesses.
3. **Feature-to-Value Comparison**: Create a markdown comparison table mapping 3-4 key product areas. Contrast {COMPETITOR_NAME}'s feature-centric approach with {PRODUCT_NAME}'s business-value outcome.
4. **Objection Handling (Objection, Competitor Claim, Our Pivot)**: Provide exact, word-for-word scripts to handle {COMMON_OBJECTIONS} and competitor-planted doubts.
5. **Why We Win / Why We Lose**: Explicitly state the customer scenarios or needs where we are the clear winner, and outline the warning signs of a deal that is a better fit for the competitor, including a graceful exit/qualification-out strategy.
6. **Real-World Proof & Case Study Outline**: Describe how to leverage a customer success story or reference customer to close the loop on value.
</instructions>

<style_and_tone>
- Tone: Highly tactical, professional, confident, objective, and consultative.
- Format: Use bullet points, bold text for key phrases, and structured tables to ensure maximum readability for a salesperson multi-tasking on a call.
- Conversational Realism: Write dialogue scripts in natural, modern professional language. Avoid robotic, overly promotional corporate jargon.
</style_and_tone>

<output_format>
Your output must be structured exactly under the following markdown headers:
# SALES BATTLECARD: {PRODUCT_NAME} vs. {COMPETITOR_NAME}

## 1. The 30-Second Elevator Hook
*(Provide the exact script to open the competitive conversation)*

## 2. Competitor Positioning & Probing Landmines
- **Competitor Narrative**: *(How they sell themselves)*
- **Probing Questions to Ask the Prospect**:
  - *[Question 1]* - Why it matters: *[Context]*
  - *[Question 2]* - Why it matters: *[Context]*
  - *[Question 3]* - Why it matters: *[Context]*

## 3. Core Battleground Comparison
| Capability / Feature Area | {COMPETITOR_NAME} Approach | {PRODUCT_NAME} Advantage & Value |
| :--- | :--- | :--- |
| *[Capability 1]* | *[Competitor's way]* | *[Our value-driven solution]* |
| *[Capability 2]* | *[Competitor's way]* | *[Our value-driven solution]* |
| *[Capability 3]* | *[Competitor's way]* | *[Our value-driven solution]* |

## 4. Objection Handling Playbook
### Objection: "{COMMON_OBJECTIONS}"
- **What the Competitor Claims**: *[Their narrative]*
- **Our Tactical Pivot Script**: *"..."*

### Objection: "[Common Competitor Pricing/Feature Claim]"
- **What the Competitor Claims**: *[Their narrative]*
- **Our Tactical Pivot Script**: *"..."*

## 5. Win/Loss Qualification Matrix
### When We Win (Our Sweet Spot)
- *[Scenario 1]*
- *[Scenario 2]*

### When We Lose (Red Flags & Exit Strategy)
- *[Scenario/Red Flag 1]*
- *[Graceful exit script to maintain goodwill]*
</output_format>

Let's begin. Analyze the competitor's profile, contrast it with our value proposition, and output the ultimate, ready-to-use B2B sales battlecard.
```

## Variables
- {PRODUCT_NAME} – The name of your product, service, or company.
- {PRODUCT_VALUE_PROP} – The core value proposition, key features, or unique business outcomes your product delivers.
- {TARGET_AUDIENCE} – The Ideal Customer Profile (ICP), industry sector, or target buyer personas.
- {COMPETITOR_NAME} – The name of the specific competitor you are positioning against.
- {COMPETITOR_STRENGTHS} – Key features, brand reputations, or pricing models where the competitor holds an advantage.
- {COMPETITOR_WEAKNESSES} – Gaps in the competitor's product, poor customer support, technical limitations, or operational challenges.
- {COMMON_OBJECTIONS} – The primary competitive objection or pushback sales reps hear from prospects when compared to this competitor.

## Notes
- **Keep it updated**: Treat this battlecard as a living document. Refresh the competitor weaknesses and feature tables quarterly as software updates or market shifts occur.
- **Enablement integration**: Distribute this output via your sales enablement portal (e.g., Highspot, Seismic) or pin it within communication channels like Slack/Teams for easy access during active deals.
- **Roleplay practice**: Use this output to run practice roleplay sessions where sales managers play the role of the competitor-biased prospect, pushing reps to execute the "Tactical Pivot Script."
- **Model Recommendation**: Best used with Claude 3.5 Sonnet or GPT-4o for nuanced competitive positioning and highly realistic conversational dialogue.
