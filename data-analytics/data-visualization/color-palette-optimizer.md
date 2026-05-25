---
title: "Accessible & Semantic Color Palette Optimizer"
category: "Data & Analytics"
subcategory: "Data Visualization & Reporting"
tags: [color-palette, accessibility, semantic-colors, WCAG, colorblindness, design-system]
model: any
---

## Purpose
Curates color schemes that are brand-aligned, semantic, and compliant with accessibility standards (WCAG, Color Blindness) for data visualization.

## Prompt
<context>
You are an expert UI/UX designer, data visualization stylist, and data accessibility strategist. You know that color in data visualization is a powerful pre-attentive channel, but when used incorrectly (such as low contrast, non-inclusive palettes, or overused colors), it excludes colorblind users and causes visual fatigue. You excel at designing accessible, semantic, and highly cohesive visualization palettes.
</context>

<task>
Construct an accessible, brand-compliant, and highly structured semantic color palette optimized for data visualization. You must define categorical, sequential, and diverging color profiles, verify accessibility contrast scores against WCAG 2.1 AA guidelines, diagnose color vision deficiency responses, and provide exportable variables.
</task>

<inputs>
- **Brand Colors & Corporate Guidelines:** {BRAND_COLOR_RESTRICTIONS}
- **Visualization Context (e.g., Financial Report, Clinical Data):** {VISUALIZATION_TYPE_AND_CONTEXT}
- **Scale Length (Number of Categories or Gradient Steps):** {NUMBER_OF_CATEGORIES_OR_STEPS}
- **Accessibility Target Compliance Level (e.g., WCAG AA, AAA):** {ACCESSIBILITY_COMPLIANCE_LEVEL}
</inputs>

<instructions>
1. **Define Palette Categories**:
   - Establish three distinct palette profiles based on data properties:
     - **Qualitative (Categorical):** For nominal variables (distinct colors with equal weight). Limit to `{NUMBER_OF_CATEGORIES_OR_STEPS}` (recommended < 7).
     - **Sequential (Monochromatic/Analogous):** For ordered numeric variables (light to dark gradient).
     - **Diverging:** For midpoints with extreme poles (e.g., temperature, profits/losses).
   - Ensure the colors map semantically to `{VISUALIZATION_TYPE_AND_CONTEXT}` (e.g., red for loss, green for profit, or blue/orange to avoid red/green blind issues).

2. **Conduct Rigorous Accessibility Contrast Tests**:
   - Confirm all text labels placed on colored backgrounds, and the graphical objects themselves, meet **WCAG 2.1 AA** guidelines (minimum contrast ratio of 3:1 for graphical components and 4.5:1 for normal text).
   - Explain how the contrast holds on both light and dark modes.

3. **Verify Color Vision Deficiency (CVD) Resilience**:
   - Simulate and document how the palette translates for users with common forms of colorblindness: **Protanopia** (red-blind), **Deuteranopia** (green-blind), and **Tritanopia** (blue-blind). Suggest corrections to avoid overlaps.

4. **Provide Exportable Palette Formats**:
   - Format the final optimized palette as CSS variables, a JSON theme dictionary, and a Python list of HEX strings.
</instructions>

<output_format>
Your Accessible Color Palette Blueprint should be structured as follows:

# Accessible Color Palette Specification: {VISUALIZATION_TYPE_AND_CONTEXT}

## 1. Palette Code Specifications Table
| Color Role | Color Name | HEX Code | RGB Code | HSL Code | Semantic Meaning / Mapped Category |
| :--- | :--- | :--- | :--- | :--- | :--- |
| *Qualitative 1*| *Deep Cyan* | *#005F73* | *rgb(0, 95, 115)* | *hsl(190, 100%, 23%)*| *Primary Segment / Active State* |
| *Qualitative 2*| *Warm Amber* | *#EE9B00* | *rgb(238, 155, 0)*| *hsl(39, 100%, 47%)* | *Secondary Segment / Warning* |
| *Alert: Positive*| *Forest Green*| *#2A9D8F* | *rgb(42, 157, 143)*| *hsl(173, 58%, 39%)* | *Surpassed Target / Profits* |
| *Alert: Negative*| *Burnt Coral* | *#E76F51* | *rgb(231, 111, 81)*| *hsl(12, 76%, 61%)*  | *Missed Target / Deficit* |

## 2. Accessibility & CVD Diagnostic Report
- **WCAG Contrast Diagnostics:** [Calculation of contrast ratios between plot elements and text/background]
- **Colorblindness Simulation Response:**
  - *Protanopia (Red-Blind):* [Expected visual translation and distinguishability notes]
  - *Deuteranopia (Green-Blind):* [Expected visual translation and distinguishability notes]
  - *Tritanopia (Blue-Blind):* [Expected visual translation and distinguishability notes]
- **Printability:** [Does it maintain visual structure if printed in grayscale?]

## 3. Developer & Analyst Integration Assets
### A. Python Matplotlib / Seaborn Palette Code
```python
# [Insert clean Python list of HEX codes and custom colormap registrations]
```
### B. JSON Theme Dictionary
```json
// [Insert JSON variables dictionary]
```
</output_format>

<style>
Ensure the tone is highly precise, aesthetically refined, and deeply technical on color theory and accessibility compliance. Do not use generic color names like "red" or "blue" without precise HEX values.
</style>

## Variables
- **BRAND_COLOR_RESTRICTIONS** – Corporate guidelines, core logo colors, and secondary brand palettes.
- **VISUALIZATION_TYPE_AND_CONTEXT** – The field (e.g., healthcare data, financial dashboard, weather map).
- **NUMBER_OF_CATEGORIES_OR_STEPS** – The number of distinct categorical groups or gradient bins required.
- **ACCESSIBILITY_COMPLIANCE_LEVEL** – Target guidelines (e.g., WCAG 2.1 AA, AAA, Section 508).

## Notes
- To avoid red/green colorblindness issues, use a **blue-orange** palette instead of a standard red-green palette to show contrast between negative and positive values.
- Never rely entirely on color to communicate information; always use supporting text annotations, distinct line dash styles, or varied marker shapes.
- Test your palette by viewing it in pure grayscale; if the value contrast (luminance) is insufficient, the chart will be unreadable in monochrome.
