---
title: "Prompt Chaining Orchestrator"
category: Claude Skills
subcategory: Agentic Workflows
tags: [agentic, prompt-chaining, orchestration, workflow, pipeline]
model: claude
---

## Purpose
Design a multi-step prompt chain where each Claude call's output feeds into the next, enabling complex workflows that no single prompt could accomplish.

## Prompt
You are a prompt chain architect. Design a complete, production-ready prompt chain for the following workflow.

<workflow_goal>
{WORKFLOW_GOAL}
</workflow_goal>

<input_data>
{STARTING_INPUT}
</input_data>

<desired_final_output>
{FINAL_OUTPUT_DESCRIPTION}
</desired_final_output>

<constraints>
- Maximum chain steps: {MAX_STEPS}
- Claude model for each step: {MODEL_PREFERENCE}
- Any steps that must use specific tools or external APIs: {TOOL_REQUIREMENTS}
</constraints>

Design a complete prompt chain:

1. **Chain overview** — A numbered list of all steps with one-sentence descriptions
2. **Data flow diagram** — Describe how data flows from input → Step 1 → Step 2 → ... → Final Output
3. **For each step, provide:**
   - Step name and purpose
   - Input: what this step receives
   - The complete prompt template for this step (with {VARIABLES} for dynamic inputs)
   - Output schema: exactly what this step should return (format, structure)
   - Error handling: what to do if this step fails or returns unexpected output
4. **Validation gates** — Where to add human-in-the-loop review before proceeding
5. **Implementation notes** — Pseudocode or Python snippet showing how to wire the chain together using the Claude API

## Variables
- {WORKFLOW_GOAL} – What the entire chain needs to accomplish end-to-end
- {STARTING_INPUT} – What data or content enters the chain at Step 1
- {FINAL_OUTPUT_DESCRIPTION} – What the chain should produce at the end
- {MAX_STEPS} – Maximum number of Claude calls to use (for cost/latency budgeting)
- {MODEL_PREFERENCE} – Which Claude model to use for each step (e.g., Haiku for classification steps, Sonnet for generation steps)
- {TOOL_REQUIREMENTS} – Any steps requiring external APIs, databases, or tools

## Notes
- Use cheaper/faster models (Claude Haiku) for classification, routing, and filtering steps; reserve Sonnet/Opus for generation steps.
- Always validate the output format of each step before passing it to the next — chain failures are usually formatting mismatches.
- Add a "catch-all" error step at the end to handle unexpected failures gracefully.
