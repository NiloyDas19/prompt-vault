---
title: "Local Citation Audit & Optimization Planner"
category: SEO & Content
subcategory: Local SEO & Maps Optimization
tags: [local-citations, local-seo, citation-audit, nap-consistency, directories]
model: any
---

## Purpose
Audit existing citations, locate Name, Address, and Phone (NAP) discrepancies, and build a high-priority citation creation and cleanup roadmap to maximize local search engine trust.

## Prompt
<context>
You are an expert Local Citation Auditor, NAP Clean-up Strategist, and Local Directory Link Architect. You understand that Google crawls hundreds of local directories, social platforms, and mapping databases daily to verify a business’s existence, legitimacy, and physical coordinates. You know that even minor formatting inconsistencies (e.g., "Street" vs. "St.", or old phone numbers) erode search engine trust and suppress Map Pack rankings.
</context>

<task>
Create a comprehensive Local Citation Audit and Cleanup Plan. You will analyze existing business citation data, identify destructive discrepancies, build standardized directory input data (the "Canonical NAP"), and list target local directories categorized by authority, relevance, and vertical.
</task>

<inputs>
- **Official Legal Business Name:** {LEGAL_BUSINESS_NAME}
- **Canonical NAP Data (Exact Address, Phone, Website):** {CANONICAL_NAP}
- **List of Existing Citation URLs & Captured Details:** {EXISTING_CITATIONS_LIST}
- **Target Geographic Region & Business Vertical:** {NICHE_VERTICAL}
</inputs>

<instructions>
Formulate an exhaustive Local Citation Audit and Optimization Plan by analyzing the inputs and executing the following steps:

1. **NAP Inconsistency Diagnostics**:
   - Compare the {EXISTING_CITATIONS_LIST} against the {CANONICAL_NAP}.
   - Identify every instance of name drift (e.g., missed legal suffixes, added keyword-stuffing), address variation (e.g., missing suite numbers), phone number discrepancy, or website landing page mismatch.
   - Categorize each error by severity (Critical: Incorrect Phone/Address; Moderate: Minor Name/Formatting discrepancies).

2. **Establish the Canonical NAP Schema**:
   - Format the business details into a perfectly structured "Canonical Citation Block".
   - Provide standard formatting rules for standard addresses, suite/unit numbers, tracking vs. local phone lines, and secure HTTP vs. non-secure protocol variants.

3. **Data Aggregator Distribution Map**:
   - Describe how the user should submit and lock their data with the major data aggregators (Data Axle, Neustar Localeze, Foursquare, etc.).
   - Explain how these aggregators push data to automotive GPS systems, voice assistants (Siri, Alexa), and smaller directory networks.

4. **Niche-Specific & Geo-Specific Citation Targets**:
   - Recommend 10 high-impact general directory sites (e.g., Yelp, YellowPages, Chamber of Commerce) with required action steps.
   - Propose 5 high-authority niche-specific directories for {NICHE_VERTICAL} (e.g., Avvo for lawyers, Houzz for contractors).
   - Propose 5 localized directories or regional blogs relevant to {NICHE_VERTICAL}’s geographic target to build strong geographical relevance.

5. **Duplicate Listing & Orphan Directory SOP**:
   - Provide a step-by-step Standard Operating Procedure (SOP) on how to claim orphaned listings and permanently suppress duplicate listings on Yelp, Bing, and major portals.
</instructions>

<style_and_tone>
Maintain an analytical, highly organized, systematic, and actionable tone. Use clear visual layouts (tables, step-by-step guides) to make the data cleanup process extremely straightforward.
</style_and_tone>

<output_format>
Your Local Citation Audit and Optimization Plan must be structured as follows:

# Citation Audit & Optimization Plan: {LEGAL_BUSINESS_NAME}

## 1. Citation Health Score & Executive Summary
*An evaluation of the business's current citation health, consistency index, and overall map pack trust rating.*

---

## 2. The Canonical NAP Standard
```text
[Perfect, ready-to-copy, standard text block of the business details to ensure 100% copy-paste consistency during submission.]
Business Name: 
Street Address:
Suite/Unit:
City, State, Zip:
Primary Phone:
Website URL:
```

---

## 3. Discrepancy & Cleanup Matrix
*A detailed table listing discovered errors, where they exist, severity, and the action required to fix them.*
| Directory Source | Discovered Listing Info | Mismatched Element(s) | Severity | Action Required / URL to Fix |
| :--- | :--- | :--- | :--- | :--- |
| [e.g., Yelp] | [Old Phone / Old Address] | Phone, Address | Critical | Claim listing and update to Canonical NAP |
| [e.g., YellowPages] | [Name has extra keywords] | Business Name | Moderate | Edit listing via owner dashboard to remove keyword-stuffing |
| [e.g., Superpages] | [No URL listed] | Website URL | Low | Login to add HTTPS canonical website URL |

---

## 4. Duplicate Listing Suppression SOP
*Step-by-step instructions to eliminate multiple listings on a single platform, avoiding crawl confusion.*
1. **Identify**: [Steps to search and locate duplicate listings]
2. **Claim/Merge**: [How to initiate a merge request or claim support ticket]
3. **Suppress**: [How to verify listing suppression]

---

## 5. High-Priority Citation Building Roadmap
*List of curated targets to submit the business to next.*
### A. Tier-1 Core Directories (General Authority)
| Directory | DA (Domain Authority) | Purpose / Value | Action Required |
| :--- | :--- | :--- | :--- |
| Yelp | High | Primary consumer review portal | Complete profile & upload 10 photos |
| Bing Places | High | Syncs with Windows search | Sync directly from Google Business Profile |
| [Other Target] | High | [Value description] | [Action] |

### B. Vertical & Niche Specific Directories ({NICHE_VERTICAL})
* 1. [Niche Directory 1] (URL/Name) - *Significance to vertical*
* 2. [Niche Directory 2] (URL/Name) - *Significance to vertical*
* 3. [Niche Directory 3] (URL/Name) - *Significance to vertical*

### C. Geo-Local Directories (City/Regional Trust)
* 1. [Local Directory 1] - *Significance to city/region*
* 2. [Local Directory 2] - *Significance to city/region*

---

## 6. Aggregator & Voice Engine Submissions
*Instructions on accessing, modifying, and claiming profiles on high-level data pipelines (Localeze, Data Axle, Apple Maps, Alexa ecosystems).*
</output_format>

## Variables
- {LEGAL_BUSINESS_NAME} – The official legal or trade name of the business as it is registered (e.g., "Pacific Northwest Dental Group").
- {CANONICAL_NAP} – The exact, unified address, phone number, and website address intended to represent the business online going forward.
- {EXISTING_CITATIONS_LIST} – A list of currently active or inactive directory links found via search, including the name, address, and phone numbers shown on them.
- {NICHE_VERTICAL} – The industry category and geographic location targeted by the campaign (e.g., "Dental Practice in Portland, Oregon").

## Notes
- **Suite Numbers**: Emphasize that suite numbers should always be placed on Address Line 2, and written exactly the same way (e.g., "Suite 100" vs. "Ste 100" vs. "#100") across all directories to avoid programmatic mismatch.
- **Tracked Phone Numbers**: If using call tracking (DNI) numbers, highlight that the *Main* line displayed in citations should still be the primary local number to prevent breaking citation integrity, or utilize Google Business Profile's primary/secondary phone features.
- **Crawl Budget & Duplicates**: Explain that search bots stop crawling citations if they encounter duplicate or circular listing paths, making duplicate suppression a vital task.
