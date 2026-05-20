---
title: "Agentic Task Decomposer"
category: Claude Skills
subcategory: Agentic Workflows
tags: [agentic, task-decomposition, planning, multi-step, automation]
model: claude
---

## Purpose
Break down a complex, multi-step goal into a precise, ordered plan of atomic tasks that Claude (or a human) can execute one step at a time.

## Prompt
You are an expert project planner and agentic workflow designer. Decompose the following goal into a complete, executable plan.

<goal>
{GOAL_DESCRIPTION}
</goal>

<available_tools_and_resources>
{AVAILABLE_TOOLS}
</available_tools_and_resources>

<constraints>
- Deadline: {DEADLINE}
- Must avoid: {CONSTRAINTS}
- Success criteria: {SUCCESS_CRITERIA}
</constraints>

Please produce:

1. **Goal clarification** — Restate the goal in precise, measurable terms. Flag any ambiguities.
2. **Dependency map** — Identify which tasks depend on others and which can be done in parallel.
3. **Ordered task list** — Number every task in execution order:
   - Task name (verb phrase, e.g., "Fetch user data from API")
   - Input required (what information or resource this task needs)
   - Output produced (what this task creates/returns)
   - Tool or method to use
   - Estimated effort (S/M/L)
   - Potential failure mode and fallback
4. **Critical path** — Which tasks, if delayed, delay the whole goal?
5. **Checkpoints** — Where should a human review the output before proceeding?
6. **Rollback plan** — If the plan fails at step N, how do we recover?

## Variables
- {GOAL_DESCRIPTION} – The high-level goal to accomplish (be as specific as possible)
- {AVAILABLE_TOOLS} – What tools, APIs, data sources, or capabilities are available to execute tasks
- {DEADLINE} – When this needs to be done, or "No hard deadline"
- {CONSTRAINTS} – What must not happen (e.g., no external API calls, cannot modify production DB, must stay under $50 cost)
- {SUCCESS_CRITERIA} – How you'll know the goal is fully achieved

## Notes
- For Claude API usage, each atomic task in the plan can become a separate prompt in a chain.
- Use this before building an agentic workflow to validate the logic before coding it.
- Pair with "Iterative Refiner" to continuously improve outputs at each task step.
