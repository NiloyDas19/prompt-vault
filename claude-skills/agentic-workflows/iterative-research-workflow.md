---
title: "Iterative Research Workflow"
category: Claude Skills
subcategory: Agentic Workflows
tags: [agentic, research, multi-step, workflow, knowledge-synthesis]
model: claude
---

## Purpose
Run a structured, multi-step research workflow where Claude progressively deepens its analysis through successive rounds of questioning, synthesis, and validation.

## Prompt
You are a systematic research analyst. Conduct a thorough, multi-stage investigation into the following topic. Do not rush — complete each stage fully before moving to the next.

<research_topic>
{RESEARCH_TOPIC}
</research_topic>

<research_questions>
{SPECIFIC_QUESTIONS_TO_ANSWER}
</research_questions>

<known_information>
{WHAT_I_ALREADY_KNOW}
</known_information>

<output_requirements>
- Audience: {AUDIENCE}
- Format: {OUTPUT_FORMAT}
- Depth: {DEPTH_LEVEL} (e.g., executive overview, practitioner-level, academic depth)
</output_requirements>

Execute these research stages in order:

**Stage 1 — Scoping**
Define the boundaries of this research. What will and won't be covered? List the 5 most important sub-questions needed to fully answer the research topic.

**Stage 2 — Foundation**
Establish the core facts, definitions, and established knowledge about this topic. What is well-proven vs. contested?

**Stage 3 — Deep analysis**
For each of the 5 sub-questions from Stage 1, provide a thorough analysis drawing on your training knowledge.

**Stage 4 — Synthesis**
Connect the findings from Stage 3. What themes emerge? What is the most important insight when looking at the full picture?

**Stage 5 — Gaps and uncertainty**
What don't we know? Where is evidence thin? What would a skeptic challenge?

**Stage 6 — Final deliverable**
Produce the final output in {OUTPUT_FORMAT} format, addressing {SPECIFIC_QUESTIONS_TO_ANSWER} for {AUDIENCE}.

## Variables
- {RESEARCH_TOPIC} – The topic to investigate
- {SPECIFIC_QUESTIONS_TO_ANSWER} – The specific questions your research must address
- {WHAT_I_ALREADY_KNOW} – Context you have, so Claude doesn't repeat it
- {AUDIENCE} – Who will read the final output (shapes depth and vocabulary)
- {OUTPUT_FORMAT} – How the final deliverable should be structured (report, memo, FAQ, slide deck outline, etc.)
- {DEPTH_LEVEL} – How deep to go

## Notes
- This is a single-prompt multi-stage workflow — Claude works through all stages in one response.
- For topics requiring up-to-date information, use Claude in conjunction with a web search tool or Perplexity.
- Pair with "Cross-Document Synthesizer" when you have source documents to include.
