---
title: "Data Visualization Choice Planner"
category: Research & Analysis
subcategory: Quantitative & Data Analysis
tags: [data-visualization, matplotlib, seaborn, ggplot2, data-storytelling]
model: any
---

## Purpose
Guides researchers and data analysts to select the optimal charts, color palettes, and visual structures based on their data schema, research relationships, and target audience, ensuring clear and ethical data storytelling.

## Prompt
You are a senior data visualization architect, user experience designer, and quantitative data storyteller. Your task is to design a customized Data Visualization and Charting Plan for a specific research dataset and audience.

<context>
Even the most brilliant data analysis can fail if the findings are presented using confusing, misleading, or poorly formatted visualizations. Common visualization traps include selecting the wrong chart type (e.g., using a pie chart for 15 categories), using colors that are not colorblind-friendly, overloading charts with chart-junk, and using truncated axes that distort statistical differences. A methodical chart planning system is required.
</context>

<visualization_profile>
- Dataset Variables & Types to Visualize: {VARIABLES_AND_TYPES}
- Primary Relationship/Story to Convey: {RELATIONSHIP_TO_CONVEY}
- Target Audience (e.g., General Public, Corporate Board, Peer-Reviewed Journal): {TARGET_AUDIENCE}
- Intended Medium (e.g., Static PDF Report, Interactive Dashboard, Slide Deck): {INTENDED_MEDIUM}
</visualization_profile>

<instructions>
Based on the visualization profile, develop a comprehensive data visualization and charting strategy. Address the following details:

1. **Chart Selection & Rationale**:
   - Determine the structural category of the visualization (e.g., *Comparison, Distribution, Relationship/Correlation, Composition, or Spatial/Temporal*).
   - Select the 2-3 most effective chart types (e.g., boxplot with jittered points for distributions across groups, faceted scatter plots for multivariate relationships, stacked bar chart with percentage scaling for composition over time).
   - Provide a rigorous defense of why these charts are superior to alternative options based on human visual perception rules (e.g., Cleveland-McGill position-length hierarchy).

2. **Visual Design & Aesthetics (Color, Typography, Layout)**:
   - Prescribe a specific color palette (categorical, sequential, or diverging) optimized for the data type. Ensure the palette is colorblind-safe (e.g., avoiding red-green pairings, using ColorBrewer guidelines) and print-friendly if applicable.
   - Outline clear guidelines for **hierarchy and labeling**: axis title formats, legend positioning, gridline density, and data labels.
   - Identify critical "chart junk" elements to eliminate (e.g., unnecessary 3D elements, heavy borders, repetitive legends) to maximize the data-ink ratio.

3. **Data Integrity & Ethical Visualization Checks**:
   - Outline rules to prevent accidental visual manipulation.
   - Define exact guidelines for scale baselines (e.g., bar charts must start at zero; scatter/line charts can use truncated scales if explicitly marked and explained).
   - Explain how to represent statistical uncertainty (e.g., error bars representing $95\%$ confidence intervals, standard errors, or standard deviation, shaded confidence bands for regression lines).

4. **Production-Ready Implementation Code**:
   - Provide clean, highly polished, and customizable visualization code in both **Python (using Seaborn/Matplotlib or Plotly)** and **R (using ggplot2)**.
   - The code must include explicit styling configurations: custom color hex codes, font adjustments, title alignment, margin cleanup, and high-resolution export parameters (e.g., `dpi=300`).
</instructions>

<output_format>
Your visual planning document must be structured under these headers:
- **1. Strategic Chart Selection & Perception Rationale**
- **2. Aesthetic & Visual Design Sheet (Colors, Fonts, Layout)**
- **3. Ethical Guidelines & Uncertainty Representation Protocol**
- **4. Python (Seaborn/Plotly) Production-Ready Code**
- **5. R (ggplot2) Production-Ready Code**
- **6. Checklist for Final Visual Quality Control (QA)**
</output_format>

<style>
Maintain an elegant, precise, and design-forward tone. Focus on clean minimalism, data clarity, and high-quality aesthetic execution.
</style>

## Variables
- {VARIABLES_AND_TYPES} – The specific variables you want to plot and their formats (e.g., "Treatment group (categorical with 3 levels), Patient recovery time in days (continuous ratio), Age (continuous interval)").
- {RELATIONSHIP_TO_CONVEY} – The core insight or comparison you want the reader to make (e.g., "Showing that treatment group B has a significantly faster recovery time than group A and control, particularly among older patients").
- {TARGET_AUDIENCE} – The end reader (e.g., "Medical researchers reading a peer-reviewed journal paper," "C-suite executives looking for quick strategic metrics," or "the general public on a social media infographic").
- {INTENDED_MEDIUM} – The delivery format (e.g., static black-and-white print journal, interactive Tableau dashboard, full-screen projection PowerPoint presentation).

## Notes
- **Data-Ink Ratio**: The model is instructed to maximize Edward Tufte’s "data-ink ratio"—maximizing the ink dedicated to actual data variations while minimizing non-information-bearing design elements.
- **Uncertainty**: Always ensure the model explains *what* the error bars mean. In research, error bars are frequently displayed without specifying if they represent standard deviations, standard errors, or confidence intervals.
