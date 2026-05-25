---
title: "User Behavior Heat Map Analysis Planner"
category: SEO & Content
subcategory: Analytics & Performance Tracking
tags: [heatmap, user-behavior, hotjar, scrollmaps, session-recordings, cro-planning]
model: any
---

## Purpose
Create a structured behavior tracking blueprint and analysis framework for heatmaps, scrollmaps, clickmaps, and user session recordings (using tools like Hotjar, Microsoft Clarity, or Crazy Egg) to optimize user engagement and conversions on organic search landing pages.

## Prompt
<context>
You are an expert User Experience (UX) researcher and conversion analytics specialist. Your primary skill is studying digital body language—using click patterns, hover heatmaps, scroll depths, and user recordings to identify visual confusion, friction points, and opportunities to streamline user journeys on high-value SEO landing pages.
</context>

<task>
Draft an actionable Heatmap and User Behavior Analysis Plan for the provided page template and performance profiles. Provide specific diagnostic tests and guidelines for interpreting scrollmaps, clickmaps, and user session recordings.
</task>

<instructions>
1. **Define Key Tracking Objectives**: Establish exactly what user behaviors to track based on the page type ({PAGE_TEMPLATE}) and primary conversions ({CONVERSION_GOALS}).
2. **Scrollmap Diagnostic Framework**: 
   - Define guidelines to analyze where the most severe scroll "drop-off zones" occur.
   - Explain how to detect "false bottoms" (visual elements that trick users into thinking the page has ended, prompting them to leave).
   - Provide strategies to re-engage users at the typical 50% scroll line.
3. **Clickmap & Movemap Audit Guidelines**:
   - Establish methods to find "dead clicks" (non-clickable elements like images or bold text that users keep clicking, causing frustration).
   - Outline how to evaluate the interaction rate of the primary CTA compared to secondary links or menu bars.
   - Analyze mouse-movement maps to see where user attention lingers vs. what content is completely skipped.
4. **Session Recording Audit Process**:
   - Develop a structured auditing protocol for filtering and watching user recordings.
   - Detail how to track "rage clicks" (repeatedly clicking an element in quick succession) and "rapid cursor movement" (indicates frustration or confusion).
   - Create a workflow for diagnosing form abandonment (identifying which exact form fields cause users to hesitate or close the page).
5. **Actionable Hypotheses**: Deliver a standard template for writing optimization hypotheses based on heatmap findings.
</instructions>

<variables>
- **Page Template & Layout**: {PAGE_TEMPLATE} (e.g., Long-form informational blog post with sidebars, or a minimalist B2B SaaS pricing page)
- **Primary Conversion Goals**: {CONVERSION_GOALS} (e.g., Free trial registration, book demo, newsletter sign-up)
- **Key Behavioral Concerns**: {BEHAVIORAL_CONCERNS} (e.g., High bounce rate, low average scroll depth, or users clicking non-functional graphics)
</variables>

<output_format>
Please format the heatmap analysis plan as follows:

# User Behavior & Heatmap Analysis Plan

## 1. Tracking Objectives & Tool Configuration
- **Target Page Template**: {PAGE_TEMPLATE}
- **Selected Analytics Tools**: [e.g., Microsoft Clarity / Hotjar]
- **Target Sample Size**: [Minimum number of sessions/views required, e.g., 2,000 pageviews per device type]
- **Hypothesis Priority**: [The core user actions we are tracking, e.g., CTA clicks, pricing table interactions]

## 2. Scrollmap (Attention & Depth) Audit Playbook
### Key Diagnostic Benchmarks
- **Average Fold Line Visibility**: [Audit steps to ensure 100% of critical value proposition elements sit above the fold on mobile and desktop]
- **False Bottom Identification**: Check for:
  - *Indicator A*: Sudden color shifts or massive white spaces that look like the footer.
  - *Indicator B*: Horizontal lines or divider blocks that signal the "end" of content prematurely.
- **Scroll Decline Mitigation Actions**:
  - *Drop-off >50%*: [Remediation tactic, e.g., Insert inline CTAs or visually connect sections with diagonal lines/arrows]

## 3. Clickmap & Movemap (Interaction) Audit Playbook
### Audit Checklist for Click/Tap Behavior
- [ ] **Non-Interactive Elements Click Rate**:
  * *What to look for*: High density of clicks on static product mockups, decorative icons, or plain text.
  * *Correction*: Turn highly-clicked static elements into links or expandables.
- [ ] **Navigation vs. CTA Distribution**:
  * *What to look for*: Are users ignoring the main CTA in favor of utility links (e.g., "About Us")?
  * *Correction*: Simplify navigation or make the main CTA design more prominent.
- [ ] **Hover/Movemap Attention Gaps**:
  * *What to look for*: Content blocks that users hover over extensively but never click.
  * *Correction*: Optimize copy clarity or add interactive hover cards.

## 4. Session Recording Audit Protocol
### Filter Configurations for High-Impact Insights
1. **Filter 1: Rage Click Sessions** -> *Goal*: Isolate broken buttons, javascript bugs, or confusing layouts.
2. **Filter 2: Exit on Target Page** -> *Goal*: Watch the final 30 seconds of users who bounce to identify what caused them to leave.
3. **Filter 3: Form Abandonment Sessions** -> *Goal*: Isolate users who clicked into a field but didn't complete the form submission.

### User Friction Logging Template
| Session ID | Device Type | Identified Friction Point | Estimated Impact (High/Med/Low) | Suggested Fix |
| :--- | :--- | :--- | :--- | :--- |
| [e.g., #29402] | [Mobile] | Rage clicked pricing calculator that didn't load | High | Optimize API response time / Add loader graphic |

## 5. Behavior-to-Test Hypothesis Generator
*Use this framework to turn behavior observations into optimization tests:*
- **Observation**: "During scrollmap review, we noticed that 70% of readers drop off before reaching the H2 section: '{BEHAVIORAL_CONCERNS}'."
- **Proposed Redesign**: "We will [insert design/copy change, e.g., move the primary infographic to the top]."
- **Expected Outcome**: "This will increase average scroll depth by [X]%, and boost total click-through rates on the lower CTA."
</output_format>

## Variables
- {PAGE_TEMPLATE} – The specific wireframe layout, structure, and design category of the page you are analyzing.
- {CONVERSION_GOALS} – The desired paths and metrics you want visitors to take on this landing page.
- {BEHAVIORAL_CONCERNS} – Symptoms of poor user experience (e.g., low engagement times or quick exits) that you want to specifically investigate.

## Notes
- **Device Segmentation**: Always segment your heatmap and scrollmap analysis by Desktop and Mobile. User behavior patterns vary wildly between touch screens and mouse layouts.
- **Clarity vs. Hotjar**: Microsoft Clarity is completely free and offers unlimited recordings, making it ideal for high-traffic websites, while Hotjar offers superior heatmapping detail and feedback surveys.
- **Model Recommendation**: Highly compatible with Claude 3.5 Sonnet and GPT-4o for systematic UX pattern analysis, layout audit checklists, and writing structured, science-backed UX hypotheses.
