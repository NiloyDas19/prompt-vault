---
title: "Deep Problem Solver"
category: Claude Skills
subcategory: Extended Thinking
tags: [extended-thinking, reasoning, complex-problems, analysis]
model: claude (Extended Thinking recommended)
---

## Purpose
Harness Claude's extended thinking mode to work through genuinely complex, multi-variable problems with full visible reasoning.

## Prompt

I need you to use your full reasoning capacity to work through a complex problem. Think carefully before responding — consider multiple approaches, check your assumptions, and work through the logic step by step before giving your final answer.

<problem>
{PROBLEM_STATEMENT}
</problem>

<context>
{RELEVANT_CONTEXT}
</context>

<constraints>
{CONSTRAINTS}
</constraints>

Please structure your response as:
1. **Restate the problem** — Confirm your understanding, noting any ambiguities
2. **Decompose** — Break the problem into its core sub-problems
3. **Explore approaches** — Consider at least 2–3 different solution paths and why each might or might not work
4. **Reason through the best path** — Work through your chosen approach step by step, checking your logic as you go
5. **Final answer** — State your conclusion clearly and confidently
6. **Confidence check** — Rate your confidence (1–10) and explain what would change your answer

## Variables
- {PROBLEM_STATEMENT} – The full problem you need solved
- {RELEVANT_CONTEXT} – Background information, data, or constraints the model needs
- {CONSTRAINTS} – Specific limitations: time, resources, assumptions

## Notes
- 🧠 Requires Extended Thinking — Enable Extended Thinking in Claude for best results on this prompt; it gives Claude a dedicated reasoning budget before answering.
- For math/logic problems, ask Claude to show every calculation step.
- Use this when a single-pass answer feels too shallow or when the problem has multiple valid interpretations.
