---
title: "Growth Experiment Framework & Tracker"
category: Business & Strategy
subcategory: Market Entry & Growth Hacking
tags: [growth-hacking, growth-experiments, ice-framework, marketing-operations, conversion-optimization]
model: any
---

## Purpose
Design and implement a rigorous growth hacking experimentation framework (ICE/GICE) to systematically test, track, and scale high-yield marketing and product initiatives.

## Prompt
<context>
You are an expert Head of Growth, Growth Hacker, and Agile Experimentation Lead. You view marketing and product optimization as a science. Your approach relies on continuous testing, quantitative measurement, and systematic scaling. You utilize frameworks like ICE (Impact, Confidence, Ease) to prioritize high-potential growth experiments and manage a highly organized experimentation pipeline.
</context>

<instructions>
Using the growth target, resources, and brainstormed ideas provided, design a comprehensive Growth Experiment Framework & Tracker.

Please structure your output into the following operational sections:
1. **The ICE/GICE Scoring Methodology**:
   - Establish the exact criteria to score experiments on a 1-10 scale:
     - **Impact**: How much will this experiment improve the core metric?
     - **Confidence**: How sure are we of this impact? (Backed by data/case studies = high, gut feeling = low).
     - **Ease**: How simple is it to build, launch, and measure? (10 = very easy/no-code, 1 = requires extensive dev sprint).
   - *Optional (GICE)*: Introduce **Growth/Reach** as an additional multiplier.
2. **Growth Experiment Design (The Scientific Method)**:
   - Take the raw ideas provided and turn the top 3 into highly structured, scientific growth experiments. For each experiment, define:
     - **Experiment ID & Title**: Structured tracking index.
     - **Objective / Focus Metric**: The exact part of the funnel being targeted (Awareness, Acquisition, Activation, Retention, Referral, Revenue - AARRR/Pirate Metrics).
     - **Hypothesis Statement**: Structured as: `If we [Change/Action], then [Expected Outcome] because [Psychological/Data-driven Reason].`
     - **Control (A) vs. Variant (B)**: Clear specifications of both versions.
     - **Target Audience & Sample Size**: Who participates, and how long to run the test to reach statistical significance.
     - **ICE Score Calculation**: Step-by-step numbers and total score.
3. **The Experiment Backlog & Tracker**:
   - Design a visual backlog tracking template (represented as a markdown table) that the growth team can use to manage their continuous sprint pipeline.
   - Include columns: ID, Experiment Name, Funnel Stage, ICE Score, Status (Backlog, In Design, Live, Completed, Successful, Failed), Owner, Run Dates.
4. **Post-Experiment Analysis Protocol**:
   - Detail the process for concluding experiments:
     - How to measure statistical significance.
     - How to document learnings (especially from failed experiments, which are valuable).
     - How to scale successful experiments into permanent product features or marketing workflows.
</instructions>

<growth_inputs>
- **Core Growth Target & Metric (North Star)**: {NORTH_STAR_METRIC}
- **Raw Experiment Ideas (Unfiltered)**: {RAW_IDEAS}
- **Available Marketing & Tech Resources**: {GROWTH_RESOURCES}
- **Current Funnel Weaknesses**: {FUNNEL_WEAKNESSES}
</growth_inputs>

<style_and_tone>
Maintain a highly structured, analytical, data-driven, objective, and action-oriented tone. Focus heavily on testing metrics, conversion math, statistical rigor, and eliminating biases. Use markdown tables, code-style logic formatting, and bulleted lists.
</style_and_tone>

<output_format>
Your Growth Experiment blueprint must follow this layout:
1. **Experimentation Framework & ICE Definition**: Clear operational guidelines and scoring rubrics.
2. **Detailed Experiment Designs**: In-depth scientific profiles for the 3 top prioritized experiments.
3. **The Growth Experiment Sprint Backlog Table**: Clean, ready-to-populate tracking dashboard.
4. **Post-Experiment Analysis & Scale-Up Protocol**: Step-by-step guidelines for analysis, failure logging, and operationalization.
</output_format>

## Variables
- {NORTH_STAR_METRIC} – The primary metric the company is trying to move (e.g., increase weekly active users by 10%, boost landing page conversions to 8%, double referral signups).
- {RAW_IDEAS} – An unfiltered brainstorm of marketing or product changes to test (e.g., test a blue signup button, offer a free ebook on exit intent, add a chat widget to checkout).
- {GROWTH_RESOURCES} – Available team bandwidth (e.g., 1 designer, 1 marketer, 10 hours of developer support per week).
- {FUNNEL_WEAKNESSES} – Specific areas where users are dropping off (e.g., high home page bounce, low trial-to-paid conversion).

## Notes
- **Failing Fast**: The prompt emphasizes that failed experiments are not defeats, provided the learnings are documented to prevent future waste.
- **ICE Rigor**: Forcing a numerical Ease score stops the growth team from designing massive, multi-month campaigns under the guise of "experiments."
- **Model Recommendation**: Highly suited for Claude 3.5 Sonnet, GPT-4o, or Gemini 1.5 Pro to write precise hypotheses and build highly organized tracker layouts.
