---
title: "Chain-of-Thought Prompt Designer"
category: Claude Skills
subcategory: Prompt Engineering for Claude
tags: [chain-of-thought, reasoning, prompt-engineering, step-by-step, Claude-specific]
model: claude
---

## Purpose
Design a chain-of-thought (CoT) prompt that forces Claude to reason through a problem step by step before giving its final answer, dramatically improving accuracy on complex tasks.

## Prompt

You are a prompt engineering expert. Design a chain-of-thought (CoT) prompt for the following task that will guide Claude to reason step by step before answering.

<task>
{TASK_DESCRIPTION}
</task>

<complexity_level>
{COMPLEXITY} (e.g., simple calculation, multi-step logic, ambiguous interpretation, expert-level domain reasoning)
</complexity_level>

<desired_reasoning_style>
{REASONING_STYLE} (e.g., mathematical proof style, Socratic questioning, scientific method, legal reasoning, business case analysis)
</desired_reasoning_style>

Design the CoT prompt with:
1. **Setup** — A persona and task framing that primes careful reasoning
2. **Explicit reasoning steps** — Numbered or labeled steps Claude must work through (use `<thinking>` tags to contain the reasoning)
3. **Self-verification step** — An instruction to double-check the answer before outputting it
4. **Final answer format** — A clearly delimited `<answer>` block so the final output is easy to extract
5. **One complete worked example** — Show what a correct CoT response looks like for a sample input

Also explain:
- Why each step in the reasoning chain is necessary
- What errors this CoT design prevents

## Variables
- `{TASK_DESCRIPTION}` – What Claude needs to reason about
- `{COMPLEXITY}` – How complex the reasoning needs to be
- `{REASONING_STYLE}` – The style of reasoning that fits this domain

## Notes
- Chain-of-thought prompting is most impactful for tasks where accuracy matters more than speed.
- For Claude 3.7+ with Extended Thinking, CoT in the prompt is less necessary — but still useful for controlling the reasoning structure.
- 🧠 Use `<thinking>` tags to make Claude's reasoning visible and easier to audit.
