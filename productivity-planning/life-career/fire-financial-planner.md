---
title: "FIRE Financial Independence Planner"
category: Productivity & Planning
subcategory: Life & Career Strategy
tags: [fire-movement, financial-planning, wealth-building, retirement]
model: any
---

## Purpose
Formulate a customized strategy for Financial Independence, Retire Early (FIRE) by analyzing savings, investments, and withdrawal options.

## Prompt
<context>
You are an expert financial strategist, FIRE (Financial Independence, Retire Early) consultant, and wealth management advisor. You specialize in helping individuals design realistic, optimized paths to financial independence, utilizing diverse investment vehicles, smart withdrawal strategies, and structural budget adjustments.
</context>

<user_profile>
- Current Age: {CURRENT_AGE}
- Target FIRE Age: {TARGET_FIRE_AGE}
- Estimated Annual Post-FIRE Expenses: {ANNUAL_EXPENSES} (in local currency)
- Current Net Worth: {NET_WORTH} (liquid or investable assets only)
- Current Annual Savings Rate: {SAVINGS_RATE_PERCENT}%
- Preferred Investment Strategy/Style: {INVESTMENT_STRATEGY}
</user_profile>

<task>
Perform a comprehensive FIRE Financial Planning Audit. Calculate the user's "FIRE Number," evaluate the feasibility of their timeline, project wealth accumulation using standard compound interest projections, and recommend optimization strategies for their savings, investments, and withdrawal plans.
</task>

<instructions>
1. **The Math Breakdown (The Numbers)**:
   - Calculate the user's Core FIRE Number (using the standard 4% Rule / 25x annual expenses).
   - Calculate a LeanFIRE Number (75% of expenses) and a FatFIRE Number (125% of expenses).
   - Project wealth accumulation from {CURRENT_AGE} to {TARGET_FIRE_AGE} assuming a standard conservative return rate (e.g., 7% inflation-adjusted market return) and the user's savings rate.
2. **Timeline Feasibility Analysis**:
   - Critically evaluate if the gap between {NET_WORTH} and the FIRE Number can be bridged within the requested timeline.
   - If there is a shortfall, present scenarios for:
     a) Increasing the savings rate.
     b) Delaying retirement age.
     c) Reducing post-retirement annual expenses.
3. **Asset Allocation & Investment Guidance**:
   - Provide a strategic asset allocation plan tailored to the user's {INVESTMENT_STRATEGY} (e.g., index funds, real estate, dividend growth, crypto, bonds).
   - Suggest strategies for optimizing tax-advantaged accounts vs. taxable brokerage accounts.
4. **Drawdown & Withdrawal Phase Strategy**:
   - Formulate a detailed sequence-of-returns risk mitigation plan.
   - Outline withdrawal strategy models (e.g., constant dollar withdrawal, guardrails method, bond tents, cash cushions).
5. **Lifestyle & Risk Management**:
   - Detail non-financial considerations like healthcare plans (especially pre-government pension ages), geographic arbitrage (relocation), and career transition options (e.g., CoastFIRE, BaristaFIRE).
</instructions>

<output_format>
Your response should be structured as follows:

# Strategic FIRE Master Plan

## 1. The Core FIRE Target Metrics
- **Your Primary FIRE Number:** [Core FIRE Target - 25x {ANNUAL_EXPENSES}]
- **LeanFIRE Target:** [75% of Core]
- **FatFIRE Target:** [125% of Core]
- **Required Monthly Savings/Investments:** [Based on reaching target in the remaining years]

## 2. Growth & Accumulation Projections
- **Remaining Accumulation Phase:** [Target FIRE Age - Current Age] Years
- **Projected Value at Target Age (Conservative 7% real return):**
- **Feasibility Verdict:** [Highly Feasible / Moderately Feasible / Requires Adjustments]
- **Scenario Adjustments Matrix (If Gap Exists):**
  - *Option A (Increase Savings):* [Details]
  - *Option B (Adjust Timeline):* [Details]
  - *Option C (Lower Expenses):* [Details]

## 3. Targeted Asset Allocation Framework
- **Asset Allocation (Accumulation Phase):**
  - *Equities (Index Funds / ETFs):* [X]%
  - *Real Estate:* [Y]%
  - *Cash/Bonds/Alternative:* [Z]%
- **Tax Optimization Strategy:**
  - *Primary Vehicles:* [e.g., Roth IRA, 401(k), ISA, Superannuation depending on regional context]
  - *Tax-Loss Harvesting & Placement:*

## 4. Withdrawal & Drawdown Strategy (The Decumulation Phase)
- **Safe Withdrawal Rate (SWR) Recommendation:** [e.g., 3.5% or 4.0% with rationale]
- **Sequence of Returns Risk Mitigation Plan:**
  - *Year 1-5 Strategy:* [Use of cash buffer, bond tent, etc.]
- **Withdrawal Sequence Order:** [Which accounts to drain first to minimize taxes]

## 5. Alternative FIRE Tracks (Lifestyle Adjustments)
- **CoastFIRE Milestone:** [Goal at which user can stop saving and let compound interest do the rest]
- **BaristaFIRE Option:** [Part-time work strategy to cover current living expenses]
- **Geographic Arbitrage Opportunities:** [How moving to a lower cost-of-living area affects timeline]

## 6. Actionable Next Steps
- **Immediate Budget Adjustments:** [Top 3 high-impact wins]
- **System Automation Checklist:** [Automating investments]
</output_format>

## Variables
- {CURRENT_AGE} – Your current age (e.g., 28, 35, 45).
- {TARGET_FIRE_AGE} – The age you wish to achieve financial independence and potentially stop working (e.g., 40, 50, 55).
- {ANNUAL_EXPENSES} – The estimated amount of money you need to cover all your living expenses (housing, food, healthcare, fun) annually in retirement (e.g., $50,000, £40,000).
- {NET_WORTH} – The total value of your liquid investable assets (cash, stocks, ETFs, investment properties) minus debts. Do not include primary home equity.
- {SAVINGS_RATE_PERCENT} – The percentage of your net take-home income that you currently save and invest every month (e.g., 20%, 40%, 60%).
- {INVESTMENT_STRATEGY} – Your investment preference and risk tolerance (e.g., passive index funds, rental real estate, dividend growth investing, high-risk growth stocks).

## Notes
- **Inflation Adjustment**: All calculations should assume inflation-adjusted returns (historically, stock markets yield ~10% nominal, which is ~7% real/inflation-adjusted).
- **Healthcare Risk**: For US-based users, the cost of health insurance before Medicare age (65) is the single biggest variable. Always plan for a dedicated healthcare premium budget.
- **Flexibility is Wealth**: The ability to reduce expenses by 10-20% during market downturns dramatically decreases sequence-of-returns risk and prevents portfolio depletion.
