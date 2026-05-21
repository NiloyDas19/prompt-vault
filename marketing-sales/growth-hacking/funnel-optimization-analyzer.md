---
title: "Funnel Optimization Analyzer"
category: Marketing & Sales
subcategory: Growth Hacking
tags: [growth, funnel, conversion, optimization, analytics]
model: any
---

## Purpose
Analyze your conversion funnel to identify the biggest bottlenecks and provide specific, prioritized recommendations to increase conversions at each stage.

## Prompt
Analyze my conversion funnel and tell me exactly where I'm losing customers and what to do about it.

**Business:** {BUSINESS}
**Funnel Type:** {FUNNEL_TYPE}
**Funnel Data:**
{FUNNEL_DATA}

### Analysis:

**1. Funnel Health Scorecard**
For each stage:
| Stage | Visitors/Users | Conversion Rate | Benchmark | Status |
|-------|---------------|-----------------|-----------|--------|
- Flag stages that are significantly below benchmark as 🔴
- Note stages performing well as 🟢

**2. Bottleneck Identification**
- Which stage has the biggest absolute drop-off?
- Which stage has the worst conversion rate relative to industry benchmarks?
- Where is the highest-leverage improvement opportunity (biggest potential revenue impact)?

**3. Root Cause Analysis**
For the top 2 bottleneck stages:
- 5 possible reasons why people are dropping off at this stage
- What data would you need to confirm each hypothesis?
- Quick diagnostic tests to identify the real cause

**4. Optimization Recommendations**
For each funnel stage, provide 3 specific, actionable improvements:
- **Quick wins** (implement in 1–2 days): UI tweaks, copy changes, trust signals
- **Medium effort** (1–2 weeks): A/B tests, flow redesigns, new features
- **Strategic** (1–2 months): major changes to the product or positioning

**5. A/B Test Prioritization**
Rank the top 5 tests by expected revenue impact:
| Test | Stage | Hypothesis | Expected Lift | Effort | Priority |
|------|-------|-----------|---------------|--------|----------|

**6. Revenue Impact Calculator**
"If you improve Stage {X} conversion by just {Y}%, here's the revenue impact: {calculation}"

## Variables
- {BUSINESS} – Your business
- {FUNNEL_TYPE} – Type (e.g., "SaaS free trial to paid", "e-commerce browse to purchase", "lead gen form to qualified lead")
- {FUNNEL_DATA} – Your actual funnel numbers. Example: "Website visits: 50,000/mo → Product page: 8,000 → Add to cart: 2,000 → Checkout started: 800 → Purchase: 400"

## Notes
- A 1% improvement at the bottom of the funnel is worth more than a 10% improvement at the top. Always optimize from the bottom up.
- Industry benchmark conversion rates: SaaS trial-to-paid: 10–25%, e-commerce: 2–4%, B2B lead gen: 5–15%. Know your benchmarks.
- Don't optimize based on gut feeling. Let data tell you where to focus.
