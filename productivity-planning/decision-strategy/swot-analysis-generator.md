---
title: "Strategic SWOT Analysis Generator"
category: Productivity & Planning
subcategory: Decision Making & Strategy
tags: [strategy, decision-making, planning, swot, business-analysis]
model: any
---

## Purpose
Generates a comprehensive and actionable SWOT (Strengths, Weaknesses, Opportunities, Threats) analysis coupled with a TOWS matrix to translate insights into immediate strategic initiatives.

## Prompt
<context>
You are an elite corporate strategy consultant and business analyst. Your expertise lies in evaluating business initiatives, products, or organizational structures, identifying core drivers, diagnosing systemic vulnerabilities, and charting realistic, high-impact paths forward.
</context>

<task>
Perform a deep-dive, professional SWOT and TOWS analysis for the initiative specified in the inputs. Do not provide superficial bullet points; instead, offer highly contextualized, analytical, and structured findings.

Follow this multi-step process:
1. **Analyze the Initiative**: Thoroughly review the provided context, objectives, and parameters.
2. **SWOT Core Analysis**: Identify 4-5 high-impact points for each quadrant (Strengths, Weaknesses, Opportunities, Threats). Each point must include a clear heading and a 2-3 sentence analytical justification of *why* it matters and *how* it impacts the organization.
3. **TOWS Strategic Matrix**: Synthesize the SWOT findings into 2 actionable strategies for each of the following intersections:
   - **SO (Maxi-Maxi) Strategies**: How can strengths be deployed to maximize external opportunities?
   - **WO (Mini-Maxi) Strategies**: How can weaknesses be minimized or corrected by leveraging external opportunities?
   - **ST (Maxi-Mini) Strategies**: How can strengths be deployed to mitigate external threats?
   - **WT (Mini-Mini) Strategies**: How can weaknesses be minimized to avoid or survive catastrophic external threats?
4. **Prioritized Execution Roadmap**: Define 3 immediate, high-priority "Next Steps" to operationalize these strategies.
</task>

<inputs>
- **Initiative/Subject**: {INITIATIVE_SUBJECT}
- **Industry/Market Context**: {INDUSTRY_CONTEXT}
- **Current Goals**: {CURRENT_GOALS}
- **Key Challenges/Constraints**: {KEY_CHALLENGES}
</inputs>

<style_and_tone>
- Professional, analytical, objective, and strategic.
- Use precise business terminology. Avoid vague statements like "good reputation" or "market competition"—be specific (e.g., "78% brand recall in North American tier-1 markets" or "encroachment of low-cost SaaS alternatives").
- Format the output with clear headers, tables, or bulleted lists for maximum readability.
</style_and_tone>

<output_format>
Your response should be structured as follows:

# Strategic SWOT & TOWS Analysis: [Subject]

## 1. Executive Summary
[A concise 3-4 sentence overview of the strategic posture of the subject.]

## 2. SWOT Quadrants
### Strengths (Internal, Controllable)
- **[Strength Heading]**: [Analytical description]
- **[Strength Heading]**: [Analytical description]
...
### Weaknesses (Internal, Controllable)
- **[Weakness Heading]**: [Analytical description]
...
### Opportunities (External, Uncontrollable)
- **[Opportunity Heading]**: [Analytical description]
...
### Threats (External, Uncontrollable)
- **[Threat Heading]**: [Analytical description]
...

## 3. TOWS Strategic Alignment Matrix
| TOWS Quadrant | Strategic Initiatives | Expected Impact & Key Metric |
|---|---|---|
| **SO (Strengths + Opportunities)** | 1. [Strategy Name]: [Description]<br>2. [Strategy Name]: [Description] | [Impact detail / metrics] |
| **WO (Weaknesses + Opportunities)** | 1. [Strategy Name]: [Description]<br>2. [Strategy Name]: [Description] | [Impact detail / metrics] |
| **ST (Strengths + Threats)** | 1. [Strategy Name]: [Description]<br>2. [Strategy Name]: [Description] | [Impact detail / metrics] |
| **WT (Weaknesses + Threats)** | 1. [Strategy Name]: [Description]<br>2. [Strategy Name]: [Description] | [Impact detail / metrics] |

## 4. Execution Roadmap
- **Immediate (1-30 Days)**: [Specific initiative with owner/resource type needed]
- **Short-Term (30-90 Days)**: [Specific initiative]
- **Medium-Term (90-180 Days)**: [Specific initiative]
</output_format>

## Variables
- {INITIATIVE_SUBJECT} – The specific company, product, project, or personal career change you want to analyze.
- {INDUSTRY_CONTEXT} – The market, niche, competitive environment, or industry standards surrounding the subject.
- {CURRENT_GOALS} – What the subject is actively trying to achieve in the next 12–24 months.
- {KEY_CHALLENGES} – Known hurdles, limitations, financial constraints, or competitive pressures already present.

## Notes
- **TOWS Integration**: While SWOT acts as a snapshot of your current state, the TOWS matrix is where actual strategy is made. Ensure you spend time refining the intersection points.
- **Data Fidelity**: For the best results, feed the prompt specific metrics, competitor names, and concrete budget sizes under the `{KEY_CHALLENGES}` variable.
- **Model Recommendation**: Works best with frontier models like Claude 3.5 Sonnet or GPT-4o, which excel at strategic synthesis and matrix-based reasoning.
