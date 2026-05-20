---
title: "Log Analyzer & Failure Interpreter"
category: Coding & Development
subcategory: Debugging
tags: [debugging, logs, monitoring, incident-response]
model: any
---

## Purpose
Parse and interpret raw application or server logs to identify the failure point and suggest next debugging steps.

## Prompt
You are an expert Site Reliability Engineer skilled at reading application logs and diagnosing failures.

I am troubleshooting an issue in a {SYSTEM_TYPE} system. Below are the relevant log entries:

```
{LOG_ENTRIES}
```

**Context:**
- System / Service: {SYSTEM_NAME}
- Stack: {TECH_STACK}
- Approximate time the issue started: {INCIDENT_TIME}
- Expected behavior: {EXPECTED_BEHAVIOR}

Please:
1. Identify the first sign of failure in the logs (the "canary" event).
2. Explain the chain of events that led to the failure.
3. Pinpoint the most likely root cause.
4. Provide a prioritized list of remediation steps.
5. Suggest what additional logging or metrics I should add to detect this class of issue earlier.

## Variables
- {SYSTEM_TYPE} – e.g., web server, microservice, batch job, queue worker
- {LOG_ENTRIES} – Paste the relevant log lines (redact any sensitive data first)
- {SYSTEM_NAME} – Name or description of the service
- {TECH_STACK} – e.g., Node.js + PostgreSQL + Redis on AWS ECS
- {INCIDENT_TIME} – Approximate timestamp or time window
- {EXPECTED_BEHAVIOR} – What the system should have done instead

## Notes
- Redact passwords, API keys, and PII before pasting logs.
- Include surrounding "normal" log lines so the model can identify anomalies by contrast.
- For very long logs, paste only the 50–100 lines around the suspected failure window.
