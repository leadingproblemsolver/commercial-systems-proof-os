---
name: route-opportunity
description: Select exactly one highest-information external transition from live signals and current proof/assets.
allowed-tools: Read Grep Glob
---

# Route Opportunity

## Goal
Choose one transition. Do not brainstorm multiple plans.

## Ranking order
1. external consequence
2. information gain
3. technical ownership
4. warm access
5. compounding leverage

## Required decision object
```yaml
selected_transition:
target:
live_problem:
existing_proof:
why_now:
action:
receipt_sought:
maximum_block:
kill_condition:
rejected_alternatives:
  - candidate:
    reason_rejected:
```

## Rules
- Prefer real use/review/access over internal preparation.
- Prefer a live owner with visible urgency over a larger abstract market.
- Existing proof/assets beat new builds unless the new build is strictly required by the selected transition.
- If no candidate clears the evidence bar, output `NO_TRANSITION_SELECTED` and name the single missing input that would change the decision.
- Exactly one transition may be active.