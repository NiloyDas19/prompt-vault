---
title: "Deep Image Analyzer"
category: Claude Skills
subcategory: Vision & Document Analysis
tags: [vision, image-analysis, multimodal, Claude-specific, visual-reasoning]
model: claude (vision-capable models only)
---

## Purpose
Perform a thorough, structured analysis of an image — describing content, reading embedded text, interpreting context, and answering specific questions.

## Prompt

Analyze the image I've attached carefully and thoroughly. Look at everything — do not miss details in the periphery or background.

<analysis_requirements>
- Primary purpose of this analysis: {ANALYSIS_PURPOSE}
- Specific questions to answer: {SPECIFIC_QUESTIONS}
- Level of detail needed: {DETAIL_LEVEL} (e.g., high-level overview, detailed technical analysis, exhaustive cataloging)
</analysis_requirements>

Please provide:
1. **Primary subject** — What is the main subject or focus of the image?
2. **Full scene description** — Describe everything visible: foreground, background, objects, people, text, colors, lighting
3. **Embedded text** — Transcribe ALL text visible in the image exactly as written
4. **Technical observations** — Image quality, composition, any notable visual techniques
5. **Contextual interpretation** — What can you infer about the context, purpose, or story of this image?
6. **Answers to specific questions** — Address each of: {SPECIFIC_QUESTIONS}
7. **Confidence flags** — Note anything you are uncertain about in your analysis

[ATTACH IMAGE HERE]

## Variables
- `{ANALYSIS_PURPOSE}` – Why you're analyzing this image (shapes depth and focus)
- `{SPECIFIC_QUESTIONS}` – Specific things you want answered about the image
- `{DETAIL_LEVEL}` – How exhaustive the description should be

## Notes
- 👁️ Requires a vision-capable Claude model (Claude 3+ Sonnet, Opus, or Haiku).
- For UI screenshots, add "Identify all interactive elements and their likely functions."
- For charts/graphs, use the dedicated "Chart Data Extractor" prompt instead.
- Attach the image directly in the Claude interface or pass it via the API's vision input.
