---
title: "SQL Schema Designer"
category: Coding & Development
subcategory: Databases
tags: [database, SQL, schema-design, normalization, ERD, PostgreSQL, MySQL]
model: any
---

## Purpose
Design a normalized, production-ready relational database schema with indexes, constraints, and an ER diagram for a given domain.

## Prompt
You are a Senior Database Architect specializing in relational databases ({DB_ENGINE}).

Design a production-ready database schema for the following system:

**System:** {SYSTEM_DESCRIPTION}

**Core entities and relationships:**
{ENTITIES_AND_RELATIONSHIPS}

**Requirements:**
- Normalization target: {NORMALIZATION_LEVEL} (e.g., 3NF, BCNF, or "prioritize read performance over strict normalization")
- Expected query patterns: {QUERY_PATTERNS} (e.g., "heavy reads on orders by user_id and date")
- Special requirements: {SPECIAL_REQUIREMENTS} (e.g., soft deletes, multi-tenancy, audit trail, GDPR right-to-erasure)

Please provide:
1. **DDL SQL** — `CREATE TABLE` statements with all columns, data types, constraints (NOT NULL, UNIQUE, CHECK), primary keys, and foreign keys
2. **Indexes** — Recommended indexes based on the stated query patterns, with justification for each
3. **Relationships summary** — A table listing each relationship (entity A → entity B, cardinality, via which FK)
4. **Mermaid ER Diagram** — A `mermaid erDiagram` code block visualizing the schema
5. **Design notes** — Explain 2–3 key decisions (e.g., why you chose a junction table, why you denormalized a field)

## Variables
- {DB_ENGINE} – Target database (e.g., PostgreSQL, MySQL, SQLite, SQL Server)
- {SYSTEM_DESCRIPTION} – What the system does (e.g., "an e-commerce platform with products, users, and orders")
- {ENTITIES_AND_RELATIONSHIPS} – List entities and describe how they relate (e.g., "A User can place many Orders. Each Order has many OrderItems. Each OrderItem references one Product.")
- {NORMALIZATION_LEVEL} – Desired normal form or performance preference
- {QUERY_PATTERNS} – Most common read/write access patterns
- {SPECIAL_REQUIREMENTS} – Any compliance, audit, or multi-tenancy needs, or "None"

## Notes
- Ask for migration scripts (Flyway/Liquibase format) as a follow-up.
- Combine with the "SQL Query Optimizer" prompt to tune queries once the schema is set.
- For NoSQL equivalents, modify the prompt to ask for a MongoDB document model or DynamoDB access patterns.
