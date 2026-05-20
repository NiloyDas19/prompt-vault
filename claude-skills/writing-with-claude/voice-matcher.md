---
title: "Writing Voice Matcher"
category: Claude Skills
subcategory: Writing with Claude
tags: [writing, voice, style-matching, content, ghostwriting]
model: claude
---

## Purpose
Analyze a sample of your writing and produce new content in your exact voice, style, and tone — indistinguishable from your own work.

## Prompt
Analyze the writing samples I provide and learn my voice deeply. Then write new content in my exact style.

<writing_samples>
{WRITING_SAMPLES}
</writing_samples>

<voice_analysis_request>
Before writing anything new, analyze my voice across these dimensions:
1. **Sentence structure** — Average length, use of fragments, compound sentences, em-dashes, parentheticals
2. **Vocabulary level** — Sophistication, domain-specific jargon, word preferences
3. **Tone** — Formal vs. casual, warm vs. clinical, confident vs. hedging
4. **Rhythm** — Short punchy statements? Long flowing prose? Varied?
5. **Quirks** — Signature phrases, punctuation habits, paragraph length, use of lists vs. prose
6. **Point of view** — First person? Inclusive "we"? Direct second person?
7. **Opening style** — How do I typically start pieces or paragraphs?
</voice_analysis_request>

<new_content_request>
Now write the following in my exact voice:

Topic: {TOPIC}
Length: {LENGTH}
Purpose: {PURPOSE} (e.g., LinkedIn post, blog article, email newsletter, internal memo)
Key message: {KEY_MESSAGE}
</new_content_request>

After writing, briefly note 2\u20133 specific voice elements you deliberately incorporated.

## Variables
- {WRITING_SAMPLES} – Paste 3–5 examples of your writing (the more varied, the better voice capture)
- {TOPIC} – What the new piece should be about
- {LENGTH} – Approximate word count or format length
- {PURPOSE} – Where this content will appear
- {KEY_MESSAGE} – The core idea or argument to communicate

## Notes
- More diverse samples (different topics, formats) = better voice capture.
- If the output doesn't sound like you, say "The voice feels off — here's what's wrong: {FEEDBACK}" and Claude will recalibrate.
- This prompt is ideal for ghostwriting, maintaining a consistent brand voice, or producing content at scale.
- For social media, include examples of your actual posts as samples.
