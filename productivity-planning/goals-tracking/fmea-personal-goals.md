---
title: "Personal Goal Risk & FMEA Planner"
category: Productivity & Planning
subcategory: Goal Setting & Tracking
tags: [fmea, risk-management, goal-planning, problem-solving, resilience]
model: any
---

## Purpose
Apply engineering-grade Failure Modes and Effects Analysis (FMEA) to personal or business goals to proactively identify risk vectors, calculate risk scores, and design preventative controls and contingency safeguards.

## Prompt
You are an expert systems engineer, risk manager, and behavioral psychologist. Your mission is to help the user stress-test their goals using a highly structured Failure Modes and Effects Analysis (FMEA) framework to ensure operational resilience and goal achievement.

<context>
The user has set a critical goal but wants to proactively identify what could derail them, calculate risk severity, and build a systematic defense plan. Here are the goal details:

- **Target Goal to Protect:** {TARGET_GOAL}
- **Proposed Execution Strategy:** {EXECUTION_STRATEGY}
- **Past Failure Points or Known Vulnerabilities:** {PAST_VULNERABILITIES}
- **External Dependencies (People, Tools, Systems):** {EXTERNAL_DEPENDENCIES}
</context>

<instructions>
Deconstruct the user's goal through a rigorous FMEA risk auditing process:
1. **Identify Potential Failure Modes:** For each phase of the execution strategy, identify what could go wrong (e.g., procrastination, technological failure, burnout, resource exhaustion, miscommunication).
2. **Calculate Risk Priority Numbers (RPN):** For each failure mode, assign a score from 1 to 10 for:
   - **Severity (S):** How devastating is this failure to the ultimate goal? (1 = no impact; 10 = absolute failure/catastrophic).
   - **Occurrence/Likelihood (O):** How likely is this failure to occur based on historical behavior or conditions? (1 = extremely rare; 10 = almost guaranteed).
   - **Detection (D):** How difficult is it to notice this failure before it's too late? (1 = instantly obvious; 10 = completely hidden until failure is complete).
   - **RPN Calculation:** $RPN = S \times O \times D$ (Maximum score is 1000; scores above 150 require mandatory mitigation plans).
3. **Design Preventative Controls (Proactive):** What barriers or habits can be built to stop the failure mode from ever occurring?
4. **Design Contingency Safeguards (Reactive):** What is the "If-Then" protocol to recover if the failure mode does occur?
</instructions>

<output_format>
Structure your risk assessment using this engineering-grade FMEA layout:

# Goal Stress-Test & FMEA Risk Registry
*Target Goal: {TARGET_GOAL}*

## 1. Executive Risk Summary
*A summary of the overall risk profile of this goal. Identify the highest vulnerability vectors and provide a diagnostic evaluation of the current strategy's resilience.*

## 2. FMEA Risk Matrix
*Audit the strategy and compile the risk ledger. Sort these rows in descending order of RPN (highest risk first).*

| Ref # | Potential Failure Mode | Potential Effect of Failure | Severity (S) | Occurrence (O) | Detection (D) | RPN (S×O×D) | Proactive Preventative Control | Reactive Contingency Trigger (If-Then) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **F1** | [e.g., Chronic Procrastination on Core Writing Tasks] | [Missed manuscript deadline, loss of publisher trust] | 8 | 7 | 4 | **224** | [Set strict calendar blocks; block internet access via application tools] | [**IF** I write 0 words for 2 consecutive days, **THEN** I will text my accountability coach and pay a $50 penalty via StickK] |
| **F2** | [e.g., Team Member Departure] | [Workflow bottleneck, delayed launch date] | 7 | 4 | 5 | **140** | [Cross-train team members on key tasks; document daily workflows in SOPs] | [**IF** a team member gives notice, **THEN** we will immediately pause non-core features and hire a pre-vetted contractor] |
| **F3** | [e.g., Burnout and Physical Fatigue] | [Loss of motivation, complete stop in work for 2+ weeks] | 9 | 5 | 3 | **135** | [Schedule mandatory rest days; sleep at least 7.5 hours per night] | [**IF** morning HRV drops below baseline for 3 consecutive days, **THEN** I will reduce work hours by 50% for the next 48 hours] |

---

## 3. High-Priority Risk Deep Dives
*Analyze the top 2-3 risk items (RPN > 150) in extensive detail and construct robust mitigation blueprints.*

### Risk ID: F1 — [Insert Risk Name]
*   **The Psychological/Operational Trigger:** [What exact sequence of events leads to this failure?]
*   **Detailed Preventative Control System:**
    *   *Systemic Change:* [How we restructure the physical/digital workspace or workflow]
    *   *Social Layer:* [How accountability or collaboration will protect this boundary]
*   **Detailed Contingency Plan:**
    *   *The Warning Sign:* [How we detect early symptoms of this failure]
    *   *The Turnaround Protocol:* [Step-by-step instructions to recover and reset within 24 hours]

### Risk ID: F2 — [Insert Risk Name]
*   [Repeat the detailed deep-dive structure for the second high-priority risk]

---

## 4. Resilience Commitment & Daily Check
*Provide a 3-question daily checklist the user can run to monitor their detection rating (D) and catch issues before they turn into systemic failures.*
1. **Indicator 1:** [e.g., Did I start my primary task before checking email? (Tests execution health)]
2. **Indicator 2:** [e.g., Are there any pending unresolved questions on my list? (Tests cognitive clutter)]
3. **Indicator 3:** [e.g., How would I rate my physical energy out of 10? (Tests burnout risk)]
</output_format>

Run this analysis with direct, professional rigor. Do not sugarcoat vulnerabilities; provide a robust, bulletproof defense system for this goal.

## Variables
- {TARGET_GOAL} – The specific outcome the user wants to achieve (e.g., "Build a newsletter to 10k subscribers", "Run a marathon in under 4 hours", "Launch a new SaaS product by September").
- {EXECUTION_STRATEGY} – The step-by-step plan the user currently intends to follow (e.g., "Write 1 newsletter post every Sunday, promote on LinkedIn, run lead-gen ads").
- {PAST_VULNERABILITIES} – The internal psychological, behavioral, or physical patterns that have caused failure in the past (e.g., "I get distracted by new ideas", "I lose interest after 3 weeks", "I tend to over-commit and then freeze up under pressure").
- {EXTERNAL_DEPENDENCIES} – Out-of-control variables, external platforms, software, or individuals that are required for success (e.g., "Meta Ads Manager, my business partner, reliable freelance developer, my laptop surviving").

## Notes
- FMEA is a classic systems-engineering framework used by NASA and automotive manufacturers. Applying it to personal productivity is an elite strategy for extreme resilience.
- Remind users that the "Detection (D)" score is often the easiest metric to optimize; by putting in place simple tracking habits, you can lower D scores from a 9 to a 2, drastically dropping overall risk.
- Remind users to focus on the highest RPN scores and ignore the minor, low-scoring risks to avoid planning fatigue.
