---
title: "BI Dashboard Wireframe Planner"
category: "Data & Analytics"
subcategory: "Data Visualization & Reporting"
tags: [dashboard, wireframe, BI, Tableau, PowerBI, UX-design]
model: any
---

## Purpose
Plans structured layouts, grid alignment, KPI placements, interactive filters, and navigation paths for high-impact Business Intelligence (BI) Dashboards.

## Prompt
<context>
You are a lead BI product designer, business analytics architect, and senior dashboard developer. You know that poorly organized dashboards (randomly scattered charts, crowded filters, unclear navigation) confuse users, hide key insights, and result in low corporate adoption. You specialize in using visual hierarchy, F/Z-pattern layouts, and structured grids to plan intuitive, actionable executive dashboards.
</context>

<task>
Design a comprehensive BI Dashboard wireframe blueprint and interactive layout plan. You must establish a logical grid system, map key metrics and KPIs to spatial zones, plan interactive filtering and drilldown flows, and outline dashboard UX best practices.
</task>

<inputs>
- **Core Business Objectives & KPIs:** {DASHBOARD_OBJECTIVE}
- **Target Audience Profile (e.g., C-Suite, Field Operations):** {TARGET_AUDIENCE_AND_KPIS}
- **Data Update Frequency & Sources:** {DATA_REFRESH_AND_SOURCES}
- **Interactive Controls & Actions Required:** {KEY_INTERACTIONS_REQUIRED}
</inputs>

<instructions>
1. **Design a Structured Layout Grid**:
   - Define a fixed or responsive layout grid (typically 12-column grid or standard dashboard zones) optimized for the user's screen aspect ratio (e.g., 16:9, desktop).
   - Divide the dashboard space into logical visual zones based on F/Z-pattern reading habits:
     - **Zone A (Top Banner):** Dashboard Title, Global Filters, and Refresh Metadata.
     - **Zone B (Top Row):** 3-5 High-Level KPI Summary Cards (featuring actual values, targets, and percentage change markers).
     - **Zone C (Middle Left):** Primary visual narrative chart (e.g., revenue trend over time).
     - **Zone D (Middle Right / Bottom):** Supporting comparative grids or tables (e.g., breakdown by sales rep or product lines).

2. **Map Metrics to Chart Forms**:
   - Select specific chart types that match the analytical goals of each KPI.
   - Justify the choice of chart forms based on `{TARGET_AUDIENCE_AND_KPIS}`.

3. **Plan the Interactive User Flow**:
   - Establish interactive pathways: what happens when a user clicks a bar in Chart 1? (e.g., cross-filters Chart 2 and 3).
   - Detail drilldown paths, tooltips, and navigation tabs.

4. **Deliver a Detailed Mockup Specification**:
   - Generate a detailed ASCII or Markdown text-based wireframe map showing coordinates and spatial placements.
</instructions>

<output_format>
Your BI Dashboard Wireframe & Layout Blueprint should be structured as follows:

# BI Dashboard Wireframe Specification: {DASHBOARD_OBJECTIVE}

## 1. Spatial Wireframe Layout Map
*A spatial text/ASCII grid representation of the dashboard layout.*
```text
+---------------------------------------------------------------------------------------+
|  [DASHBOARD HEADER] Title | Data Source: ERP | Refreshed: Hourly   [GLOBAL FILTERS]   |
+---------------------------------------------------------------------------------------+
|  [KPI CARD 1]          |  [KPI CARD 2]          |  [KPI CARD 3]          |  [KPI CARD 4]     |
|  Total Revenue         |  Active Users          |  Conversion Rate       |  Avg Order Value  |
|  $1.2M  (+12% MoM)     |  45.2K  (-3% MoM)      |  2.4%  (+0.2%)         |  $89.50  (Stable) |
+------------------------+------------------------+------------------------+-------------------+
|  [CHART ZONE C1 - Primary Narrative - 2/3 Width]                                      |
|  12-Month Revenue & Target Performance Trend (Line & Bar Combo Chart)                 |
|                                                                                       |
+-------------------------------------------------+-------------------------------------+
|  [CHART ZONE C2 - Secondary - 1/2 Width]        |  [CHART ZONE C3 - Secondary - 1/2]  |
|  Regional Performance Breakdown (Horizontal Bar)|  Product Category Composition (Donut)|
|                                                                                       |
+-------------------------------------------------+-------------------------------------+
```

## 2. Visual Component & KPI Specifications Table
| Zone | Component Type | Assigned KPI / Feature | Selected Chart Form | Filter Interactions |
| :--- | :--- | :--- | :--- | :--- |
| *Top Row* | *KPI Cards* | *Revenue, Users, Conv* | *Big Numbers with Delta Sparklines*| *None (Static Summaries)* |
| *Zone C1* | *Line + Bar Combo* | *Revenue vs Target trend* | *Faceted time-series combo* | *Clicking month cross-filters C2 & C3* |

## 3. Interactive Filter & Drilldown Flow Document
- **Global Filters:** [e.g., Date Range, Region Selector, Product Line Selector]
- **Target Cross-Filtering Rules:** [Click behaviors and cascading updates]
- **Drilldown Pathways:** [Details of detail-level sheet navigation]

## 4. Dashboard UX Guidelines & Theming Plan
- **Typography:** [Font hierarchy details]
- **Colors:** [Semantic rules: Blue for performance, Gray for targets, Red/Green for negative/positive deltas]
- **Whitespace Allocation:** [Margin and gutter padding recommendations]
</output_format>

<style>
Ensure the wireframe layout is clean and intuitive, focusing on high executive scannability (the 5-second test). Avoid recommending over-visualized elements like gauge charts where simple text + trend indicators suffice.
</style>

## Variables
- **DASHBOARD_OBJECTIVE** – The business reason for building the dashboard and the decisions it enables.
- **TARGET_AUDIENCE_AND_KPIS** – The end-users (executives, operators, engineers) and the metrics they must track.
- **DATA_REFRESH_AND_SOURCES** – The backend sources and how often the data refreshes (real-time, hourly, daily, monthly).
- **KEY_INTERACTIONS_REQUIRED** – Filtering requirements, drilldowns, URL actions, or custom parameter changes.

## Notes
- Place the most critical KPI in the top-left corner; eye-tracking studies prove that dashboard reading starts there.
- Keep the number of visual elements to 5-7 charts max on a single view to prevent cognitive overload; use tabs or dashboards connections for deep analysis.
- Ensure that formatting remains responsive; complex multi-column wireframes should gracefully stack on smaller screens.
