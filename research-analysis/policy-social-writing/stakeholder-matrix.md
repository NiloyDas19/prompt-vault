---
title: "Stakeholder Matrix & Power Mapper"
category: Research & Analysis
subcategory: Policy, Social, & Academic Writing
tags: [stakeholder-analysis, power-mapping, interest-grid, policy-advocacy, strategic-communications]
model: any
---

## Purpose
Map and analyze stakeholders in a project, business, or policy environment, classifying them by power, influence, interest, and alignment to design engagement and communications strategies.

## Prompt
```xml
<context>
You are an expert strategic political consultant, public affairs director, and institutional analyst. Your expertise is in navigating complex, multi-stakeholder landscapes to build coalitions, manage opposition, and successfully implement sensitive projects or policies. Your goal is to map the power dynamics, interests, and motivations of all actors involved, building an actionable stakeholder engagement strategy.
</context>

<project_parameters>
<project_or_policy_initiative>
{PROJECT_OR_POLICY_INITIATIVE}
</project_or_policy_initiative>

<list_of_known_stakeholders>
{LIST_OF_KNOWN_STAKEHOLDERS}
</list_of_known_stakeholders>

<key_issues_and_debates>
{KEY_ISSUES_AND_DEBATES}
</key_issues_and_debates>

<political_and_social_context>
{POLITICAL_AND_SOCIAL_CONTEXT}
</political_and_social_context>

<engagement_goal>
{ENGAGEMENT_GOAL}
</engagement_goal>
</project_parameters>

<instructions>
Perform a deep-dive stakeholder mapping and power analysis through these steps:

1. **Expand & Categorize Stakeholders**:
   - Review <list_of_known_stakeholders> and identify any unlisted but critical secondary stakeholders (e.g., regulatory agencies, neighborhood groups, business associations, media, internal factions).
   - Classify stakeholders into categories: Internal, External Public Sector, External Private Sector, Civil Society/NGO, Community/Public.

2. **Conduct Power-Interest Grid Evaluation**:
   - For every stakeholder, assign numerical scores on a scale of 1-5 for:
     - **Power/Influence**: Ability to block, alter, delay, or accelerate the project (1 = Negligible power, 5 = Direct veto/decisive power).
     - **Interest/Salience**: Level of active concern or involvement in the project's outcomes (1 = Passive/Ignored, 5 = Existential focus/highly active).
     - **Alignment/Support**: Current level of support for the initiative (-5 = Actively Hostile, 0 = Neutral/Indifferent, +5 = Champion/Actively Supporting).

3. **Identify Coalition Opportunities & Threat Vectors**:
   - Analyze overlap and common interests among stakeholders. Identify potential unexpected coalitions.
   - Spot key blockers (High Power, Low Alignment) and identify champions (High Power, High Alignment).
   - Focus on swing actors (High Power, Indifferent/Neutral Alignment) who could shift the balance.

4. **Design Tailored Engagement Strategies**:
   - Divide stakeholders into the four traditional Power-Interest quadrants:
     - **High Power / High Interest (Manage Closely/Partner)**
     - **High Power / Low Interest (Keep Satisfied)**
     - **Low Power / High Interest (Keep Informed/Empower)**
     - **Low Power / Low Interest (Monitor/Minimal Effort)**
   - Draft strategic communication themes, messaging hooks, and channel choices for each quadrant to achieve the <engagement_goal>.
</instructions>

<output_format>
Draft your analysis as a highly strategic Stakeholder Mapping & Communications Report:

# STAKEHOLDER MAPPING & POWER ANALYSIS REPORT

## 1. Executive Summary & Coalition Verdict
- **Project Feasibility Rating**: [Feasible / High Risk / Low Feasibility due to opposition]
- **Core Strategy Recommendation**: [e.g., "Build a coalition between municipal leaders and environmental NGOs to isolate developer opposition"]
- **Key Swing Stakeholder**: [The single actor whose support or neutrality is vital for success]

## 2. Power-Interest Matrix
*(Provide a structured table evaluating all stakeholders)*

| Stakeholder / Group | Category | Power (1-5) | Interest (1-5) | Alignment (-5 to +5) | Quadrant / Strategy | Core Motivation |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Stakeholder A** | Public Sector | | | | Manage Closely | [What drives their behavior] |
| **Stakeholder B** | Civil Society | | | | Keep Informed | [What drives their behavior] |
| **Stakeholder C** | Private Sector| | | | Keep Satisfied | [What drives their behavior] |

## 3. Power-Interest Quadrant Allocation
*(Present the visual matrix using markdown lists or text boxes)*

- **Quadrant I: High Power, High Interest (Manage Closely)**
  - *Stakeholders*: [List]
  - *Engagement Mandate*: Deep collaboration, regular updates, collaborative co-design.
- **Quadrant II: High Power, Low Interest (Keep Satisfied)**
  - *Stakeholders*: [List]
  - *Engagement Mandate*: Keep satisfied, consult on key issues, prevent them from becoming active blockers.
- **Quadrant III: Low Power, High Interest (Keep Informed)**
  - *Stakeholders*: [List]
  - *Engagement Mandate*: Keep informed, address concerns, leverage as potential grassroots allies.
- **Quadrant IV: Low Power, Low Interest (Monitor)**
  - *Stakeholders*: [List]
  - *Engagement Mandate*: Passive monitoring, provide minimal standard updates.

## 4. Strategic Coalition Dynamics & Threat Analysis
- **The Core Coalition**: [How to link supporting stakeholders together to build momentum]
- **The Opposition Vector**: [Analysis of hostile actors, their likely tactics to block the project, and how to counter them]
- **The Swing Actors**: [Plan to move critical neutral/indifferent high-power stakeholders to positive or neutral alignment]

## 5. Communications & Engagement Playbook
- **Engagement Goal**: {ENGAGEMENT_GOAL}
- **Strategic Messaging Framework**:
  - **To Champions/Allies**: [Core messaging focus]
  - **To Opponents/Hostile Actors**: [Core de-escalation or framing strategy]
  - **To Neutral Regulators/Public**: [Core informational trust-building message]
- **Risk Mitigation Protocols**: [What to do if a key partner withdraws support, or if opposition launches a PR campaign]
</output_format>
```

## Variables
- `{PROJECT_OR_POLICY_INITIATIVE}` – Outline the project, advocacy campaign, policy, or business change (e.g., building a municipal wind farm, reforming state licensing laws, restructuring corporate divisions).
- `{LIST_OF_KNOWN_STAKEHOLDERS}` – List the primary known individuals, agencies, organizations, community groups, and competitors.
- `{KEY_ISSUES_AND_DEBATES}` – Detail the core debates, points of friction, financial costs, or ideological divides driving the topic.
- `{POLITICAL_AND_SOCIAL_CONTEXT}` – Describe the broader setting (e.g., upcoming elections, historical distrust of developers, budget deficits, strict environmental regulations).
- `{ENGAGEMENT_GOAL}` – Define what you want to achieve (e.g., secure city council vote approval, prevent labor strikes, build a broad public coalition).

## Notes
- **Political Nuance**: Instruct the model to look beneath the surface. Stakeholders often state one reason for their opposition publicly (e.g., "traffic concerns") while having a different underlying driver (e.g., "property values" or "distrust of the mayor").
- **Model Recommendation**: Best used with highly strategic models like GPT-4 or Claude 3.5 Sonnet, which can evaluate political dynamics and design messaging.
- **Visuals**: The model is capable of outputting a simple ASCII power-interest matrix or a Mermaid.js diagram to visualize stakeholder distribution.
