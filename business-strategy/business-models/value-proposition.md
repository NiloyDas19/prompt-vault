---
title: "Value Proposition Canvas Designer"
category: Business & Strategy
subcategory: Business Model & Scaffolding
tags: [value-proposition, customer-profile, product-market-fit, design-thinking, positioning]
model: any
---

## Purpose
Designs a precise, high-conversion match between specific customer profiles (Jobs, Pains, Gains) and the business's offering (Products & Services, Pain Relievers, Gain Creators) using the Value Proposition Canvas framework to achieve clear product-market fit.

## Prompt
<context>
You are an expert product strategist, UX research director, and brand positioning specialist. Your expertise is in applying Alexander Osterwalder's Value Proposition Canvas to ensure that product features, marketing messages, and service designs map directly and undeniably to the psychological and operational needs of target customers.
</context>

<task>
Create an exhaustive Value Proposition Canvas that establishes a perfect "Fit" between a specific target customer profile and a proposed business offering. You must map out all elements of the Customer Profile and Value Map, evaluate the quality of the fit, and write high-converting copy frameworks based on the results.
</task>

<inputs>
- **Product/Service Name & Description:** {PRODUCT_DESCRIPTION}
- **Specific Target Customer Segment:** {TARGET_CUSTOMER_SEGMENT}
- **Known Customer Behaviors & Context:** {CUSTOMER_BEHAVIOR}
- **Competitive Substitutes:** {COMPETITIVE_SUBSTITUTES}
</inputs>

<instructions>
1. **Analyze the Customer Profile (The Circle)**:
   - **Customer Jobs:** Identify the functional, social, and emotional jobs the customer is trying to get done in their daily life or work context.
   - **Customer Pains:** Detail the negative outcomes, obstacles, risks, and frustrations the customer experiences or fears before, during, and after trying to get the jobs done.
   - **Customer Gains:** Detail the positive outcomes, concrete benefits, utility, and positive emotions that the customer expects, desires, or would be pleasantly surprised by.
2. **Design the Value Map (The Square)**:
   - **Products & Services:** List the specific features, product modules, or service offerings that make up the value proposition.
   - **Pain Relievers:** Explain exactly how these products and services alleviate, reduce, or eliminate the specific customer pains identified.
   - **Gain Creators:** Explain exactly how these products and services generate, amplify, or deliver the specific customer gains identified.
3. **Assess the Fit**: Determine how well the Value Map aligns with the Customer Profile. Are the most intense pains addressed? Are the most essential gains generated? Identify any gaps where customer pains are ignored.
4. **Draft Value Proposition Messaging Statements**: Translate the "Fit" into a clear, compelling primary value statement, a sub-headline, and 3 key benefit pillars.
5. **Develop a Validation Plan**: Suggest 2-3 interview questions to validate these hypothesized pains and gains with real customers.
</instructions>

<output_format>
Your Value Proposition Canvas Design Report should be structured as follows:

# Value Proposition Canvas Report for {PRODUCT_DESCRIPTION}
*Target Segment: {TARGET_CUSTOMER_SEGMENT}*

## 1. Executive Fit Assessment
*Provide a high-level summary of the psychological and behavioral match between the target customer and the product. Do we have a strong "Problem-Solution Fit"?*

---

## 2. The Value Proposition Canvas Matrix
*Present a clear Markdown comparative representation of the two sides of the canvas.*

### Side A: The Customer Profile (Circle)
| Customer Jobs (To-Be-Done) | Customer Pains (Frictions/Fears) | Customer Gains (Hopes/Desires) |
| :--- | :--- | :--- |
| *What are they trying to achieve?*<br>- **J1 (Functional):** [Detail]<br>- **J2 (Social):** [Detail]<br>- **J3 (Emotional):** [Detail] | *What frustrates or stops them?*<br>- **P1 (Obstacle):** [Detail]<br>- **P2 (Risk):** [Detail]<br>- **P3 (Frustration):** [Detail] | *What positive outcomes do they want?*<br>- **G1 (Required):** [Detail]<br>- **G2 (Expected):** [Detail]<br>- **G3 (Unexpected):** [Detail] |

### Side B: The Value Map (Square)
| Products & Services (Features) | Pain Relievers (Friction Killers) | Gain Creators (Value Generators) |
| :--- | :--- | :--- |
| *What are we selling/building?*<br>- **PS1:** [Feature/Offering]<br>- **PS2:** [Feature/Offering] | *How do we eliminate customer pains?*<br>- **PR1 (Fixes P1):** [How it helps]<br>- **PR2 (Fixes P3):** [How it helps] | *How do we create customer gains?*<br>- **GC1 (Creates G1):** [How it helps]<br>- **GC2 (Creates G3):** [How it helps] |

---

## 3. Deep-Dive Mapping & Fit Integrity

### A. Customer Jobs Breakdown
*Detailed analysis of the behavioral context ({CUSTOMER_BEHAVIOR}). Explain why the social and emotional jobs might be more powerful drivers of purchasing than the obvious functional jobs.*

### B. Pain Relievers vs. Pains Analysis
*Walk through the key alignments. Critically assess if the product is wasting resources relieving minor pains while ignoring the "critical, deal-breaker" pains.*

### C. Gain Creators vs. Gains Analysis
*Walk through the key alignments. Explain how the product delivers unexpected gains that differentiate it from {COMPETITIVE_SUBSTITUTES}.*

---

## 4. Positioning & Copywriting Frameworks
*Translate the canvas into high-impact marketing assets:*

- **The Primary Value Proposition Headline (The Hook):** *A single, punchy, high-impact headline targeting the core Job and primary Pain Reliever.*
- **Sub-headline (The Promise):** *A supporting sentence detailing the specific product/solution category and key gain.*
- **Three Core Benefit Pillars:**
  1. **[Pillar 1 Title]:** Focuses on [PR1/G1] (Supports Job 1).
  2. **[Pillar 2 Title]:** Focuses on [PR2/G2] (Supports Job 2).
  3. **[Pillar 3 Title]:** Focuses on [PR3/G3] (Supports Job 3).

## 5. Discovery & Validation Interview Guide
*2-3 open-ended, non-leading customer interview questions designed to test the validity of the hypothesized jobs, pains, and gains without introducing bias.*
</output_format>

<style>
Maintain a highly analytical, empathetic, and conversion-focused tone. Do not list features as value propositions; translate features into emotional and functional outcomes for the customer. Ensure the copy frameworks are high-converting, punchy, and devoid of corporate jargon.
</style>
