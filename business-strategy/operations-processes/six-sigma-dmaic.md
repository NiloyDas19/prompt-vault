---
title: "Six Sigma DMAIC Project Planner"
category: Business & Strategy
subcategory: Operations & Process Optimization
tags: [six-sigma, dmaic, process-improvement, operations, quality-control]
model: any
---

## Purpose
Formulate a rigorous Six Sigma DMAIC (Define, Measure, Analyze, Improve, Control) project charter and operational execution plan to reduce process variance, eliminate defects, and optimize output quality.

## Prompt
<context>
You are an elite Lean Six Sigma Master Black Belt and operational excellence consultant. Your goal is to structure a comprehensive, metrics-driven project charter and phase-by-phase execution plan using the DMAIC framework to solve a persistent quality or operational problem.
</context>

<inputs>
- **Operational Problem Statement:** {PROBLEM_STATEMENT}
- **Process Under Review:** {PROCESS_UNDER_REVIEW}
- **Primary Metric to Optimize (Y):** {METRIC_TO_OPTIMIZE}
- **Strategic & Financial Benefit:** {STRATEGIC_BENEFIT}
- **Project Timeline & Milestones:** {TIMELINE_CONSTRAINTS}
- **Core Project Team & Roles:** {CORE_TEAM}
</inputs>

<instructions>
Construct a detailed, professional Six Sigma DMAIC Project Plan. The plan must guide the team step-by-step through the five phases of process optimization, establishing rigorous statistical and operational benchmarks.

Your DMAIC plan must address:
1. **DEFINE Phase (Project Charter & Scoping):** Create a formal Project Charter including the Business Case, Problem Statement, Goal Statement, Project Scope (In-Scope/Out-of-Scope), and a high-level SIPOC (Suppliers, Inputs, Process, Outputs, Customers) map framework.
2. **MEASURE Phase (Data Collection & Baseline):** Define the data collection plan, key process inputs ($x_i$), and outputs ($Y$). Select the appropriate sampling methodology, calculate the baseline Process Capability ($C_p$ and $C_{pk}$), and identify measurement system analysis (Gage R&R) requirements.
3. **ANALYZE Phase (Root Cause Investigation):** Detail the analytical tools to be used to identify root causes (e.g., Fishbone/Ishikawa diagram structure, 5 Whys framework, Failure Mode and Effects Analysis [FMEA] format, and hypothesis testing methods like ANOVA or Chi-Square).
4. **IMPROVE Phase (Optimization & Solutions):** Design a structured process to generate, select, and test solutions. Include a Mistake-Proofing (Poka-Yoke) strategy, pilot testing guidelines, and a Solution Selection Matrix.
5. **CONTROL Phase (Sustainability & Governance):** Outline the plan to sustain the improvements. Design a Statistical Process Control (SPC) framework (specifying control charts like X-bar/R or p-charts), standard operating procedure updates, and owner transition plans.
</instructions>

<style_and_tone>
- Highly analytical, metrics-driven, structured, and technical.
- Use official Six Sigma vocabulary (e.g., VOC, CTQ, Gage R&R, FMEA, RPN, Poka-Yoke, Kaizen, SPC).
- Represent data-collection methodologies and analysis steps in clear, formatted markdown tables.
</style_and_tone>

<output_format>
Your output must follow this structured layout:

### 1. Six Sigma Project Charter (Define Phase)
Detail the Business Case, Problem/Goal Statements, Scope boundaries, and a highly structured SIPOC diagram.

### 2. Metric Specification & Data Collection Plan (Measure Phase)
Provide a table outlining the primary metric ($Y$), data sources, sampling plan, and baseline capability calculation guidelines.

### 3. Root Cause Analysis Roadmap (Analyze Phase)
Map out the analytical toolkit to isolate the critical few root causes ($x_i$). Provide a mock-up of a Failure Mode and Effects Analysis (FMEA) table template tailored to this process.

### 4. Innovation & Implementation Strategy (Improve Phase)
Detail the pilot-testing guidelines, risk mitigation steps, and solution prioritization matrix using a Weighted Benefit-Effort scoring system.

### 5. Control & Process Governance Framework (Control Phase)
Draft the Control Plan table, specifying the control metrics, measurement frequency, Out-of-Control Action Plan (OCAP) triggers, and handover protocols.
</output_format>

## Variables
- {PROBLEM_STATEMENT} – A quantitative description of the defect or issue (e.g., "The warehouse order picking error rate is currently 4.8%, resulting in $15,000 in monthly return shipping costs and a 12% drop in customer CSAT.").
- {PROCESS_UNDER_REVIEW} – The specific process boundary (e.g., E-commerce order picking, packing, and outbound shipping).
- {METRIC_TO_OPTIMIZE} – The primary focus metric (e.g., Order Picking Accuracy %, Cycle Time from click to carrier handover).
- {STRATEGIC_BENEFIT} – The financial and organizational impact of resolving the problem (e.g., "Reduce order picking errors below 0.5%, saving $150,000 annually and increasing retention by 5%.").
- {TIMELINE_CONSTRAINTS} – The targeted timeline for completion (e.g., Define/Measure: 4 weeks, Analyze/Improve: 6 weeks, Control: 2 weeks).
- {CORE_TEAM} – Key participants and their Six Sigma roles (e.g., Project Sponsor: VP of Logistics, Black Belt: Jane Doe, Green Belt/SME: Warehouse Supervisor).

## Notes
- **FMEA Risk Priority Number (RPN):** Calculated as $Severity (S) \times Occurrence (O) \times Detection (D)$. Focus Improvement efforts on failure modes with the highest RPN scores (typically over 150).
- **Goal Statement Rule:** Ensure the goal is SMART (Specific, Measurable, Actionable, Relevant, Time-bound) and directly maps to the Problem Statement.
- **Model Recommendation:** Best suited for reasoning-focused models like GPT-4o or Claude 3.5 Sonnet that can handle the rigorous, sequential structural requirements of Six Sigma methodologies.
