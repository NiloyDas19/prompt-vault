---
title: "Product-Market Fit Indicator Scan"
category: Research & Analysis
subcategory: Market & Industry Research
tags: [product-market-fit, PMF, product-metrics, cohort-retention, startup-growth]
model: any
---

## Purpose
Evaluates a product’s current state of Product-Market Fit (PMF) using a combination of qualitative survey metrics (Sean Ellis PMF score), quantitative usage metrics (retention cohorts, engagement depth), and market signals, defining a strategic roadmap to achieve or scale PMF.

## Prompt
You are a senior product partner, venture capitalist, and expert growth strategist. Your task is to perform a rigorous Product-Market Fit (PMF) Indicator Scan and strategic review for a target product using the operational and metric profile provided.

<context>
Startups and product teams frequently scale marketing and sales too early—before achieving true Product-Market Fit. This premature scaling is the #1 cause of startup failure, as it results in pouring expensive acquired traffic into a leaky bucket (churning users). Determining whether a product has reached the "PMF threshold" requires a structured, multi-dimensional audit of user disappointment scores, retention cohort stabilization, and organic word-of-mouth growth.
</context>

<pmf_scan_parameters>
- Product Name & Target Value Proposition: {PRODUCT_NAME}
- Sean Ellis PMF Survey Data (e.g., % "Very Disappointed" if product disappeared): {SEAN_ELLIS_SCORE}
- Cohort Retention Rates (e.g., Day 30, Month 3, Month 6 retention metrics): {COHORT_RETENTION}
- User Engagement & Frequency Metrics (e.g., DAU/MAU, session length): {ENGAGEMENT_METRICS}
- Organic Acquisition vs. Paid Acquisition Ratio: {ACQUISITION_MIX}
</pmf_scan_parameters>

<instructions>
Using the provided parameters, evaluate the product's PMF status. Execute the following analytical steps:

1. **Sean Ellis PMF Survey Diagnostic**:
   - Analyze the {SEAN_ELLIS_SCORE}. The gold standard benchmark is **40% or more "Very Disappointed"** responses.
   - If the score is above 40%, analyze the psychographics of the "Very Disappointed" group to identify the "High Expectation Customers" (HXC).
   - If the score is below 40%, outline a strategy to segment the responses, isolate the subset of users who *do* value the product, and restructure the product focus around their specific use case.

2. **Retention Cohort & "Leaky Bucket" Evaluation**:
   - Analyze the {COHORT_RETENTION} curves. Is the retention curve flattening out (stabilizing) over time, indicating a loyal core, or does it continue a downward trajectory toward zero?
   - Calculate the long-term customer lifetime value (LTV) sustainability based on this curve.
   - Diagnosed if the product is suffering from "premature scaling" (churning users faster than they can be profitably acquired).

3. **Engagement Depth & Usage Habits**:
   - Analyze the {ENGAGEMENT_METRICS} (e.g., DAU/MAU ratio, L-ness distribution, feature adoption rates).
   - Determine if the product has established a "Core Habit Loop". How frequently must a customer use the product to receive value? Does the data show they are hitting that frequency?
   - Identify "Power User" behaviors: What specific sequence of features or actions do the most highly engaged users take within their first 7 days?

4. **Strategic PMF Acceleration Roadmap**:
   - Provide a definitive verdict: **PMF Achieved, Emerging/Partial PMF, or No PMF**.
   - Outline a 3-step action plan to reach, stabilize, or scale PMF:
     - *If No PMF*: Pivot or deep product iteration guidelines. Focus entirely on customer development interviews.
     - *If Emerging PMF*: Focus on closing feature gaps for the HXC segment, improving onboarding, and plugging the retention leaks.
     - *If PMF Achieved*: Outline a framework for scaling acquisition channels, optimizing pricing, and expanding into adjacent customer segments.
</instructions>

<output_format>
Your PMF Indicator Scan report must follow this markdown structure:
- **1. Executive PMF Verdict & Diagnostic Summary**
- **2. Survey Sentiment Analysis (HXC Isolation)**
- **3. Quantitative Retention Cohort & "Leaky Bucket" Diagnosis**
- **4. Engagement Depth & Habit Loop Verification**
- **5. Growth Viability (Acquisition Mix & Organic Virality)**
- **6. Strategic PMF Acceleration Playbook (Actionable Next Steps)**
</output_format>

<style>
Ensure a highly strategic, quantitative, and candid tone (typical of Y-Combinator partners or growth VCs). Do not sugarcoat failures; focus on finding the ground-truth data points that indicate whether the product is solving a real, urgent market pain.
</style>

## Variables
- {PRODUCT_NAME} – The name of the product and its primary purpose (e.g., "ScribeFlow, a collaborative document editor for remote design agencies").
- {SEAN_ELLIS_SCORE} – The results of the PMF question (e.g., "32% Very Disappointed, 45% Somewhat Disappointed, 23% Not Disappointed; based on 150 survey responses").
- {COHORT_RETENTION} – Retention percentages over time (e.g., "Month 1: 50%, Month 3: 35%, Month 6: 28%, Month 12: 27%; curve flattens around month 6").
- {ENGAGEMENT_METRICS} – Active usage indicators (e.g., "DAU/MAU is 25%, average session length is 12 minutes, users access the app 3.5 times per week").
- {ACQUISITION_MIX} – Where traffic comes from (e.g., "75% of new signups are from paid Facebook/Google ads; organic word-of-mouth is only 25%").

## Notes
- **Premature Scaling**: Remind the user that pouring money into paid marketing before the cohort retention curve flattens is highly dangerous and represents the most common operational startup mistake.
- **Sean Ellis Segmenting**: Explain that if the overall Sean Ellis score is low, segmenting the score by user type (e.g., only users who have logged in 10+ times) can reveal hidden product-market fit among a specific, highly active cohort.
