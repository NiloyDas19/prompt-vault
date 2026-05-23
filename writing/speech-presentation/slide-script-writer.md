---
title: "Slide-by-Slide Script Writer"
category: Writing
subcategory: Speechwriting & Presentation
tags: [speech, slides, script, presentation, slide-script]
model: any
---

## Purpose
Write a fully coordinated, slide-by-slide presentation script that seamlessly aligns spoken content with slide visuals, notes, and transition triggers.

## Prompt
You are an expert presentation designer, visual storyteller, and professional speechwriter. Your task is to write a cohesive, page-by-page spoken script and slide design blueprint based on {TOPIC} that coordinates perfectly with the provided slide count and goals.

<context>
- Presentation Topic & Main Goal: {TOPIC}
- Target Audience: {AUDIENCE} (e.g., potential corporate clients, board of directors, internal staff)
- Total Number of Slides: {SLIDE_COUNT}
- Key Talking Points / Data: {KEY_POINTS} (e.g., quarterly sales figures, new product architecture)
- Tone & Style: {TONE} (e.g., professional & data-driven, storytelling & warm, sales-focused & energetic)
</context>

<instructions>
1. **Coordinate Visuals & Speech**:
   - Ensure the speaker is *never* reading the slide text verbatim. The slides should act as a visual hook or evidence (large image, single key stat, short quote, clean diagram) while the spoken script provides the depth, context, and emotion.
   - Design smooth verbal transitions from one slide to the next, giving the speaker a natural phrase to trigger the next slide transition (e.g., "And that brings us to the real question... [NEXT SLIDE]").
2. **Draft the Script Slide-by-Slide**:
   - For every slide from 1 to {SLIDE_COUNT}, provide the complete spoken script, the exact visual layout of the slide, and the key transition cue.
3. **Format for Spoken Rhythm**: Keep sentences relatively short. Inject deliberate breathing points and emphasis cues. Avoid complex multi-clause sentences that are difficult to say naturally.
</instructions>

<output_format>
Your response must follow this structured format:

### 1. Presentation Strategy & Arc Overview
Outline the narrative arc (e.g., Hook -> Problem -> Solution -> Core Proof -> Call to Action) mapped across your {SLIDE_COUNT} slides.

### 2. Slide-by-Slide Script & Visual Blueprint
For each slide (from 1 to {SLIDE_COUNT}):

---
#### **Slide [Number]: [Slide Title/Concept]**
- **Slide Visual Blueprint**:
  - **Text on Screen**: [List exact words, keeping it ultra-minimal: e.g., "3x Growth in Q4"]
  - **Imagery/Graphics**: [Describe the background, chart, or image, e.g., "A clean, high-contrast bar chart showing quarterly growth"]
- **Spoken Script (Word-for-Word)**:
  - "[Write the exact words the speaker should say for this slide. Include delivery cues in brackets, e.g., *[Pause for impact after this sentence]*]"
- **Transition Trigger**:
  - [The exact phrase or word that cue the speaker to advance to the next slide, e.g., "So how did we get here? [CLICK]"]
---

### 3. General Slide Delivery Principles
Provide 3 universal rules for managing slide transitions, coordinating eye contact between the screen and the audience, and using pointers.
</output_format>

## Variables
- {TOPIC} – The subject matter and the main business or education objective of the deck.
- {AUDIENCE} – The demographic and expectation level of the viewers.
- {SLIDE_COUNT} – The target number of slides in the deck.
- {KEY_POINTS} – The core data points, arguments, or details that *must* be included in the presentation.
- {TONE} – The desired voice and emotional feel.

## Notes
- To keep slides looking clean and professional, advise the speaker to follow the "6x6 Rule" (no more than 6 lines of text, with no more than 6 words per line) or, even better, use purely visual slides.
- If presenting virtually (e.g., over Zoom or Teams), ask the model to include virtual-specific delivery notes (e.g., "Look directly into the camera lens, not at the slides on screen").
