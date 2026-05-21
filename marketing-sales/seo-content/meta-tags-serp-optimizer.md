---
title: "Meta Tags & SERP Optimizer"
category: Marketing & Sales
subcategory: SEO & Content
tags: [seo, meta-tags, SERP, titles, click-through-rate]
model: any
---

## Purpose
Generate optimized title tags, meta descriptions, and structured data suggestions that maximize click-through rates from search engine results pages.

## Prompt
Generate SEO-optimized meta tags for the following pages. Optimize for both search engine ranking AND human click-through rates.

**Pages to optimize:**
{PAGES_LIST}

For each page, provide:

### Title Tags (3 variations each)
- Under 60 characters (critical — longer titles get truncated)
- Primary keyword near the beginning
- Variation 1: Direct and keyword-focused
- Variation 2: Curiosity-driven (question or number)
- Variation 3: Power words and emotional triggers
- For each: character count and whether the keyword appears in the first 3 words

### Meta Descriptions (2 variations each)
- Under 155 characters
- Include primary keyword naturally
- Compelling reason to click (benefit, statistic, or value prop)
- Include a subtle CTA ("Learn how", "Discover", "Get the guide")
- For each: character count

### Open Graph Tags
- og:title (may differ from SEO title — optimize for social sharing)
- og:description (more conversational than meta description)
- Suggested og:image specifications

### Structured Data Suggestions
- Recommend appropriate schema markup type (Article, FAQ, HowTo, Product, Review, etc.)
- Sample FAQ schema questions (if applicable)

### SERP Preview
- Show exactly how the listing would appear in Google search results
- Flag any truncation issues

## Variables
- {PAGES_LIST} – List each page with: URL, primary keyword, page type (e.g., "Homepage — 'project management software'", "Blog post — 'how to run a sprint retrospective'")

## Notes
- Title tags are the single highest-impact on-page SEO element. Changing a title tag alone can move rankings 5–10 positions.
- Meta descriptions don't directly affect rankings, but they dramatically affect click-through rate — which indirectly affects rankings.
- Use numbers, parentheses, and the current year to boost CTR: "10 Best Tools (2024 Guide)" outperforms "Best Tools Guide."
- Google rewrites meta descriptions ~70% of the time. Write them anyway — they still influence clicks when Google uses yours.
