---
title: "Chart & Graph Data Extractor"
category: Claude Skills
subcategory: Vision & Document Analysis
tags: [vision, charts, data-extraction, multimodal, analytics, Claude-specific]
model: claude (vision-capable models only)
---

## Purpose
Extract precise data, trends, and insights from charts, graphs, infographics, or dashboards shared as images.

## Prompt
Analyze the chart or graph I've attached. Extract all data as accurately as possible, then provide analytical insights.

<extraction_requirements>
- Chart type identified: (you determine this from the image)
- What I need from this chart: {EXTRACTION_GOAL} (e.g., all data points as a table, trend analysis, comparison between series, key outliers)
- How I plan to use this data: {USE_CASE} (e.g., recreate in Excel, write a report, compare against another dataset)
</extraction_requirements>

Please provide:
1. **Chart identification** — Type of chart, title, axis labels, legend items, units of measurement
2. **Data extraction** — Extract ALL visible data points into a clean markdown table with headers matching the chart's axes/legend
3. **Data quality notes** — Flag any values that are difficult to read precisely (provide a range instead)
4. **Key insights** — What does this data show? Identify:
   - Overall trend (increasing, decreasing, cyclical, volatile)
   - Peak and trough values with their labels
   - Notable outliers or anomalies
   - Significant patterns or inflection points
5. **Comparative analysis** — {COMPARISON_QUESTION}
6. **CSV-ready format** — Restate the extracted data in a copyable CSV format

[ATTACH CHART/GRAPH IMAGE HERE]

## Variables
- {EXTRACTION_GOAL} – What you need from the chart (data table, trend, comparison, etc.)
- {USE_CASE} – How you'll use the extracted data
- {COMPARISON_QUESTION} – A specific comparison question about the data, or "Identify the most interesting comparison within this chart"

## Notes
- 👁️ Requires vision-capable Claude model.
- Claude reads approximate values from charts — for precision-critical work, verify against the original data source.
- Works on bar charts, line graphs, pie/donut charts, scatter plots, heatmaps, and infographics.
- For dashboards with multiple charts, paste each chart separately for cleaner extraction.
