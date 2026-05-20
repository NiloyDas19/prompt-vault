---
title: "Few-Shot Example Designer"
category: Claude Skills
subcategory: Prompt Engineering for Claude
tags: [prompt-engineering, few-shot, examples, Claude-specific, quality-control]
model: claude
---

## Purpose
Design high-quality, diverse few-shot examples for a Claude prompt to lock in the exact tone, format, and quality level you need.

## Prompt

You are an expert in few-shot prompting. Help me design ideal few-shot examples to include in a Claude prompt.

<task_description>
{TASK_DESCRIPTION}
</task_description>

<example_of_ideal_output>
{IDEAL_OUTPUT_EXAMPLE}
</example_of_ideal_output>

<known_failure_modes>
{WHAT_GOES_WRONG_WITHOUT_EXAMPLES}
</known_failure_modes>

<number_of_examples_needed>
{NUM_EXAMPLES}
</number_of_examples_needed>

Please:
1. **Analyze the ideal output** — What specific qualities make it good? (tone, length, structure, vocabulary, depth)
2. **Design {NUM_EXAMPLES} diverse examples** — Each as a full input→output pair, wrapped in `<example>` tags
3. **Ensure diversity** — Cover different input types, edge cases, and tone variations
4. **Add negative examples** (if helpful) — 1–2 `<bad_example>` pairs showing what NOT to do
5. **Integration advice** — Where to place the examples in the prompt and how to label them
6. **Quality check** — Review the examples as a set: do they collectively teach the right behavior without introducing unwanted patterns?

## Variables
- `{TASK_DESCRIPTION}` – What Claude needs to do (e.g., "classify customer support tickets by urgency", "write product descriptions in a casual voice")
- `{IDEAL_OUTPUT_EXAMPLE}` – One example of a perfect output for this task
- `{WHAT_GOES_WRONG_WITHOUT_EXAMPLES}` – Current failure modes (e.g., "too formal", "too long", "ignores edge cases")
- `{NUM_EXAMPLES}` – How many examples you need (3–5 is usually optimal)

## Notes
- 3–5 high-quality examples outperform 10+ mediocre ones. Quality matters more than quantity.
- Always include at least one edge-case example — Claude uses examples to infer how to handle unusual inputs.
- Wrap example blocks in `<examples>...</examples>` and individual pairs in `<example>...</example>` for best parsing.
