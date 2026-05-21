---
title: "Ad Performance Analyzer"
category: Marketing & Sales
subcategory: Advertising
tags: [advertising, analytics, performance, optimization, ROAS]
model: any
---

## Purpose
Analyze advertising campaign performance data, diagnose issues, and provide specific optimization recommendations to improve ROAS.

## Prompt
Analyze my advertising campaign performance and tell me what's working, what's not, and exactly what to change.

**Campaign Data:**
{PASTE_CAMPAIGN_DATA}

**Business Context:**
- Product: {PRODUCT}
- Average Order Value / Deal Size: {AOV}
- Customer LTV: {LTV}
- Target CPA: {TARGET_CPA}
- Conversion Window: {CONVERSION_WINDOW}

### Analysis:

**1. Performance Overview**
- Summary of key metrics vs. benchmarks
| Metric | Current | Benchmark | Status |
|--------|---------|-----------|--------|
| CTR | | | 🟢/🟡/🔴 |
| CPC | | | |
| Conversion Rate | | | |
| CPA | | | |
| ROAS | | | |

**2. Diagnosis**
- Where is the biggest problem: traffic quality, ad creative, or landing page?
- If CTR is low → creative/targeting issue
- If CTR is high but conversion is low → landing page or offer issue
- If CPA is high → multiple possible causes

**3. Campaign-Level Recommendations**
For each campaign/ad set:
- Verdict: Scale, Optimize, Pause, or Kill
- Specific changes to make
- Priority order

**4. Creative Analysis**
- Which ads are winners and losers?
- Pattern analysis: what do winning ads have in common?
- Creative fatigue indicators
- 3 new ad concepts to test based on winner patterns

**5. Audience Analysis**
- Which audiences are most/least efficient?
- Audience overlap issues
- New audiences to test

**6. Budget Reallocation**
- How to redistribute budget from losers to winners
- Expected impact of reallocation

**7. Action Plan (This Week)**
Prioritized list of exactly what to do:
1. [Highest impact action]
2. [Second highest]
3. [Third highest]

## Variables
- {PASTE_CAMPAIGN_DATA} – Paste your ad performance data (from Google Ads, Meta Ads Manager, etc.)
- {PRODUCT} – What you're selling
- {AOV} – Average order value
- {LTV} – Customer lifetime value
- {TARGET_CPA} – Target cost per acquisition
- {CONVERSION_WINDOW} – How long after a click before a conversion typically happens

## Notes
- Always analyze at the ad set/ad group level, not just the campaign level. Campaign averages hide both winners and losers.
- Give campaigns at least 50 conversions before making budget decisions. Fewer than 50 conversions is not statistically significant.
- ROAS without LTV context is misleading. A 2x ROAS looks bad until you realize those customers have a 12-month LTV of 8x.
