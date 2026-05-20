---
title: "XML Structured Prompt Builder"
category: Claude Skills
subcategory: Prompt Engineering for Claude
tags: [prompt-engineering, XML-tags, structure, Claude-specific, formatting]
model: claude
---

## Purpose
Convert a messy or underperforming prompt into a well-structured, XML-tagged Claude prompt that produces consistently better outputs.

## Prompt

You are an expert Claude prompt engineer. Transform the following prompt into a well-structured, high-performance Claude prompt using XML tags for clarity and precision.

<original_prompt>
{ORIGINAL_PROMPT}
</original_prompt>

<performance_issues>
{WHAT_IS_WRONG}
</performance_issues>

<desired_output_format>
{DESIRED_FORMAT}
</desired_output_format>

Please:
1. **Diagnose** — Identify 3–5 specific reasons the original prompt underperforms (e.g., ambiguous instructions, missing context, no format specification, conflates role with task)
2. **Redesign** — Rewrite the prompt using XML tags to separate:
   - `<role>` — Who Claude is
   - `<context>` — Background information
   - `<task>` — What Claude must do
   - `<constraints>` — What to avoid or limit
   - `<output_format>` — Exact format expected
   - `<examples>` — If few-shot examples would help
3. **Before/After comparison** — Show the original and redesigned prompts side by side
4. **Improvement rationale** — Explain each structural change and why it helps Claude perform better
5. **Variable placeholders** — Add {VARIABLE} placeholders for any user-specific inputs

## Variables
- `{ORIGINAL_PROMPT}` – The prompt you want to improve
- `{WHAT_IS_WRONG}` – What's not working (e.g., "outputs are too long", "ignores constraints", "too generic", "wrong tone")
- `{DESIRED_FORMAT}` – What a perfect output looks like (length, structure, tone)

## Notes
- Claude is specifically trained to parse XML tags accurately, making this the most reliable structuring method for complex prompts.
- Don't over-tag simple prompts — XML tagging is most valuable when prompts have 3+ distinct sections.
- Use this iteratively: improve → test → identify new issues → improve again.
