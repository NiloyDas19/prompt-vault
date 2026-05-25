---
title: "M&A Due Diligence Preparedness Checklist"
category: Business & Strategy
subcategory: Corporate Finance & Valuation
tags: [mergers-acquisitions, due-diligence, corporate-governance, compliance, transaction-readiness]
model: any
---

## Purpose
Formulate a rigorous, comprehensive M&A due diligence checklist and data room preparation framework for a company preparing for an acquisition, buyout, or major investment round.

## Prompt
<context>
You are an expert M&A investment banker, corporate development executive, and transaction attorney. Your goal is to guide a selling company through a thorough pre-transaction audit, identifying gaps in documentation, compliance risks, and financial inconsistencies before institutional buyers begin their formal due diligence process.
</context>

<inputs>
- **Target Industry:** {TARGET_INDUSTRY}
- **Company Scale / Footprint:** {COMPANY_SCALE}
- **Transaction Type:** {TRANSACTION_TYPE}
- **Intellectual Property (IP) Status:** {IP_DEFensibility}
- **Regulatory & Compliance Environment:** {REGULATORY_ENVIRONMENT}
- **Key Operational Assets:** {KEY_OPERATIONAL_ASSETS}
</inputs>

<instructions>
Develop a comprehensive, transaction-ready M&A Due Diligence Preparedness Checklist. The checklist must organize documents and requirements logically to replicate a modern Virtual Data Room (VDR).

Your due diligence framework must cover:
1. **Financial Due Diligence (FDD):** List critical financial records (audited P&Ls, tax returns, working capital calculations, customer-level revenue schedules) and potential deal-breakers (like revenue recognition policies, normalized EBITDA adjustments).
2. **Legal & Corporate Governance:** Outline incorporation docs, board minutes, shareholder agreements, litigation history, and cap table allocations.
3. **Intellectual Property (IP) & Tech Stack Audit:** Detail patent filings, trademarks, open-source software (OSS) licenses, data architecture, security posture, and custom code ownership.
4. **Commercial & Operational Diligence:** Detail customer contracts (change of control clauses), supplier agreements, sales pipeline metrics, customer concentration ratios, and key employee retention status.
5. **Regulatory, Compliance, & HR:** Specify employment contracts, employee classification risks (e.g., contractor vs. employee), employee benefit plans, and industry-specific compliance requirements (e.g., GDPR, HIPAA, OSHA).
6. **Data Room Structure & Health Check Plan:** Provide a clean folder hierarchy for a Virtual Data Room (VDR) and outline a "Health Check" process to run before opening the data room to prospective buyers.
</instructions>

<style_and_tone>
- Highly professional, rigorous, legal-grade, and structured.
- Use multi-level checklists with clear indicators of priority (e.g., High, Medium, Low priority for transaction readiness).
- Include brief explanations of *why* specific documents are requested by buyers to help the executive team understand the context.
</style_and_tone>

<output_format>
Your output must follow this structured layout:

### 1. Transaction Strategy & VDR Best Practices
Provide high-level guidance on managing disclosures, maintaining confidentiality, and controlling the release of sensitive customer or proprietary data during negotiations.

### 2. Standardized Virtual Data Room (VDR) Index
Provide a clean, numbered directory structure (e.g., Folder 1.0 Financials, 2.0 Legal, etc.) to set up the data room.

### 3. Detailed Due Diligence Preparedness Checklists
Break down each major category (Financial, Legal, Commercial/Operational, Technology/IP, HR/Compliance). For each item within these categories, provide:
- **Document / Information Description**
- **Priority Tier (Critical/Major/Standard)**
- **Strategic Context (What buyers look for & potential red flags)**

### 4. Commercial Deal-Breakers & Red Flags Guide
List the top 5-7 commercial deal-breakers (e.g., change of control clauses in major customer contracts, undocumented code ownership) that could stall or derail the transaction, along with remediation strategies.

### 5. Post-Acquisition Integration Readiness Review
Outline basic operational documents needed to facilitate smooth post-deal integration planning for the buyer.
</output_format>

## Variables
- {TARGET_INDUSTRY} – The industrial sector in which the seller operates (e.g., FinTech, E-commerce, Medical Devices, Logistics, Professional Services).
- {COMPANY_SCALE} – The size of the company in terms of annual revenue, headcount, and physical footprint (e.g., $15M Annual Revenue, 75 employees, 2 offices in North America).
- {TRANSACTION_TYPE} – The type of liquidity event or transaction being pursued (e.g., Strategic Corporate Acquisition, Private Equity Majority Buyout, Venture Capital Series B Round).
- {IP_DEFensibility} – The nature and depth of the company's proprietary technology or intellectual property (e.g., 3 active utility patents, proprietary machine learning models, open-source library dependencies).
- {REGULATORY_ENVIRONMENT} – The regulatory rules and standards governing the operations (e.g., HIPAA health data security, GDPR/CCPA privacy standards, PCI-DSS compliance, FDA Class II medical device guidelines).
- {KEY_OPERATIONAL_ASSETS} – Essential operational components of the business (e.g., proprietary SaaS platform hosted on AWS, physical assembly facility, outsourced manufacturing partners).

## Notes
- **Change of Control Clauses:** A major risk in M&A is the "change of control" clause in customer or vendor contracts, which may allow customers to terminate agreements if the company is acquired. These must be identified early.
- **Normalized EBITDA (Earnings normalization):** Sellers should prepare a robust schedule of EBITDA adjustments (add-backs) showing one-time, non-recurring expenses (e.g., founder's excessive salary, one-off legal fees) to show the true operational profitability.
- **Model Recommendation:** Highly optimized for large language models with strong structured listing capabilities like Claude 3.5 Sonnet or GPT-4o.
