---
title: "Corporate Cybersecurity Incident Policy"
category: Business & Strategy
subcategory: Risk Management & Crisis Strategy
tags: [cybersecurity, incident-response, tech-policy, data-security, risk-management]
model: any
---

## Purpose
Draft a highly structured, operational corporate Cybersecurity Incident Response Policy and Playbook to detect, isolate, eradicate, and recover from system breaches, data leaks, or ransomware attacks.

## Prompt
You are an expert Chief Information Security Officer (CISO), cybersecurity legal advisor, and crisis response consultant. Your goal is to draft a comprehensive Corporate Cybersecurity Incident Response Policy and execution guide based on the company's infrastructure and regulatory context.

<context>
The company needs a clear, operational, and legally compliant policy to handle security incidents. The document must define roles, establish classification protocols, and outline exact mitigation steps to prevent data loss and legal penalties.
- **IT Infrastructure & Technical Stack Overview**: {ORGANIZATIONAL_IT_INFRASTRUCTURE}
- **Data Privacy & Regulatory Obligations (e.g., HIPAA, GDPR, SEC)**: {REGULATORY_DATA_OBLIGATIONS}
- **Incident Response Team (IRT) Roles & Resources**: {INCIDENT_RESPONSE_TEAM_ROLES}
- **Security Incident Severity Scale Definitions**: {SEVERITY_LEVEL_DEFINITIONS}
</context>

<incident_response_phases>
The response playbook must follow the industry-standard **NIST Incident Response Lifecycle**:
1. **Preparation**: Maintaining security controls, logs, backups, and training IRT members.
2. **Detection & Analysis**: Monitoring indicators, validating active alerts, and classifying severity levels.
3. **Containment, Eradication, & Recovery**:
   - *Short-term containment* (e.g., isolating network subnets).
   - *Long-term containment* (e.g., patching systems, resetting credentials).
   - *Eradication* (e.g., removing malware, deleting unauthorized user accounts).
   - *Recovery* (e.g., restoring systems from clean backups, verifying performance).
4. **Post-Incident Activity**: Conducting a blameless post-mortem, documenting lessons learned, and updating policies.
</incident_response_phases>

<instructions>
1. **Define Security Breach Levels**: Using `{SEVERITY_LEVEL_DEFINITIONS}`, build a clear, structured classification matrix that defines Level 1 (Low/Informational) to Level 4 (Critical/Crisis) incidents, specifying technical and business triggers.
2. **Establish the Incident Response Team (IRT)**: Map the exact roles, contact protocols, and decision-making authority for members (CISO, Security Engineer, Legal Counsel, PR Lead, COO) as detailed in `{INCIDENT_RESPONSE_TEAM_ROLES}`.
3. **Detail Containment & Recovery Workflows**: Draft a step-by-step playbook for the technical team to follow once a breach (such as a ransomware attack or data exfiltration) is detected within the `{ORGANIZATIONAL_IT_INFRASTRUCTURE}`.
4. **Construct the Legal & Regulatory Notification Guide**: Outline the mandatory reporting windows, formatting guidelines, and communication protocols based on `{REGULATORY_DATA_OBLIGATIONS}` (e.g., GDPR 72-hour notice, SEC disclosure requirements).
5. **Formulate Post-Mortem Templates**: Design a structured "lessons learned" feedback template to run at the conclusion of an incident to prevent repeat occurrences.
</instructions>

<output_format>
Your Cybersecurity Incident Response Policy must be structured as follows:
1. **Policy Purpose & Scope**: Strategic statement of commitment, operational scope, and user responsibility.
2. **The Incident Classification Matrix**: A table mapping severity levels, description of impact, and response times.
3. **Incident Response Team (IRT) Directory & RACI Matrix**: Clear operational guidelines showing who drives, who supports, and who signs off during an incident.
4. **Phase-by-Phase Response Playbook (NIST Aligned)**:
   - Detection & Reporting procedures.
   - Isolation & Containment strategies (detailed technical steps).
   - System Eradication & Backup Recovery protocols.
5. **Regulatory Disclosure & Notification Protocols**: Precise timelines and draft language placeholders for communicating with data protection authorities, clients, and partners.
6. **Blameless Post-Mortem Form**: Structured sections for root-cause analysis, timeline logs, and operational action items.
</output_format>

## Variables
- {ORGANIZATIONAL_IT_INFRASTRUCTURE} – Technical details of the company's network (e.g., AWS Cloud-native, hybrid cloud, on-premises servers), core software tools, and customer databases.
- {REGULATORY_DATA_OBLIGATIONS} – The regulations governing data breaches for the industry (e.g., GDPR, HIPAA, SOC 2, PCI-DSS, SEC, CCPA).
- {INCIDENT_RESPONSE_TEAM_ROLES} – The directory of roles, internal/external contact rules, and escalation paths (such as when to notify insurance, law enforcement, or external forensic investigators).
- {SEVERITY_LEVEL_DEFINITIONS} – The framework for rating incidents, from minor phishing emails to full-scale databases compromises or ransom threats.

## Notes
- Advise users that regular "tabletop exercises" (simulating a live cybersecurity breach with executive teams) is the single best way to ensure the policy actually works under pressure.
- Remind IT teams that "backups are useless if they cannot be restored"—offline or air-gapped backup systems must be tested at least quarterly.
- Emphasize maintaining strict chains of evidence during containment to ensure legal and insurance validity if forensic investigation is required later.
