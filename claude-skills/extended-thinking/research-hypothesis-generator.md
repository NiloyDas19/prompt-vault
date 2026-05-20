---
title: "Research Hypothesis Generator"
category: Claude Skills
subcategory: Extended Thinking
tags: [research, hypothesis, scientific-method, analysis, brainstorming]
model: claude (Extended Thinking recommended)
---

## Purpose
Generate, evaluate, and rank multiple testable hypotheses for a research question, with reasoning about feasibility and impact.

## Prompt

I need to develop strong, testable research hypotheses. Think broadly first, then narrow down to the most promising candidates.

<research_area>
{RESEARCH_AREA}
</research_area>

<research_question>
{RESEARCH_QUESTION}
</research_question>

<known_facts_and_prior_work>
{BACKGROUND_KNOWLEDGE}
</known_facts_and_prior_work>

<constraints>
{CONSTRAINTS}
</constraints>

Please:
1. **Explore the hypothesis space** — Generate 8–10 possible hypotheses, ranging from conservative to bold
2. **Screen for testability** — For each, assess: Is it falsifiable? Can it be tested with {AVAILABLE_RESOURCES}?
3. **Evaluate novelty** — Does this go beyond what is already known or obvious?
4. **Rank the top 3** — Select the most promising hypotheses and explain why
5. **For each top hypothesis, provide:**
   - Null hypothesis (H₀) and alternative hypothesis (H₁)
   - Suggested study design or experiment type
   - Key variables (independent, dependent, controlled)
   - Potential confounds to control for
6. **Blind spot check** — What important hypothesis might you have missed?

## Variables
- {RESEARCH_AREA} – The field or domain (e.g., behavioral economics, materials science, UX design)
- {RESEARCH_QUESTION} – The overarching question you want to answer
- {BACKGROUND_KNOWLEDGE} – What is already known; prior studies, established facts
- {CONSTRAINTS} – Budget, time, resources, ethical limitations
- {AVAILABLE_RESOURCES} – What you can realistically use to test (surveys, lab equipment, datasets, etc.)

## Notes
- 🧠 Requires Extended Thinking — Extended Thinking produces more creative and better-reasoned hypothesis generation.
- For academic research, follow up with the "Research Paper Summarizer" to check what existing literature says.
- Works across all research domains: scientific, social science, UX, market research.
