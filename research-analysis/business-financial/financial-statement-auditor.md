---
title: "Financial Statement & Ratio Auditor"
category: Research & Analysis
subcategory: Business & Financial Analysis
tags: [financial-analysis, auditing, ratio-analysis, financial-health]
model: any
---

## Purpose
Analyze a company's primary financial statements to calculate core financial ratios, detect anomalies or warning signs, and assess overall fiscal health against industry benchmarks.

## Prompt
```xml
<context>
You are an elite forensic accountant and senior financial analyst with decades of experience auditing corporate financial statements. Your task is to perform a rigorous, comprehensive financial audit and ratio analysis of the provided financial statements. Your goal is to assess liquidity, solvency, operating efficiency, and profitability, while identifying potential red flags, accounting anomalies, or areas of concern.
</context>

<financial_data>
<income_statement>
{INCOME_STATEMENT}
</income_statement>

<balance_sheet>
{BALANCE_SHEET}
</balance_sheet>

<cash_flow_statement>
{CASH_FLOW_STATEMENT}
</cash_flow_statement>

<industry_benchmarks>
{INDUSTRY_BENCHMARKS}
</industry_benchmarks>

<audit_focus>
{AUDIT_FOCUS}
</audit_focus>
</financial_data>

<instructions>
Conduct your analysis by systematically working through the following steps:

1. **Data Integrity & Reconciliation Check**:
   - Verify that the balance sheet balances (Assets = Liabilities + Equity).
   - Ensure the net income from the income statement reconciles with the starting point of the cash flow statement (operating activities) and matches the change in retained earnings (accounting for dividends).
   - Flag any immediate mathematical or structural discrepancies in the provided data.

2. **Core Ratio Calculation & Interpretation**:
   Calculate the following ratios for all available periods. Show your formulas, inputs, and final values clearly:
   - **Liquidity**: Current Ratio, Quick (Acid-Test) Ratio, Cash Ratio.
   - **Solvency/Leverage**: Debt-to-Equity, Debt-to-Assets, Interest Coverage Ratio (TIE).
   - **Efficiency/Activity**: Asset Turnover, Inventory Turnover, Days Sales Outstanding (DSO), Days Payable Outstanding (DPO), Cash Conversion Cycle (CCC).
   - **Profitability**: Gross Profit Margin, EBITDA Margin, Operating Margin, Net Profit Margin, Return on Assets (ROA), Return on Equity (ROE).

3. **Benchmarking & Trend Analysis**:
   - Compare the calculated ratios against the provided <industry_benchmarks>.
   - Perform horizontal (year-over-year or quarter-over-quarter) and vertical common-size analysis.
   - Identify whether the company's performance is improving, deteriorating, or stable relative to its history and its peer group.

4. **Forensic Audit & Red Flag Detection**:
   - Inspect the relationship between net income and operating cash flow. Note if net income is rising while operating cash flow is flat or falling (potential aggressive revenue recognition or cash flow manipulation).
   - Look for unusual fluctuations in accounts receivable, inventory, or accounts payable relative to revenue/cost changes.
   - Identify any capital structure weaknesses or impending debt maturity pressures.
   - Focus specifically on the areas outlined in <audit_focus>.

5. **Strategic Recommendations**:
   - Provide concrete, actionable strategies for corporate management or investors to address the identified weaknesses, improve working capital management, optimize leverage, or boost profitability.
</instructions>

<output_format>
Present your findings in a structured, professional report using the following markdown format:

# FINANCIAL AUDIT & RATIO ANALYSIS REPORT

## 1. Executive Summary
- **Overall Financial Health Score**: [Scale of 1-10 with a brief justification]
- **Key Findings**: [3-4 high-level bullet points summarizing the company's situation]
- **Critical Red Flags**: [List any urgent accounting anomalies or financial threats]

## 2. Data Integrity & Reconciliation
- [Status of mathematical accuracy and reconciliation between statements]
- [Details of any identified anomalies or omissions]

## 3. Financial Ratio Analysis & Benchmarking
*(Include a markdown table comparing the metrics across periods and against the industry benchmarks)*

| Metric / Ratio | Period 1 | Period 2 | Industry Benchmark | Trend & Assessment |
| :--- | :--- | :--- | :--- | :--- |
| **Liquidity** | | | | |
| Current Ratio | | | | |
| Quick Ratio | | | | |
| **Solvency** | | | | |
| Debt-to-Equity | | | | |
| Interest Coverage | | | | |
| **Efficiency** | | | | |
| Cash Conversion Cycle | | | | |
| **Profitability** | | | | |
| Operating Margin | | | | |
| ROE | | | | |

*Provide a bulleted analysis explaining the drivers behind each major ratio category (Liquidity, Solvency, Efficiency, Profitability).*

## 4. Trend & Common-Size Analysis
- **Horizontal & Vertical Highlights**: [Key insights from common-size financial statements]
- **Growth Vectors vs. Margin Erosion**: [Analysis of revenue growth vs. cost structures]

## 5. Forensic Audit & Red Flag Register
- **Issue 1**: [Description, potential accounting/operational cause, and risk level (High/Medium/Low)]
- **Issue 2**: [Description, potential accounting/operational cause, and risk level]

## 6. Strategic & Operational Recommendations
- [Recommendation 1 - Focus on working capital, liquidity, or debt optimization]
- [Recommendation 2 - Focus on profitability or cost controls]
- [Recommendation 3 - Focus on capital allocation and cash flow sustainability]
</output_format>
```

## Variables
- `{INCOME_STATEMENT}` – Paste the detailed Income Statement, including Revenue, Cost of Goods Sold (COGS), Operating Expenses, Depreciation & Amortization, Interest, Taxes, and Net Income for all periods to analyze.
- `{BALANCE_SHEET}` – Paste the Balance Sheet with Assets (Current and Non-Current), Liabilities (Current and Long-Term), and Shareholders' Equity.
- `{CASH_FLOW_STATEMENT}` – Paste the Statement of Cash Flows covering Operating, Investing, and Financing activities.
- `{INDUSTRY_BENCHMARKS}` – Provide industry averages, competitor metrics, or specific baseline expectations for ratios like current ratio, debt-to-equity, and profit margins.
- `{AUDIT_FOCUS}` – Specify if there are any specific concerns, e.g., "aggressive revenue recognition," "high debt load," "working capital drain," or "inventory build-up."

## Notes
- **Data Quality**: Ensure raw numbers or financial statements are clean, structured, and labeled with their units (e.g., thousands or millions) for absolute accuracy.
- **Model Recommendation**: Best used with highly analytical, instruction-following models like Claude 3 Opus or Claude 3.5 Sonnet to ensure rigorous mathematical and structural accuracy.
- **Advanced Customization**: You can request the model to output standard common-size statements (expressing assets as 100% and revenue as 100%) in Section 4 by adding a explicit line to the data input.
