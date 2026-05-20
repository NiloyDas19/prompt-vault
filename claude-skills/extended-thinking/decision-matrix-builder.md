---
title: "Decision Matrix Builder"
category: Claude Skills
subcategory: Extended Thinking
tags: [decision-making, matrix, trade-offs, reasoning, strategy]
model: claude
---

## Purpose
Build a structured, weighted decision matrix to evaluate competing options across multiple criteria, with Claude reasoning through the weightings and scores.

## Prompt

Help me make a high-stakes decision using a structured decision matrix. Reason through each criterion carefully before scoring.

<decision_to_make>
{DECISION_DESCRIPTION}
</decision_to_make>

<options>
{OPTIONS_LIST}
</options>

<evaluation_criteria>
{CRITERIA}
</evaluation_criteria>

<priorities_and_context>
{CONTEXT_AND_PRIORITIES}
</priorities_and_context>

Please:
1. **Validate or refine the criteria** — Are these the right things to evaluate? Suggest any missing criteria.
2. **Assign weights** — Assign a weight (1–5) to each criterion based on my stated priorities. Explain the weighting rationale.
3. **Score each option** — Score each option (1–10) on each criterion with a brief justification.
4. **Build the matrix** — Present a formatted table: Options × Criteria with weighted scores and totals.
5. **Interpret the result** — Which option wins? Does the winner feel right intuitively? If not, explore why.
6. **Sensitivity analysis** — What single criteria weight change would flip the decision?

## Variables
- {DECISION_DESCRIPTION} – What you're deciding (e.g., "Which cloud provider to migrate to")
- {OPTIONS_LIST} – The options you're choosing between (list each one)
- {CRITERIA} – What matters in this decision (e.g., cost, scalability, team expertise, vendor lock-in)
- {CONTEXT_AND_PRIORITIES} – Your situation and what matters most to you

## Notes
- For personal decisions (career, location, relationships), the criteria and weights are especially important to get right — push back if they seem off.
- Pair with the "System Architecture Critic" if this is a technical infrastructure decision.
