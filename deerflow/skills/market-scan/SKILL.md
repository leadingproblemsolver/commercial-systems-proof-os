---
name: market-scan
description: Acquire current source-linked market, hiring, workflow-pain, repo and operator signals for routing.
allowed-tools: WebSearch WebFetch Read Bash
---

# Market Scan

## Goal
Produce a bounded evidence register from live sources. Do not recommend strategy, create content, invent a product, or contact anyone.

## Input
- target role/problem class
- time window
- optional geography/company/repo constraints
- current proof primitives available

## Required output per candidate

```yaml
signal_id:
source_url:
observed_actor:
observed_problem_or_need:
observable_urgency:
observable_ownership:
role_company_repo:
proof_overlap:
possible_intervention:
external_receipt_available:
confidence: high|medium|low
unknowns: []
```

## Rules
1. Preserve original source URL.
2. Separate observation from inference.
3. Prefer signals with visible ownership, urgency, measurable consequence and reachable reviewer.
4. Reject generic trend/news items with no actionable owner.
5. Do not score a signal highly just because it matches an existing project.
6. Stop after enough candidates exist to make a routing decision; more volume is not success.

## Completion
Return the evidence register and nothing that implies execution occurred.