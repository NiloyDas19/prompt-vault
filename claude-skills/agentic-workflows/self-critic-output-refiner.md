---
title: "Self-Critic & Output Refiner"
category: Claude Skills
subcategory: Agentic Workflows
tags: [agentic, self-critique, iteration, quality-control, output-refinement]
model: claude
---

## Purpose
Have Claude generate an output, critically evaluate it against specific criteria, then produce an improved version — all in a single prompt, without human intervention between rounds.

## Prompt
Complete the following task, then critically evaluate your own output and produce a refined version. Do not skip the evaluation step.

<task>
{TASK_DESCRIPTION}
</task>

<quality_criteria>
{QUALITY_CRITERIA}
</quality_criteria>

<context>
{RELEVANT_CONTEXT}
</context>

**Step 1 — Initial output**
Complete the task above to the best of your ability. Label this section `[DRAFT]`.

**Step 2 — Self-critique**
Now critique your own draft honestly. For each quality criterion listed, rate your draft (1–5) and explain what is lacking. Be harsh — a lenient self-critique defeats the purpose. Label this section `[CRITIQUE]`.

**Step 3 — Refined output**
Using your critique as a guide, produce an improved version that addresses every issue identified. Label this section `[REFINED]`.

**Step 4 — Improvement summary**
List the specific changes made between Draft and Refined, and confirm each quality criterion is now met.

## Variables
- {TASK_DESCRIPTION} – The task Claude should complete (e.g., "Write a product description for {PRODUCT}", "Draft a reply to this email: {EMAIL}")
- {QUALITY_CRITERIA} – The standards to evaluate against (e.g., "Concise (under 150 words), persuasive, no jargon, ends with a clear CTA, professional but warm tone")
- {RELEVANT_CONTEXT} – Background Claude needs to complete the task well

## Notes
- This prompt is an agentic pattern — Claude acts as both creator and evaluator, reducing the need for multiple human review rounds.
- Increase critique rigor by adding "Be extremely critical. A score of 4/5 or lower means the criterion needs addressing."
- Chain multiple refinement rounds by feeding the `[REFINED]` output back into Step 1.
- Works best when quality criteria are specific and measurable rather than vague (e.g., "persuasive" is vague; "includes a statistic, addresses the reader's top objection, ends with a question" is measurable).
