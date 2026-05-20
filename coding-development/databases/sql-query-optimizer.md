---
title: "SQL Query Optimizer"
category: Coding & Development
subcategory: Databases
tags: [SQL, performance, query-optimization, indexing, database, profiling]
model: any
---

## Purpose
Analyze a slow or inefficient SQL query, explain performance bottlenecks, and provide an optimized version with indexing recommendations.

## Prompt
You are a Senior Database Performance Engineer with deep expertise in query planning and {DB_ENGINE} internals.

Optimize the following query that is performing poorly:

**SQL Query:**
```sql
{SQL_QUERY}
```

**Context:**
- Database engine: {DB_ENGINE} (e.g., PostgreSQL 15, MySQL 8, SQL Server 2022)
- Relevant table sizes: {TABLE_SIZES} (e.g., "users: 2M rows, orders: 15M rows, order_items: 60M rows")
- Existing indexes: {EXISTING_INDEXES} (list any indexes already on these tables, or "Unknown")
- Current query execution time: {CURRENT_TIME} (e.g., ~4.2 seconds average)
- EXPLAIN / EXPLAIN ANALYZE output (if available):
```
{EXPLAIN_OUTPUT}
```

Please:
1. **Diagnose** — Identify the top performance problems (e.g., full table scan, Cartesian join, missing index, correlated subquery)
2. **Optimized Query** — Provide a rewritten version of the SQL that addresses the bottlenecks
3. **Index Recommendations** — List the exact `CREATE INDEX` statements that would help, with justification
4. **Complexity Analysis** — Estimate the before vs. after query plan improvement (e.g., "seq scan → index scan")
5. **Trade-offs** — Note any side effects (e.g., write slowdown from new indexes, result set differences)

## Variables
- {SQL_QUERY} – The slow query to optimize
- {DB_ENGINE} – Database engine and version
- {TABLE_SIZES} – Approximate row counts for each table in the query
- {EXISTING_INDEXES} – Current indexes, or "Unknown"
- {CURRENT_TIME} – Current average query execution time
- {EXPLAIN_OUTPUT} – Output of EXPLAIN / EXPLAIN ANALYZE, or "Not available"

## Notes
- Always run `EXPLAIN ANALYZE` on the optimized query to validate improvements before deploying.
- For PostgreSQL, ask the model to check for "sequential scan on large table" and "hash joins with bad row estimates."
- Pair with the "SQL Schema Designer" prompt if the schema itself may be contributing to poor performance.
