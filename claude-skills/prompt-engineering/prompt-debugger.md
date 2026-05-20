---
title: "Prompt Debugger & Optimizer"
category: Claude Skills
subcategory: Prompt Engineering for Claude
tags: [prompt-engineering, debugging, optimization, iteration, Claude-specific]
model: claude
---

## Purpose
Diagnose why a Claude prompt is underperforming and produce an improved version with a clear explanation of what changed.

## Prompt

You are a world-class Claude prompt engineer. Diagnose the issues with the following prompt and produce an improved version.

<failing_prompt>
{FAILING_PROMPT}
</failing_prompt>

<expected_output>
{WHAT_GOOD_LOOKS_LIKE}
</expected_output>

<actual_output_examples>
{WHAT_CLAUDE_IS_ACTUALLY_PRODUCING}
</actual_output_examples>

<model_and_settings>
- Model: {CLAUDE_MODEL} (e.g., Claude 3.5 Sonnet, Claude 3 Haiku)
- Temperature: {TEMPERATURE}
- System prompt in use: {SYSTEM_PROMPT_IF_ANY}
</model_and_settings>

Analysis steps:
1. **Gap analysis** — Describe the gap between expected and actual outputs in specific, measurable terms
2. **Root cause diagnosis** — Identify the top 3 prompt issues causing this gap (e.g., ambiguous instruction, missing context, conflicting directives, no output format, wrong persona)
3. **Improved prompt** — Rewrite the prompt to fix these issues, using XML tags and {VARIABLE} placeholders
4. **Change log** — A table: Issue | Change Made | Expected Impact
5. **Validation prompts** — 3 test inputs to verify the improved prompt works as intended
6. **Further tuning** — If the improved prompt still fails, suggest: system prompt changes, few-shot examples, or model/temperature adjustments

## Variables
- `{FAILING_PROMPT}` – The prompt that isn't working
- `{WHAT_GOOD_LOOKS_LIKE}` – Describe a perfect output or paste an example
- `{WHAT_CLAUDE_IS_ACTUALLY_PRODUCING}` – Paste 1–3 examples of the bad outputs
- `{CLAUDE_MODEL}` – Which Claude model you're using
- `{TEMPERATURE}` – Temperature setting (0–1), or "default"
- `{SYSTEM_PROMPT_IF_ANY}` – System prompt if one is in use, or "None"

## Notes
- Always test improved prompts with the same inputs that caused failures to verify improvement.
- If Claude ignores a specific instruction repeatedly, try rephrasing it as a positive instruction and placing it at the END of the prompt.
- Temperature 0 reduces variability; use it when consistency matters more than creativity.
