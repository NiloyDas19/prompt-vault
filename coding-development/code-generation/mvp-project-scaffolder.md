---
title: "MVP Project Scaffolder"
category: Coding & Development
subcategory: Code Generation
tags: [scaffolding, MVP, project-structure, boilerplate, code-generation, full-stack]
model: any
---

## Purpose
Generate a complete, modular MVP project structure with folder layout, database schema, core API endpoints, and key boilerplate code for rapid prototyping.

## Prompt
You are an expert full-stack engineer specializing in rapid MVP development with {TECH_STACK}.

Scaffold a complete MVP project for the following application:

**Product name:** {PRODUCT_NAME}
**What it does:** {PRODUCT_DESCRIPTION}
**Core user actions (3–5 max):** {USER_ACTIONS} (e.g., register, log in, create a post, follow a user)
**Tech stack:** {TECH_STACK} (e.g., Node.js + Express + PostgreSQL + React, or Python + FastAPI + SQLite + Vue 3)

Generate the following:

1. **Project folder structure** — Complete directory tree with a one-line description for every folder and file
2. **Environment setup** — `.env.example` with all required environment variables and descriptions
3. **Database schema** — SQL DDL or ORM model definitions for all core entities
4. **API routes** — CRUD endpoints for each core entity (list, get by ID, create, update, delete) with request/response shapes
5. **Core boilerplate code** — Implement the 2 most complex API endpoints fully (not just stubs)
6. **Authentication** — Middleware or module for {AUTH_TYPE} (e.g., JWT, session-based) authentication
7. **Error handling** — A centralized error handler with consistent JSON error responses
8. **Quick-start guide** — Step-by-step commands to get from `git clone` to a running server in under 5 minutes

Keep code modular, add comments explaining non-obvious choices, and follow {TECH_STACK} conventions and best practices throughout.

## Variables
- {PRODUCT_NAME} – Name of the product
- {PRODUCT_DESCRIPTION} – 1–3 sentences describing what it does
- {USER_ACTIONS} – The 3–5 core things users do in the product
- {TECH_STACK} – Exact technologies (be specific about versions if you have preferences)
- {AUTH_TYPE} – Authentication mechanism (JWT, OAuth 2.0, magic link, session cookies)

## Notes
- For frontend scaffolding, add "Also generate the component structure and routing for the frontend using {FRONTEND_FRAMEWORK}."
- Ask for Docker Compose configuration to containerize the stack as a follow-up.
- This prompt works best for greenfield projects; for adding features to an existing project, use the "Feature Implementation Planner" prompt instead.
