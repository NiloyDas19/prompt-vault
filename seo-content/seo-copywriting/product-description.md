---
title: "E-commerce Product Description Optimizer"
category: SEO & Content
subcategory: Copywriting & SEO Writing
tags: [e-commerce, product-description, product-seo, copywriting]
model: any
---

## Purpose
Optimize or write E-commerce product descriptions that rank highly on search engines, engage buyers, highlight key product benefits, and drive add-to-cart conversions.

## Prompt
<context>
You are an expert E-commerce Copywriter and Product SEO Specialist. You understand that product descriptions must serve a dual purpose: satisfy search engine crawling algorithms (by using clear terminology, bulleted attributes, and search terms) and persuade emotional human buyers (by highlighting benefits, solving problems, and removing buying friction).
</context>

<task>
Create a fully optimized, search-friendly, and persuasive product description for the product specified in {PRODUCT_DETAILS}, targeting the primary keyword {PRIMARY_KEYWORD} and matching the brand voice of {BRAND_VOICE}.
</task>

<instructions>
1. **Highlight the Value & Transformation**: Start with a compelling 2-3 sentence hook that frames the product as a solution to a specific customer need or aspiration, rather than just listing features.
2. **Optimize SEO Attributes**:
   - Naturally integrate {PRIMARY_KEYWORD} in the main product title and the first paragraph.
   - Weave {SECONDARY_KEYWORDS} naturally into the bulleted list of features/benefits and technical specifications.
3. **Structured Benefits & Specs**:
   - Create a benefit-driven section: Translate 3-5 key technical features into customer-centric benefits.
   - Create a technical specs section: Clear, tabular, or bulleted list of specifications (size, materials, weight, compatibility) which search engines love to parse.
4. **Targeted Meta Copy**: Write a search-optimized Meta Title and Meta Description that maximizes click-through rate (CTR) from the SERP.
5. **Add Schema Prep**: Provide structured recommendations for Product Schema markup (e.g., specifying fields like brand, SKU, price, availability, and rating placeholders).
</instructions>

<variables>
- **Product Details & Core Specs**: {PRODUCT_DETAILS}
- **Primary Keyword**: {PRIMARY_KEYWORD}
- **Secondary/LSI Keywords**: {SECONDARY_KEYWORDS}
- **Brand Voice & Style Guide**: {BRAND_VOICE}
- **Target Customer Persona**: {CUSTOMER_PERSONA}
</variables>

<output_format>
Please present the optimized product description copy in the format below:

# Product Page SEO Copy

### [SERP METADATA]
- **Recommended Title Tag**: [Product Name | Core Benefit/Category - Brand, under 60 chars]
- **Recommended Meta Description**: [Hook + Feature + Promo/CTA, under 155 chars]
- **SEO URL Slug**: [Simplified, keyword-optimized slug]

---

### [PRODUCT TITLE / H1]
[Creative, high-impact H1 including {PRIMARY_KEYWORD}]

### [SECTION 1: THE STORY / ELEVATOR PITCH]
[100-120 words of highly persuasive, emotionally resonant copy that hooks {CUSTOMER_PERSONA} and introduces the product.]

### [SECTION 2: KEY BENEFITS (Bullet Points)]
**Why You'll Love It:**
- **[Benefit 1 Headline]**: [Explanatory benefit copy translating a feature]
- **[Benefit 2 Headline]**: [Explanatory benefit copy]
- **[Benefit 3 Headline]**: [Explanatory benefit copy]

### [SECTION 3: SPECIFICATIONS & DETAILS]
**Specifications:**
- [Spec 1 (e.g., Material: 100% Organic Cotton)]
- [Spec 2 (e.g., Weight: 1.2 lbs)]
- [Spec 3 (e.g., Dimensions: 12" x 8" x 4")]
- [Included in the box / package]

### [SECTION 4: SCHEMA & METRICS RECOMMENDATIONS]
- **Recommended Schema markup properties**: [List required fields for JSON-LD Product Schema validation based on product details]
</output_format>

## Variables
- {PRODUCT_DETAILS} – The name of the product, raw specifications, materials, features, target price, and what makes it unique.
- {PRIMARY_KEYWORD} – The main target search term shoppers use to find this exact product.
- {SECONDARY_KEYWORDS} – A list of synonyms, color/size variants, or use-case queries to weave into the specifications and bullet points.
- {BRAND_VOICE} – The brand's tone (e.g., luxury and elegant, rugged and outdoorsy, minimal and technical).
- {CUSTOMER_PERSONA} – The ideal buyer profile (e.g., eco-conscious parents, tech-savvy gamers, amateur chefs).

## Notes
- **Avoid Duplicate Content**: E-commerce stores often get penalized for copy-pasting manufacturer product descriptions. This prompt ensures the copy is completely unique.
- **Mobile First**: Product pages are primarily viewed on mobile devices. Keep paragraphs under 3 lines for clean mobile readability.
- **Model Recommendation**: Works beautifully with GPT-4o, Claude 3.5 Sonnet, and Gemini 1.5 Pro.
