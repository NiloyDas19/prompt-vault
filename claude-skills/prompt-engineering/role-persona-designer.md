---
title: "Claude Persona Designer"
category: Claude Skills
subcategory: Prompt Engineering for Claude
tags: [persona, role-playing, system-prompt, prompt-engineering, Claude-specific]
model: claude
---

## Purpose
Design a richly detailed, consistent persona for Claude to inhabit across a conversation or application, with behavioral guidelines that hold up under stress.

## Prompt

You are a character designer specializing in AI persona creation. Design a complete, consistent Claude persona for the following use case.

<use_case>
{USE_CASE_DESCRIPTION}
</use_case>

<persona_requirements>
- Name / title: {PERSONA_NAME}
- Domain expertise: {EXPERTISE_AREAS}
- Communication style: {COMMUNICATION_STYLE}
- Values and principles: {CORE_VALUES}
- What this persona never does: {HARD_LIMITS}
</persona_requirements>

Design the following:
1. **Persona identity statement** (3–5 sentences) — Who this persona is, their background, and their worldview
2. **Communication style guide** — Vocabulary level, sentence length, use of jargon, warmth level, humor guidelines
3. **Behavioral rules** — 5–8 specific behavioral guidelines (what the persona always does, sometimes does, never does)
4. **Edge case handling** — How the persona responds when: asked something outside its expertise, challenged or criticized, asked to break character, given ambiguous requests
5. **Sample dialogue** — 3 example exchanges showing the persona in action across different scenarios
6. **System prompt block** — A ready-to-paste system prompt section that installs this persona

## Variables
- `{USE_CASE_DESCRIPTION}` – Where and how this persona will be used (e.g., "customer support bot for a fintech app", "Socratic tutor for philosophy students", "creative writing collaborator")
- `{PERSONA_NAME}` – Name or title for the persona
- `{EXPERTISE_AREAS}` – What this persona is an expert in
- `{COMMUNICATION_STYLE}` – How they speak (e.g., warm and empathetic, precise and clinical, witty and informal)
- `{CORE_VALUES}` – What principles guide this persona's behavior
- `{HARD_LIMITS}` – What this persona will never do or say

## Notes
- The most effective Claude personas are defined by what they DO rather than only what they don't do.
- Stress-test personas with challenging inputs before deployment.
- For multi-turn applications, add memory and continuity instructions ("Remember details the user shares across the conversation").
