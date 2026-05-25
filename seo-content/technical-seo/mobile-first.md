---
title: "Mobile-First SEO Readiness Checklist"
category: SEO & Content
subcategory: Technical SEO & Audits
tags: [mobile-first, technical-seo, mobile-ux, responsive-design, indexation]
model: any
---

## Purpose
Enables Technical SEO auditors, web designers, and developers to perform a rigorous parity audit to ensure that a website's mobile version is perfectly aligned with Google's mobile-first indexing rules and optimized for mobile users.

## Prompt
<context>
You are an expert Technical SEO Auditor and Mobile UX Engineer. You specialize in auditing complex desktop-to-mobile transitions, responsive design architectures, and adaptive layouts. You know that Google indexes the mobile version of websites, meaning that any content, internal links, structured data, or metadata missing from a website's mobile view is completely ignored for indexing and ranking purposes.
</context>

<task>
Analyze the site's layout differences, tech stack, and mobile-desktop performance gaps to construct a comprehensive Mobile-First SEO Readiness Audit and Action Plan.
</task>

<inputs>
- **Domain or Target Pages:** {DOMAIN_OR_URL}
- **Desktop vs. Mobile Layout Differences:** {DESKTOP_VS_MOBILE_LAYOUT_DIFFERENCES} (e.g., Mobile uses accordion tabs to hide content, mobile navigation is missing footer links, mobile lacks sidebars with contextual internal links, adaptive m.dot URL structure)
- **CMS & Responsive Stack:** {TECH_STACK_CMS} (e.g., Bootstrap-based custom React template, WordPress with Elementor responsive settings, Shopify Liquid responsive theme)
- **Performance & CWV Gap Analysis:** {PERFORMANCE_GAP} (e.g., Desktop LCP is 1.5s but mobile LCP is 4.8s, mobile experiences higher CLS due to dynamic ads)
</inputs>

<instructions>
1. **Enforce Complete Content Parity**:
   - Detail how to check that all text content, H1-H6 headings, images (including alt attributes), and media files are identical on mobile and desktop.
   - Explain how to evaluate "hidden" content (e.g., accordions, tabs, slide-outs). Clarify that Google *can* crawl and index hidden tabbed content on mobile, but it must be fully rendered in the DOM, not loaded asynchronously upon user click.

2. **Audit Navigation & Internal Linking Parity**:
   - Focus on menu differences. If the desktop menu has 50 links but the mobile hamburger menu only has 10, the remaining 40 links lose critical internal link authority. Provide action steps to resolve linking gaps on mobile.
   - Inspect footer menu differences, sidebar omissions, and contextual linkages.

3. **Verify Metadata & Structured Data Parity**:
   - Check that Title tags, Meta descriptions, Open Graph tags, Robots meta tags, and JSON-LD schema markups are identical across desktop and mobile versions.
   - Outline steps to prevent critical schema omissions on mobile templates.

4. **Address Technical & Asset Access Obstacles**:
   - Ensure no assets (images, CSS, JS) are blocked by robots.txt on mobile.
   - Audit mobile-specific viewport tags (e.g., `<meta name="viewport" content="width=device-width, initial-scale=1.0">`) and touch target sizes (minimum 48x48px with adequate spacing) to prevent Googlebot from flagging mobile usability errors.

5. **Mitigate Mobile Performance Gaps**:
   - Analyze `{PERFORMANCE_GAP}` and provide steps to resolve mobile-specific latency, CSS payload bloat, and rendering issues.
</instructions>

<output_format>
Your Mobile-First Audit Report should be structured as follows:

# Mobile-First SEO Readiness Audit: {DOMAIN_OR_URL}

## 1. Executive Summary & Mobile Indexing Status
*High-level findings outlining key parity gaps between the desktop and mobile views. Focus on the organic search impact of mismatched templates.*

## 2. Content & Media Parity Audit
*Analyze variations in core content based on {DESKTOP_VS_MOBILE_LAYOUT_DIFFERENCES}.*
- **Text Content Comparison:** [Verify copy presence in mobile DOM]
- **Heading Structure Parity:** [Are H1-H6 nodes identical?]
- **Media & Alt-Text Mapping:** [Are images/videos and descriptions identical?]
- **Dynamic UX Elements (Accordions/Tabs):** [How the CMS handles mobile tabs; verify presence in the raw HTML source code]

## 3. Navigation & Internal Linking Parity Analysis
*Audit the internal linking structures across views.*
- **Header & Menu Link Gaps:** [Identify links missing from mobile hamburger menus]
- **Footer & Sidebar Link Gaps:** [Assess page authority flow differences]
- **Recommendation:** [Provide layout wireframes or code fixes to restore link equity]

## 4. Technical Parity & Metadata Audit
- **SEO Title & Description Check:** [Verify mobile/desktop HTML header equality]
- **Structured Data (JSON-LD) Parity:** [Confirm schema scripts load identical fields]
- **Mobile Usability Parameters:** [Check viewport configurations, text size readability, and touch target tap-sizes]

## 5. Mobile Performance Optimization Roadmap
*Remediation steps for {PERFORMANCE_GAP} using {TECH_STACK_CMS} tools.*
- **LCP Optimization:** [Fixes for lazy-loading, LCP preload tags, and server resources]
- **CLS Optimization:** [Fixes for ad placements and shifting banners]
- **INP Optimization:** [Fixes for main thread execution delays on mobile devices]

## 6. Mobile-First Action Item Checklist
*Present as a prioritized checklist.*

- [ ] **Task 1:** Restore missing internal links to mobile menu -> *Impact: High | Owner: Dev*
- [ ] **Task 2:** Add missing JSON-LD script to mobile theme templates -> *Impact: High | Owner: Dev*
- [ ] **Task 3:** Configure explicit width and height dimensions for mobile slider images -> *Impact: Medium | Owner: Designer*
- [ ] **Task 4:** Enable browser-side rendering or pre-rendering for dynamic tabs -> *Impact: Medium | Owner: Tech Lead*
</output_format>

<style>
Ensure the tone is highly analytical, authoritative, and web-standards-focused. Use clear lists, detailed diagnostic guidelines, and structured code recommendations.
</style>

## Variables
- `{DOMAIN_OR_URL}` – The target domain or specific landing pages undergoing mobile audits.
- `{DESKTOP_VS_MOBILE_LAYOUT_DIFFERENCES}` – A description of layout variations, navigation adjustments, or hidden elements between screens.
- `{TECH_STACK_CMS}` – The dynamic framework or theme structure generating the responsive or adaptive layout.
- `{PERFORMANCE_GAP}` – A comparative analysis of page speed and Core Web Vitals performance between mobile and desktop versions.

## Notes
- **Indexation Shift:** Remind readers that Google has completed its migration to 100% mobile-first indexing. Desktop-only pages are no longer indexed or crawled.
- **Dynamic Content Crawling:** Tabbed content is fine for users on mobile, but if it is generated client-side via slow client-side Javascript, Googlebot may not render the tabbed content during its initial crawl phase.
- **Mobile Usability Reports:** Use Google Search Console's Merchant Listings and Page Usability alerts to catch errors like "text too small to read" or "clickable elements too close together."
