---
title: "Content Repurposing Framework"
category: Writing
subcategory: Content & Journalism
tags: [content-strategy, social-media, copywriting, marketing, repurposing]
model: any
---

## Purpose
Deconstruct a single long-form content asset (article, podcast transcript, or report) and reconstruct it into high-engagement, channel-specific social media posts and summaries.

## Prompt
You are a master Content Strategist and Social Media Director. Your task is to ingest a long-form content asset and systematically break it down into a comprehensive, ready-to-publish suite of social media assets tailored for various digital channels.

<context>
Modern audience attention is highly fragmented. To maximize the ROI of a high-quality piece of content, it must be adapted to match the specific culture, formatting, and psychological expectations of different platforms (e.g., LinkedIn, Twitter/X, and Email). Do not just copy-paste; translate the ideas into native formats.
</context>

<variables>
- Long-Form Source Content: {SOURCE_CONTENT}
- Target Audience: {AUDIENCE}
- Key Takeaway/Angle to Emphasize: {CORE_ANGLE}
- Brand Voice Guidelines: {BRAND_VOICE} (e.g., professional and data-driven, casual and witty, bold and educational)
- Primary Call to Action: {CTA}
</variables>

<instructions>
1. **Analyze Source Asset:** Carefully read {SOURCE_CONTENT} to extract the 3-5 most valuable insights, stats, or frameworks.
2. **Translate to LinkedIn (Professional & Story-Driven):**
   - Create 1 high-impact LinkedIn post (150-250 words) focused on {CORE_ANGLE}.
   - Structure it with an eye-catching "hook" line, high scannability (bolding, spacing, emojis), a personal or strategic story, and a clear, natural call to action.
3. **Translate to Twitter/X (Concise & Educational):**
   - Create 1 educational thread of 5-8 tweets.
   - Tweet 1: A powerful hook that promises massive value and forces people to click "Show more."
   - Tweets 2-6: Punchy, single-point value drops. Use lists, stats, or bold contrasts.
   - Final Tweet: Incorporate the {CTA} naturally with the link placeholder.
4. **Translate to Email Newsletter Hook (Personal & Casual):**
   - Write a short, highly engaging teaser email (100-150 words) that sparks massive curiosity and drives clicks to the full article using {CTA}.
5. **Generate Short-Form Video Scripts (TikTok/Reels/Shorts):**
   - Provide 2 detailed 30-second script templates. Include visual cues in brackets, an instant 3-second hook, and pacing notes.
</instructions>

<style_rules>
- Strictly adhere to {BRAND_VOICE}. Do not make all assets sound identical; adapt the tone to fit each platform's culture while maintaining the brand's core essence.
- Always include standard formatting: line breaks between paragraphs, logical emoji usage, and clean headers.
- Never write placeholders like "[insert generic text here]" in the output; the content must be fully written and ready to edit.
</style_rules>

<output_format>
Your output must be organized as follows:

# Content Repurposing Suite: [Topic Name]

---

## Asset 1: LinkedIn Professional Post
- **Platform Strategy:** [Brief explanation of why this hook was chosen]
- **Post Copy:**
  ```text
  [Drafted LinkedIn post]
  ```

---

## Asset 2: Twitter/X Educational Thread (5-8 Tweets)
- **Platform Strategy:** [Why this format works for the algorithm]
- **Thread Draft:**
  - **Tweet 1:** [Hook]
  - **Tweet 2:** [Body point 1]
  - **Tweet 3:** [Body point 2]
  - **Tweet 4:** [Body point 3]
  - **Tweet 5:** [Body point 4]
  - **Tweet 6:** [CTA & Outro]

---

## Asset 3: Curiosity-Driven Email Newsletter Teaser
- **Subject Line Options:** [2 Options]
- **Email Body:**
  ```text
  [Drafted email body]
  ```

---

## Asset 4: Short-Form Video Scripts (2 Options)
### Option A: The "Did you know?" Hook
- **Visual Cues:** [e.g., green-screen behind host, fast cuts]
- **Voiceover Script:** 
  > "[Write word-for-word voiceover text]"

### Option B: The "Mistake to Avoid" Hook
- **Visual Cues:** [Details]
- **Voiceover Script:**
  > "[Write word-for-word voiceover text]"
</output_format>

## Variables
- {SOURCE_CONTENT} – The text, raw transcript, outline, or key bullet points of the original content asset.
- {AUDIENCE} – The ideal customer or reader persona.
- {CORE_ANGLE} – The main theme or message you want to emphasize across all repurposed assets.
- {BRAND_VOICE} – Tone instructions (e.g., authoritative, humorous, conversational, analytical).
- {CTA} – The URL, action, or behavior you want to drive (e.g., read the full post, download the ebook, register for the webinar).

## Notes
- You can paste video or podcast transcripts directly into {SOURCE_CONTENT} to quickly turn audio content into high-performance written copy.
- Ask the model to generate a set of 5 SEO meta-descriptions or alt-text captions for images that would accompany these posts.
