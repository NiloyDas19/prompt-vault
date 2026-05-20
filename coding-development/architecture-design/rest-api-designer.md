---
title: "REST API Designer"
category: Coding & Development
subcategory: Architecture & Design
tags: [API, REST, OpenAPI, backend, architecture, design]
model: any
---

## Purpose
Design a complete, production-grade REST API specification including endpoints, schemas, status codes, and architectural rationale.

## Prompt
You are a Backend Architect with expertise in RESTful API design, OpenAPI 3.0, and {DOMAIN} systems.

Design a production-ready REST API for the following service:

**Service Description:** {SERVICE_DESCRIPTION}

**Key Entities / Resources:** {ENTITIES} (e.g., User, Order, Product)

**Requirements:**
- Expected scale: {SCALE} (e.g., 10k requests/day, 1M daily users)
- Authentication method: {AUTH_METHOD} (e.g., JWT Bearer, OAuth 2.0, API Key)
- Special constraints: {CONSTRAINTS} (e.g., must be stateless, GDPR compliance required, versioned API)

Please deliver:
1. **Resource hierarchy** — How resources relate and nest
2. **Endpoint table** — Method, path, description, request body, and success response for each endpoint
3. **Request/Response schemas** — JSON examples for the 3 most complex endpoints
4. **HTTP status codes** — Which codes each endpoint can return and under what conditions
5. **Error response format** — A consistent error envelope (include error code, message, and trace ID)
6. **Design decisions** — Explain 3 key architectural choices and their trade-offs
7. **OpenAPI 3.0 stub** — A YAML snippet for at least 2 endpoints

## Variables
- {SERVICE_DESCRIPTION} – What the API does (e.g., "manages user subscriptions for a SaaS billing platform")
- {ENTITIES} – Main data entities the API manages
- {DOMAIN} – Business domain (e.g., e-commerce, healthcare, fintech)
- {SCALE} – Expected traffic or data volume
- {AUTH_METHOD} – How callers will authenticate
- {CONSTRAINTS} – Any non-functional requirements or compliance needs

## Notes
- Ask for a Mermaid.js sequence diagram to visualize the authentication flow.
- Follow up with the "SQL Schema Designer" prompt to generate the backing database design.
- Add "Provide a versioning strategy (URL vs. header vs. query param)" if you need API versioning guidance.
