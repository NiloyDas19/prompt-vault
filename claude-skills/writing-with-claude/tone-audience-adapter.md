---
title: "Tone & Audience Adapter"
category: Claude Skills
subcategory: Writing with Claude
tags: [writing, tone, audience-adaptation, communication, clarity]
model: claude
---

## Purpose
Rewrite any piece of content for a completely different audience or tone level — from technical to plain language, formal to casual, or vice versa.

## Prompt
Rewrite the following content for a different audience and/or tone. Preserve all the substance and key information — change only how it's communicated.

<original_content>
{ORIGINAL_CONTENT}
</original_content>

<original_context>
- Written for: {ORIGINAL_AUDIENCE}
- Original tone: {ORIGINAL_TONE}
</original_context>

<adaptation_requirements>
- Rewrite for: {TARGET_AUDIENCE}
- Target tone: {TARGET_TONE}
- Reading level: {READING_LEVEL} (e.g., 8th grade, college level, expert practitioners)
- Key constraints: {CONSTRAINTS} (e.g., max 200 words, no jargon, must include a call to action, must sound warm not corporate)
</adaptation_requirements>

Please:
1. **Produce the adapted version** — fully rewritten, not just tweaked
2. **Vocabulary changes** — List 5+ specific word/phrase swaps you made and why (e.g., "leveraged → used, because the target audience prefers plain language")
3. **Structural changes** — What did you reorganize or reframe and why?
4. **What was preserved** — The core ideas and information that stayed intact
5. **Reading level check** — What approximate Flesch-Kincaid reading level is the adapted version?

## Variables
- {ORIGINAL_CONTENT} – The content to adapt
- {ORIGINAL_AUDIENCE} – Who the original was written for
- {ORIGINAL_TONE} – The original's tone (e.g., academic, casual, technical, sales-focused)
- {TARGET_AUDIENCE} – Who the new version is for (be specific: "C-suite executives with no technical background", "teenagers", "experienced nurses", etc.)
- {TARGET_TONE} – The desired tone in the new version
- {READING_LEVEL} – Approximate reading level target
- {CONSTRAINTS} – Any hard requirements on length, vocabulary, format, or content

## Notes
- The more specific your target audience definition, the better the adaptation.
- Use this for: technical docs → executive summaries, academic papers → blog posts, legal text → plain language, internal docs → customer-facing content.
- For regulated industries (healthcare, finance, legal), always have a compliance expert review plain-language adaptations.
