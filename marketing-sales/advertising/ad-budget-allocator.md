---
title: "Ad Budget Allocator"
category: Marketing & Sales
subcategory: Advertising
tags: [advertising, budget, allocation, ROI, planning]
model: any
---

## Purpose
Allocate advertising budget across channels, campaigns, and funnel stages for maximum ROI based on your business goals and constraints.

## Prompt
Help me allocate my advertising budget for maximum ROI. I want to know exactly where every dollar should go.

**Total Monthly Ad Budget:** {BUDGET}
**Business Type:** {BUSINESS_TYPE}
**Primary Goal:** {GOAL}
**Current Channels (and their performance):** {CURRENT_CHANNELS}
**Available Channels:** {AVAILABLE_CHANNELS}
**Average Customer Lifetime Value:** {LTV}
**Maximum Acceptable Cost Per Acquisition:** {MAX_CPA}
**Previous Ad Spend Results (if any):** {HISTORICAL_DATA}

### 1. Channel Allocation
| Channel | Monthly Budget | % of Total | Expected CPA | Expected ROAS | Rationale |
|---------|---------------|-----------|-------------|---------------|-----------|

### 2. Funnel Stage Allocation
| Funnel Stage | % of Budget | Channels Used | Purpose |
|-------------|------------|---------------|---------|
| Awareness (TOFU) | | | |
| Consideration (MOFU) | | | |
| Conversion (BOFU) | | | |
| Retention | | | |

### 3. New Channel Testing Budget
- Recommend setting aside {X}% for testing new channels
- Which 2 channels to test next and why
- How to structure channel tests (budget, duration, success criteria)

### 4. Scaling Rules
- When to increase budget on a channel (performance thresholds)
- When to decrease or pause (loss thresholds)
- How quickly to scale (recommended daily budget increase rate)

### 5. Seasonal Adjustments
- How to adjust budget for seasonal trends
- When to increase spend (high-conversion periods)
- When to reduce spend (low-intent periods)

### 6. Monthly Budget Review Template
- Which metrics to review for each channel
- Decision framework: scale, maintain, or cut
- Reallocation triggers

## Variables
- {BUDGET} – Total monthly advertising budget
- {BUSINESS_TYPE} – Type (e.g., "B2B SaaS", "DTC e-commerce", "local service business", "marketplace")
- {GOAL} – Primary objective
- {CURRENT_CHANNELS} – Channels you're running and their current performance
- {AVAILABLE_CHANNELS} – All channels you could use
- {LTV} – Customer lifetime value
- {MAX_CPA} – Maximum cost per acquisition you can afford
- {HISTORICAL_DATA} – Past ad spend results if available

## Notes
- The 70/20/10 rule: 70% of budget on proven channels, 20% on channels showing promise, 10% on experimental channels.
- Don't spread your budget too thin. It's better to dominate 2 channels than to be invisible on 5.
- Your target CPA should never exceed 1/3 of your LTV. If LTV is $300, your max CPA is $100.
