---
title: "Performance Optimizer"
category: Coding & Development
subcategory: Refactoring
tags: [performance, optimization, Big-O, profiling, efficiency]
model: any
---

## Purpose
Analyze code for performance bottlenecks, provide an optimized version, and explain the complexity trade-offs.

## Prompt
You are a performance engineering specialist with deep knowledge of {LANGUAGE} runtime internals and algorithmic complexity.

I need to optimize the following code for {OPTIMIZATION_GOAL}.

**Current Code:**
```{LANGUAGE}
{CODE}
```

**Performance Context:**
- Current estimated scale: {SCALE} (e.g., 10k records, 500 concurrent users, runs every 5 minutes)
- Known bottleneck (if any): {KNOWN_BOTTLENECK}
- Available infrastructure: {INFRASTRUCTURE} (e.g., single server, Redis available, read replicas allowed)

Please:
1. Profile the code visually — annotate each section with its time and space complexity (Big-O notation).
2. Identify the top 3 most impactful performance bottlenecks.
3. Provide an optimized version of the code.
4. For each optimization, explain:
   - What changed
   - Why it's faster (algorithmic gain, cache hit, reduced I/O, etc.)
   - The new complexity after the change
5. Highlight any trade-offs (e.g., memory vs. speed, code clarity vs. performance).

## Variables
- {LANGUAGE} – Programming language (e.g., Python, Go, Java, JavaScript)
- {CODE} – The code to optimize
- {OPTIMIZATION_GOAL} – What to optimize for: speed, memory, I/O throughput, latency, etc.
- {SCALE} – Current or expected data size / request volume
- {KNOWN_BOTTLENECK} – Any bottleneck you've already identified, or "Unknown"
- {INFRASTRUCTURE} – What tools/hardware/services are available to leverage

## Notes
- For database-heavy code, focus on the "N+1 query" prompt in the Database subcategory instead.
- Pair this with a profiler (cProfile, perf, JProfiler) to validate the model's predictions.
- Ask for benchmarking code if you want to measure before/after improvements programmatically.
