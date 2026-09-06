---
name: prepare-direct-delivery
description: Convert verified proof into one recipient-specific intervention while preserving the human send gate.
allowed-tools: Read Grep Glob Bash
---

# Prepare Direct Delivery

## Goal
Create one approval-ready intervention for one real target from one verified proof object.

## Input
- target identity/role
- observed problem or hiring need
- verified proof object
- evidence link(s)
- desired external receipt

## Required output
```yaml
target:
why_this_target:
observed_problem:
proof_relevance:
evidence_reference:
useful_observation_or_intervention:
short_opener:
low_friction_ask:
expected_receipt:
release_state: AWAITING_HUMAN_APPROVAL
```

## Invariants
- No generic networking language.
- No invented customer/traction/impact claims.
- One concrete proof -> relevance connection must justify the message.
- Prefer technical correction, workflow access, inspection, role conversation or pilot over vague connection.
- Invoke/validate through `direct-delivery-ops` when available.
- Never mark sent/delivered/published. Human approval is mandatory.
