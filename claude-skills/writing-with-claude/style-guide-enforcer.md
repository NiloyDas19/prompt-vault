---
title: "Style Guide Enforcer"
category: Claude Skills
subcategory: Writing with Claude
tags: [writing, style-guide, brand-voice, editing, consistency]
model: claude
---

## Purpose
Edit a piece of writing to strictly conform to a specific style guide (AP, Chicago, company brand guide, etc.) and flag every deviation with an explanation.

## Prompt
You are a rigorous copy editor with expertise in {STYLE_GUIDE}. Edit the following content to conform perfectly to the style guide rules I specify. Flag every change with an explanation.

<style_guide_rules>
{STYLE_GUIDE_RULES}
</style_guide_rules>

<content_to_edit>
{CONTENT}
</content_to_edit>

<editing_priorities>
1. Correct all rule violations — do not leave any violations
2. Preserve the author's meaning — change style only, not substance
3. Flag every change so the author can learn from it
</editing_priorities>

Please provide:
1. **Edited content** — The fully corrected version
2. **Change log** — A numbered list of every change made:
   - Original text → Edited text
   - Rule violated → Correct rule
   - Brief explanation
3. **Pattern analysis** — What style violations appeared most frequently? (Helps the author improve)
4. **Unresolved issues** — Any cases where the style guide doesn't provide clear guidance, with your recommendation

## Variables
- {STYLE_GUIDE} – The style guide to apply (e.g., AP Style, Chicago Manual of Style 17th ed., APA 7th, your company's brand guide)
- {STYLE_GUIDE_RULES} – The specific rules to enforce. Either:
  a) Reference a known guide: "Standard AP Style rules"
  b) Paste your custom rules: "1. Always use Oxford comma. 2. Numbers under 10 spelled out. 3. Never use passive voice. 4. Product names always capitalized. 5. No exclamation marks except in direct quotes."
- {CONTENT} – The text to edit

## Notes
- For company-specific brand guides, paste the actual rules directly — Claude cannot access external URLs.
- The more specific your rules, the more precise the editing.
- Use this as a final pass before publishing or submitting content.
- For very long documents, process section by section to maintain output quality.
