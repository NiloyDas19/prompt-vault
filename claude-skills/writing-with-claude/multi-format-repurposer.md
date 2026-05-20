---
title: "Multi-Format Content Repurposer"
category: Claude Skills
subcategory: Writing with Claude
tags: [writing, repurposing, content-strategy, multi-format, efficiency]
model: claude
---

## Purpose
Take one piece of content and repurpose it into multiple formats simultaneously — maximizing the reach of a single idea across different channels.

## Prompt
You are a content strategist and skilled writer. Take the source content I provide and repurpose it into all the formats I specify, maintaining the core message while optimizing for each format's unique requirements.

<source_content>
{SOURCE_CONTENT}
</source_content>

<source_metadata>
- Original format: {ORIGINAL_FORMAT} (e.g., blog post, podcast transcript, research report, meeting notes)
- Core message: {CORE_MESSAGE}
- Target audience: {AUDIENCE}
- Brand voice: {BRAND_VOICE} (e.g., professional and authoritative, casual and witty, inspirational and warm)
</source_metadata>

<required_formats>
{TARGET_FORMATS}
</required_formats>

For each format, produce content that:
1. Is fully optimized for that specific channel/format
2. Stands alone — doesn't require reading the original
3. Matches the word count / length conventions of that format
4. Maintains {BRAND_VOICE} throughout
5. Preserves the most important insights from the original

Label each piece of repurposed content clearly with the format name.

## Variables
- {SOURCE_CONTENT} – The original piece of content to repurpose
- {ORIGINAL_FORMAT} – What the original content is
- {CORE_MESSAGE} – The key idea you want preserved in all repurposed versions
- {AUDIENCE} – Who all the repurposed content is for
- {BRAND_VOICE} – The voice and tone to maintain
- {TARGET_FORMATS} – List the formats needed, e.g.:
  "- LinkedIn post (150–300 words)
   - Twitter/X thread (5–7 tweets, 280 chars each)
   - Email newsletter section (200 words)
   - TikTok/Reel script (60 seconds, spoken word)
   - Slide deck outline (5 slides with bullet points)"

## Notes
- Specify character/word counts for each format — this prevents Claude from guessing.
- For social media, add "Include relevant hashtag suggestions for each platform."
- For video scripts, add "Write in a conversational, spoken-word style with natural pauses indicated."
- Best results when source content is at least 500 words with clear structure.
