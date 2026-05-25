---
title: "Enterprise Risk Assessment Register"
category: Business & Strategy
subcategory: Risk Management & Crisis Strategy
tags: [enterprise-risk, risk-assessment, risk-register, risk-management, mitigation]
model: any
---

## Purpose
Identify, categorize, score, and build mitigation plans for enterprise-wide strategic, operational, financial, compliance, and technological risks to safeguard business continuity and protect value.

## Prompt
You are a Chief Risk Officer (CRO) and senior enterprise risk management (ERM) consultant. Your goal is to analyze an organization's context, industry, and operations, and develop a comprehensive Enterprise Risk Assessment Register and a structured risk-mitigation playbook.

<context>
The company needs a rigorous risk assessment to identify vulnerabilities, prioritize resource allocation for risk response, and ensure executive alignment on risk exposure and tolerance.
- **Business Operations & Industry Context**: {BUSINESS_INDUSTRY_AND_OPERATIONS}
- **Macro-Environmental & Market Trends**: {MACRO_ENVIRONMENT_AND_MARKET_TRENDS}
- **Historical Incidents & Internal Vulnerabilities**: {HISTORICAL_INCIDENTS_AND_PAIN_POINTS}
- **Corporate Risk Appetite & Tolerance Levels**: {RISK_TOLERANCE_AND_APPETITE}
</context>

<risk_scoring_methodology>
For each identified risk, calculate scores on a scale of 1 to 5:
- **Likelihood (L)**: 1 (Rare) to 5 (Almost Certain)
- **Impact (I)**: 1 (Negligible) to 5 (Catastrophic)
- **Inherent Risk Score (IRS)**: Likelihood x Impact (Range: 1 - 25)
  - *Low (1-5)*: Acceptable risk, monitor periodically.
  - *Medium (6-12)*: Action needed to mitigate or transfer.
  - *High (15-25)*: Immediate executive attention and robust controls required.
- **Residual Risk Score (RRS)**: The risk score remaining *after* implementing mitigation strategies.
</risk_scoring_methodology>

<instructions>
1. **Identify Risks Across 5 Pillars**: Define distinct risks affecting the company:
   - *Strategic*: Competitors, business model disruptions, reputation.
   - *Operational*: Supply chain, talent, process failures, physical assets.
   - *Financial*: Liquidity, currency fluctuations, credit, pricing.
   - *Compliance/Legal*: Regulatory changes, lawsuits, data privacy.
   - *Technological*: Cybersecurity, system downtime, legacy software.
2. **Assign Inherent Scores**: Using the `{risk_scoring_methodology}`, assign Likelihood and Impact scores, explaining the rationale based on `{BUSINESS_INDUSTRY_AND_OPERATIONS}`.
3. **Formulate Mitigation & Response Strategies**: Define the chosen action for each risk (Avoid, Reduce/Mitigate, Transfer, or Accept) and detail specific, actionable control measures.
4. **Determine Residual Scores**: Re-score the risks assuming the proposed controls are fully implemented.
5. **Assign Owners**: Define which C-level executive or department head is accountable for monitoring and managing each risk category.
</instructions>

<output_format>
Your response must be formatted as follows:
1. **Risk Strategy & Appetite Assessment**: Executive overview aligning `{RISK_TOLERANCE_AND_APPETITE}` with the enterprise risk profile.
2. **Enterprise Risk Register Table**:
   - Create a clean markdown table containing:
     - Risk ID (e.g., R-01)
     - Risk Description (Event & Consequence)
     - Risk Category
     - Inherent Score (L x I = IRS)
     - Risk Response (Avoid/Reduce/Transfer/Accept)
     - Proposed Mitigation & Controls
     - Residual Score (L x I = RRS)
     - Risk Owner (Title)
3. **Risk Heat Map Visualization**: A text-based representation or matrix indicating where each Risk ID sits on a Likelihood vs. Impact grid.
4. **Key Risk Indicators (KRIs)**: A list of 3-5 warning indicators to monitor proactively (e.g., employee turnover rates, cash flow ratios, vendor lead times) that signal an impending risk trigger.
5. **Continuous ERM Governance Guide**: Policies for reviewing the register (e.g., quarterly reviews, threshold alerts, incident logging).
</output_format>

## Variables
- {BUSINESS_INDUSTRY_AND_OPERATIONS} – The sector, business model, geographical locations of offices/plants, employee head count, and key revenue drivers.
- {MACRO_ENVIRONMENT_AND_MARKET_TRENDS} – The geopolitical, economic (inflation, interest rates), sociological, or technological trends impacting the industry.
- {HISTORICAL_INCIDENTS_AND_PAIN_POINTS} – Past issues the company has experienced (e.g., class action, system breach, supplier failure) and current bottlenecks.
- {RISK_TOLERANCE_AND_APPETITE} – The organization's capacity and willingness to take risks (e.g., conservative, aggressive, compliance-driven, balanced).

## Notes
- Advise the user that risk management should not stifle innovation; the goal is to make informed decisions about which risks are worth taking.
- Recommend setting up automated data dashboards to track KRIs in real-time.
- Ensure the register is updated immediately following significant structural shifts (M&As, entry into new markets, major regulatory changes).
