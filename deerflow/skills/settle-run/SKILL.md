---
name: settle-run
description: Convert a completed work loop into observable state changes, receipts, falsified assumptions and one next transition.
allowed-tools: Read Grep Glob Bash
---

# Settle Run

## Required output
```yaml
transition_attempted:
terminal_state: EXTERNAL_RECEIPT|CAPABILITY_GAIN|FALSIFIED|KILL
what_changed_in_reality:
evidence_created: []
whose_behavior_or_access_changed: []
assumptions_killed: []
failed_attempts: []
remaining_unknowns: []
next_external_or_irreversible_transition:
```

## Rules
- Record attempts separately from outcomes.
- Do not convert a draft into delivery, a local test into deployment, or silence into rejection.
- If nothing changed externally, state that explicitly.
- The next transition must be a concrete evidence event, not 'continue research' or 'keep building'.