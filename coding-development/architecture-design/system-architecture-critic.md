---
title: "System Architecture Critic"
category: Coding & Development
subcategory: Architecture & Design
tags: [architecture, system-design, scalability, ADR, trade-offs]
model: any
---

## Purpose
Critique a proposed system architecture for bottlenecks and failure modes, and generate Architectural Decision Records (ADRs).

## Prompt
You are a Principal Software Architect with experience designing large-scale distributed systems.

I need a critical review of the following architecture proposal:

**System Name:** {SYSTEM_NAME}
**Purpose:** {SYSTEM_PURPOSE}
**Current Architecture:**
{ARCHITECTURE_DESCRIPTION}

**Scale targets:**
- Concurrent users: {CONCURRENT_USERS}
- Data volume: {DATA_VOLUME}
- Uptime requirement: {UPTIME_SLA} (e.g., 99.9%)

Please:
1. **Identify failure modes** — For each component, what breaks first under load or failure?
2. **Traffic spike analysis** — What happens to the system at 10x current load? Which component collapses first?
3. **Single points of failure (SPOFs)** — List all SPOFs and a mitigation for each.
4. **Security surface** — What are the top 3 security risks in this architecture?
5. **Top 3 recommended changes** — Ordered by impact-to-effort ratio.
6. **ADR stubs** — Write an Architectural Decision Record (ADR) for each of your top 3 recommendations using the MADR format (Motivation, Alternatives, Decision, Rationale, Consequences).

## Variables
- {SYSTEM_NAME} – Name or codename of the system
- {SYSTEM_PURPOSE} – What the system does and who uses it
- {ARCHITECTURE_DESCRIPTION} – Describe the architecture (components, data flows, infra). Paste a diagram description, text list, or Mermaid code.
- {CONCURRENT_USERS} – Current and target concurrent user count
- {DATA_VOLUME} – Current data size and growth rate
- {UPTIME_SLA} – Required availability (e.g., 99.9% = ~8.7 hours downtime/year)

## Notes
- Paste a Mermaid.js diagram for richer analysis ("here is the architecture as a Mermaid diagram: ...").
- Ask the model to prioritize cloud-native mitigations if you're on AWS/GCP/Azure.
- Useful before major refactors, migrations, or funding reviews where architectural rigor matters.
