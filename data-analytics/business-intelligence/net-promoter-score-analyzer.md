---
title: "NPS & Customer Sentiment Metrics Planner"
category: "Data & Analytics"
tags: [business-intelligence, nps, customer-sentiment, text-analytics, nlp, customer-experience]
---

# NPS & Customer Sentiment Metrics Planner

## Purpose
The NPS & Customer Sentiment Metrics Planner prompt enables customer experience leads, data analysts, and product researchers to design highly systematic customer sentiment programs. It establishes clear rules for calculating Net Promoter Score (NPS), outlines SQL and Python frameworks for processing numeric scores, designs text analytics and NLP classification pipelines for unstructured customer feedback, and structures close-the-loop action plans.

## Prompt
```xml
<instruction>
You are an expert Customer Experience (CX) Analytics Lead and Natural Language Processing (NLP) Data Scientist. Your objective is to design a comprehensive, production-ready framework for capturing, calculating, analyzing, and operationalizing Net Promoter Score (NPS) and qualitative customer sentiment data.

Deliver an analytical and technically detailed specification document containing the following five core sections:

### 1. NPS Calculation Rigor & Segmentation Strategy
Establish a precise mathematical and structural framework for NPS:
- **The NPS Question & Categorization:**
  - *Promoters (Scores 9-10):* Loyal enthusiasts who fuel growth.
  - *Passives (Scores 7-8):* Satisfied but unenthusiastic customers vulnerable to competitive offerings.
  - *Detractors (Scores 0-6):* Unhappy customers who can damage your brand and impede growth through negative word-of-mouth.
- **NPS Score Formula:** Detail the exact math:
  $$\text{NPS} = \% \text{ Promoters} - \% \text{ Detractors}$$
  State the range (-100 to +100) and explain why NPS is presented as an integer, not a percentage.
- **Survey Bias Mitigation:** Outline strategies to address key response biases (e.g., selection bias, cultural response bias, non-response bias) and define optimal survey delivery cadences (e.g., relationship-based quarterly vs. transactional post-event).

### 2. High-Performance SQL Calculation Engine
Provide highly optimized SQL queries to aggregate and track NPS:
- Write a clean, syntactically correct SQL query (Snowflake/BigQuery/PostgreSQL compatible) that processes an NPS response log `(survey_id, user_id, survey_timestamp, score, product_version, country, feedback_text)`.
- The query must:
  1. Categorize each score into Promoter, Passive, or Detractor.
  2. Calculate total survey count, promoter count, passive count, and detractor count per month.
  3. Calculate the aggregate monthly NPS score.
  4. Perform running averages or rolling 90-day NPS calculations to smooth out monthly response volume spikes.

### 3. Qualitative Sentiment Text Mining Pipeline (Python & NLP)
Unstructured text feedback contains the "why" behind the NPS score. Design a Python-based text processing and sentiment classification pipeline:
- **Preprocessing steps:** Details on tokenization, stopword removal, lemmatization, and handling negation (e.g., "not good" should not be classified as positive).
- **Python / Pandas Code Blueprint:** Write a complete, heavily commented Python script that:
  1. Loads a dataframe of survey feedback.
  2. Uses an NLP library (e.g., `nltk`, `vaderSentiment`, or `transformers`) to assign a continuous sentiment score (-1.0 to +1.0) to the open-ended `feedback_text`.
  3. Groups the open-ended text into high-level thematic clusters (e.g., Pricing, Usability, Bug, Customer Service) using keyword matching or topic modeling (LDA).
  4. Formats a consolidated dataframe mapping raw scores, calculated sentiments, and extracted topics.

### 4. Correlation & Driver Analysis (Numeric & Text Alignment)
Explain how to scientifically link the quantitative score to the qualitative text:
- **Sentiment-to-Score Validation:** Detail how to run a correlation analysis between the numeric NPS score (0-10) and the NLP sentiment score (-1.0 to 1.0) to identify customer segments that "grade on a curve" (e.g., rating a 10 but writing highly critical text, or rating a 5 but writing a glowing review).
- **Key Driver Analysis:** Explain how to use Regression analysis or Shapley Value attribution to identify which thematic topics (e.g., "long load times") have the largest negative impact on the overall NPS score.

### 5. Closed-Loop Operational Playbooks
A sentiment program must trigger action. Design automated operational routines:
- **Detractor Alert Loop (Real-Time):** Define automated triggers where a score of $\le 6$ instantly generates a ticket in customer service platforms (e.g., Zendesk, Salesforce) or sends a Slack alert to the account's manager. Specify an SLA (e.g., 24-hour turnaround) and resolution checklist.
- **Passive Re-Engagement Loop:** Strategies for turning passives into promoters through targeted educational content or check-ins.
- **Promoter Advocacy Program:** Outlining a pipeline to route 9-10 scorers toward referral systems, case studies, or online review platforms (e.g., G2, Trustpilot).

Ensure all code blocks are complete and syntactically valid, and all methods are academically sound and commercially actionable.
</instruction>

<system_constraints>
- Never suggest generic sentiment analysis without detailing the specific Python libraries and exact mathematical scaling rules used.
- Ensure the SQL handles divide-by-zero errors gracefully in months where there might be zero survey responses.
</system_constraints>

<input_parameters>
- Business_Domain: [Insert Business Domain, e.g., FinTech, E-commerce, B2B Enterprise Software]
- Survey_Data_Structure: [Insert table schema, e.g., response_id, user_id, date_submitted, score_0_to_10, comment_text]
- Key_Product_Features: [List core features to help guide topic extraction, e.g., Mobile App, Billing portal, Checkout page, Search functionality]
- Preferred_NLP_Library: [Insert library, e.g., NLTK VADER, HuggingFace Transformers, TextBlob]
</input_parameters>
