---
title: "Multi-Angle Analyst"
category: Claude Skills
subcategory: Extended Thinking
tags: [analysis, perspective, critical-thinking, strategy, extended-thinking]
model: claude (Extended Thinking recommended)
---

## Purpose
Analyze a situation, topic, or decision from multiple stakeholder perspectives simultaneously, surfacing blind spots and conflicting interests.

## Prompt

Analyze the following situation from multiple distinct perspectives. Approach each perspective with genuine empathy and rigor — do not just summarize, actually inhabit each viewpoint.

<situation>
{SITUATION_DESCRIPTION}
</situation>

<perspectives_to_analyze>
{PERSPECTIVES}
</perspectives_to_analyze>

<goal_of_analysis>
{GOAL}
</goal_of_analysis>

For each perspective:
1. **Identify their core interests** — What does this party fundamentally want or need?
2. **Their view of the situation** — How do they see it, and why?
3. **What they stand to gain or lose**
4. **What they would likely do or recommend**
5. **What they are NOT saying** — Unstated concerns, fears, or agendas

After all perspectives:
6. **Common ground** — Where do all perspectives agree?
7. **Key conflicts** — Where are the sharpest disagreements, and why?
8. **Synthesis** — Given all perspectives, what is the wisest path forward?
9. **Blind spot check** — Whose perspective is missing from this analysis?

## Variables
- {SITUATION_DESCRIPTION} – The scenario, decision, or topic to analyze
- {PERSPECTIVES} – List the stakeholders or viewpoints (e.g., "CEO, front-line employees, customers, regulators" or "environmentalists, local community, mining company, government")
- {GOAL} – What you want from this analysis (e.g., "find a policy everyone can accept", "understand why this project failed", "prepare for negotiations")

## Notes
- 🧠 Requires Extended Thinking — Extended Thinking allows Claude to maintain multiple simultaneous mental models, producing richer perspective analysis.
- Use this before negotiations, policy decisions, product launches, or any situation with multiple stakeholders.
- Add "also analyze from the perspective of {ADDITIONAL_PERSPECTIVE}" in follow-up messages to extend the analysis.
