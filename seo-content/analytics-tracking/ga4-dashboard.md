---
title: "GA4 Strategic Metric Dashboard Planner"
category: SEO & Content
subcategory: Analytics & Performance Tracking
tags: [ga4, google-analytics-4, seo-dashboards, looker-studio, performance-metrics]
model: any
---

## Purpose
Design a comprehensive blueprint and custom implementation plan for a Google Analytics 4 (GA4) and Looker Studio dashboard tailored specifically to show the business value, user engagement, and conversion impact of organic search traffic.

## Prompt
<context>
You are a senior Web Analytics Architect and seasoned SEO Director. Your core expertise lies in translating vague business objectives into highly practical GA4 exploration templates, custom event tagging schemas, and executive-ready Looker Studio visualization dashboards.
</context>

<task>
Based on the provided business goals, target audience personas, and website architecture, design a comprehensive blueprint for an organic search performance dashboard in GA4 and Looker Studio.
</task>

<instructions>
1. **Define Core Business Outcomes**: Align your dashboard metrics with the specified conversion activities ({CONVERSION_ACTIVITIES}). Focus on tracking organic search contributions to both micro-conversions (e.g., newsletter sign-ups, PDF downloads) and macro-conversions (e.g., purchase events, sales-qualified leads).
2. **Select Crucial Metrics & Dimensions**: Outline the exact GA4 metrics (e.g., Session manual source/medium, Active users, Engagement rate, Key events, Average engagement time per active user) and dimensions (e.g., Landing page + query string, First user source/medium, Country, Device category) that must be visible on each page of the dashboard.
3. **Draft Visual Layout Pages**: Design a multi-page dashboard blueprint divided by stakeholder needs:
   - **Page 1: Executive Overview**: High-level ROI, organic traffic trends, revenue/lead attribution, and conversion path summaries.
   - **Page 2: Content Performance**: Performance categorized by content clusters, subdirectories (e.g., /blog/ vs /product/), landing page engagement, and scroll depths.
   - **Page 3: Technical & Engagement Auditing**: Page load speeds, exit rates, conversion leakage points, and user journey paths.
4. **Draft Custom Event Tracking Specifications**: Provide clear instructions on what custom events, parameters, or custom definitions ({CUSTOM_EVENTS_PARAMS}) need to be configured in GTM or GA4 to feed this dashboard.
</instructions>

<variables>
- **Conversion Activities**: {CONVERSION_ACTIVITIES} (e.g., E-commerce purchases, high-intent lead forms, resource downloads, newsletter signups)
- **Website Architecture & Focus**: {SITE_ARCHITECTURE} (e.g., B2B SaaS with blog/resources and trial sign-ups, or a multi-category E-commerce platform)
- **Custom Event Requirements**: {CUSTOM_EVENTS_PARAMS} (e.g., tracking specific button clicks, internal searches, file downloads, or video watch times)
- **Dashboard Audience**: {DASHBOARD_AUDIENCE} (e.g., CMO & Executives, Editorial content team, or Technical SEO specialists)
</variables>

<output_format>
Please format the dashboard blueprint as follows:

# GA4 & Looker Studio SEO Dashboard Blueprint

## 1. Measurement Framework & Goal Mapping
- **Business Goal**: [Brief explanation of how SEO supports business goals]
- **Primary KPIs**: [List of 3-5 high-level metrics]
- **Supporting Metrics**: [Metrics that provide diagnostic context]

## 2. Multi-Page Dashboard Visual Layout
### Page 1: [Page Name, e.g., Executive ROI Dashboard]
- **Target Audience**: [CMO, CEO, Head of Growth]
- **Key Visualization Elements**:
  - *Chart 1*: [Type of chart, e.g., Time series line chart of Organic Sessions vs. E-commerce Purchases]
  - *Chart 2*: [Type of chart, e.g., Scorecard widgets for total Leads, Conversion Rate, and Value]
  - *Chart 3*: [Type of chart, e.g., Table showing performance by First User Source/Medium]
- **Stakeholder Insight Question Answered**: [e.g., "What is the direct pipeline value of our SEO investment this month?"]

### Page 2: [Page Name, e.g., Content Performance & Intent Hub]
- **Target Audience**: [Content Managers, Writers]
- **Key Visualization Elements**:
  - *Chart 1*: [Type of chart, e.g., Scatter plot showing Pageviews vs. Average Engagement Time to map high-value content]
  - *Chart 2*: [Type of chart, e.g., Table grouped by Landing Page Subfolder path showing bounce-equivalents and form submissions]

## 3. GA4 Configuration & Custom Event Mapping
Provide the parameters required to track custom actions:
- **Event Name**: [e.g., `lead_form_submitted`]
  * **Triggering Action**: [e.g., Submission of the contact form]
  * **Custom Parameters to Collect**: [e.g., `form_id`, `form_location`, `lead_type`]
  * **Looker Studio Treatment**: [How this should be parsed or displayed]

## 4. Implementation Checklist & Looker Studio Filters
1. [ ] **Organic Filter definition**: [Details on how to isolate pure organic traffic in Looker Studio, e.g. using Regex filters]
2. [ ] **Data Source Configuration**: [How to merge GSC and GA4 data sources together using blend tools]
3. [ ] **Report Sharing & Scheduled Email Cadence**: [Recommendations for delivery schedules]
</output_format>

## Variables
- {CONVERSION_ACTIVITIES} – The crucial actions that represent business success (such as purchase, demo request, signup, email subscription).
- {SITE_ARCHITECTURE} – The layout and structure of the website (e.g., "B2B SaaS site with /blog, /features, /pricing subdirectories").
- {CUSTOM_EVENTS_PARAMS} – Any specific events or custom dimensions you need to track (e.g., scroll percentage, click-to-call, newsletter signups).
- {DASHBOARD_AUDIENCE} – The core team or executives who will rely on this dashboard to make decisions.

## Notes
- **Data Blending Tip**: When building Looker Studio reports, blend Google Search Console data (queries and pages) with GA4 landing page data using the Landing Page URL / Landing Page dimension as the join key.
- **Data Retention Settings**: Remind the user to increase the default GA4 data retention setting from 2 months to 14 months in the GA4 admin panel to allow for year-over-year comparative reporting.
- **Model Recommendation**: Highly compatible with Claude 3.5 Sonnet and GPT-4o for precise structure, technical parameter naming conventions, and layout visualization ideas.
