---
title: "FAQ Schema Generator"
category: Marketing & Sales
subcategory: SEO & Content
tags: [seo, FAQ, schema, structured-data, featured-snippet]
model: any
---

## Purpose
Generate SEO-optimized FAQ sections with JSON-LD schema markup ready to paste into your page for rich results in Google.

## Prompt
Generate a complete FAQ section for the following page, optimized for "People Also Ask" featured snippets and FAQ rich results.

**Page Topic:** {PAGE_TOPIC}
**Target Keyword:** {TARGET_KEYWORD}
**Page Type:** {PAGE_TYPE}
**Target Audience:** {AUDIENCE}

### 1. FAQ Content (10 questions)
For each Q&A:
- **Question** — Written exactly as someone would type or ask Google
- **Answer** — 40–60 words (the ideal length for featured snippets). Must be direct, authoritative, and self-contained.
- **Extended Answer** — An additional 2–3 sentences for the page (provides more depth than the snippet)
- **Source/Citation** — What data or authority backs this answer

Organize questions by intent:
- **Definitional** (3): "What is..." / "What does... mean?"
- **Process/How-to** (3): "How do I..." / "How does... work?"
- **Comparison** (2): "What's the difference between..." / "Is X better than Y?"
- **Cost/Value** (2): "How much does... cost?" / "Is it worth it?"

### 2. JSON-LD Schema Markup
- Provide the complete, valid JSON-LD FAQPage schema markup ready to paste into the page's `<head>` or `<body>`
- Include all 10 Q&As in the schema

### 3. Placement Recommendations
- Where on the page to place the FAQ section for maximum SEO benefit
- How to format the FAQ section for readability (accordion vs. open, etc.)

## Variables
- {PAGE_TOPIC} – What the page is about
- {TARGET_KEYWORD} – Primary keyword
- {PAGE_TYPE} – Type (e.g., "product page", "service page", "blog post", "landing page")
- {AUDIENCE} – Who's asking these questions

## Notes
- FAQ rich results can increase your SERP real estate by 2–3x, pushing competitors down the page.
- Google has tightened FAQ rich result eligibility — they now only show for government and health authority sites in many cases. However, the FAQ content itself still helps with "People Also Ask" placements.
- Keep answers concise. Google's featured snippet sweet spot is 40–60 words.
