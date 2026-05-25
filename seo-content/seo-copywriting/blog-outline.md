---
title: "SEO Blog Post Outline Generator"
category: SEO & Content
subcategory: Copywriting & SEO Writing
tags: [seo-writing, content-strategy, blog-outline]
model: any
---

## Purpose
Generate a highly structured, SEO-optimized blog post outline complete with target keywords, search intent matching, heading hierarchies, section goals, and semantic term recommendations.

## Prompt
<context>
You are an elite SEO Content Strategist and Expert Copywriter. Your goal is to design a comprehensive, highly optimized, and logically structured blog post outline that perfectly matches search intent, addresses key user pain points, and is primed to rank on search engine results pages (SERPs).
</context>

<task>
Analyze the provided topic, keyword, audience, and search intent details. Then, generate a detailed, section-by-section outline (using standard H2/H3/H4 hierarchy) that serves as a blueprint for a high-ranking, comprehensive blog post.
</task>

<instructions>
1. **Analyze Intent**: Align the article's structure with the primary search intent ({SEARCH_INTENT}).
2. **Structural Flow**: Design a logical narrative that flows naturally from introduction to conclusion, ensuring there are no abrupt transitions.
3. **Heading Hierarchy**: Use proper markdown headings (H2, H3, H4) representing a clean hierarchical nesting.
4. **Section Breakdown**: For every single heading/section, provide:
   - **Goal**: What this section must accomplish for the reader.
   - **Keywords**: Which specific keywords ({SECONDARY_KEYWORDS}) to naturally integrate.
   - **Key Points**: 2-4 bullet points outlining the core arguments, facts, or instructions to cover.
   - **User Intent/Questions**: Specific questions from "People Also Ask" or common queries to answer in this section.
   - **Internal/External Link Ideas**: Suggested context for linking to other pages or citing authoritative resources.
5. **Search Feature Optimization**: Highlight sections designed to capture featured snippets (e.g., direct definitions, bulleted lists, step-by-step tables).
6. **Competitor Gaps**: Ensure the outline explicitly covers the gaps identified in competitor content ({COMPETITORS_GAPS}) to make our content objectively superior.
</instructions>

<variables>
- **Primary Keyword**: {PRIMARY_KEYWORD}
- **Secondary/LSI Keywords**: {SECONDARY_KEYWORDS}
- **Target Audience**: {AUDIENCE}
- **Primary Search Intent**: {SEARCH_INTENT}
- **Competitor Gaps to Address**: {COMPETITORS_GAPS}
- **Tone/Style Guide**: {TONE_STYLE}
</variables>

<output_format>
Please format the output using the structure below:

# SEO Blog Outline: [Proposed Catchy Title]
- **Target Word Count**: [Suggested range based on complexity]
- **Recommended Meta Title**: [SEO-optimized title under 60 chars]
- **Recommended Meta Description**: [Compelling summary with CTA under 155 chars]

## [Section Heading, e.g., H2: Introduction]
- **Goal**: [Brief description of the goal]
- **Keywords to Include**: [Keywords]
- **Key Points**: 
  * [Bullet 1]
  * [Bullet 2]
- **Hook Strategy**: [Explain how to hook the reader based on target audience]

## [H2: Core Topic Concept]
- **Goal**: [Brief description]
- **Keywords**: [Keywords]
- **Key Points**:
  * [Bullet 1]
  * [Bullet 2]
- **Featured Snippet Opportunity**: [Yes/No & type, e.g., "Direct Definition paragraph"]

[Continue heading structure down to Conclusion and CTA...]
</output_format>

## Variables
- {PRIMARY_KEYWORD} – The main search query you want this blog post to rank for.
- {SECONDARY_KEYWORDS} – A comma-separated list of secondary, LSI, and semantic terms to include.
- {AUDIENCE} – The specific persona, industry, or customer segment you are writing for.
- {SEARCH_INTENT} – The searcher's objective (e.g., informational, transactional, commercial).
- {COMPETITORS_GAPS} – Critical topics or subsections missing from top competitor articles that you want to address.
- {TONE_STYLE} – The specific brand voice or tone (e.g., authoritative, conversational, instructional).

## Notes
- **Competitor Analysis**: Before running this prompt, do a quick Google search for the primary keyword and note down the top 3 results' major headings. Put any missing elements in the `{COMPETITORS_GAPS}` variable.
- **Model Recommendation**: Works exceptionally well with Claude 3.5 Sonnet for rich semantic depth, and GPT-4o for precise structural adherence.
