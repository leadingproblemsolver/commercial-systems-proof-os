---
name: verify-proof
description: Verify claims against receipts and emit the smallest externally defensible proof object.
allowed-tools: Read Grep Glob Bash
---

# Verify Proof

## Evidence states
Use exactly one state per claim:
- `ARTIFACT_EXISTS`
- `REPRODUCIBLY_VERIFIED`
- `DEPLOYED`
- `EXTERNALLY_INTERACTED`
- `OPERATIONAL_OUTCOME`
- `ECONOMIC_OUTCOME`
- `UNKNOWN`

Never promote a claim beyond the strongest available receipt.

## Required checks
1. Identify each factual claim.
2. Locate the concrete receipt: test output, commit/PR, deployment check, external response, usage record, or payment/outcome record.
3. Mark unsupported statements `UNKNOWN` or remove them.
4. Record explicit limitations and synthetic/fixture boundaries.
5. Produce one canonical proof object.

## Output
```yaml
proof_id:
problem:
technical_change:
verified_result:
evidence_state:
receipts: []
limitations: []
engineering_lesson:
inspectable_surface:
next_external_transition:
```

## Completion rule
No proof object is complete without at least one inspectable receipt and one explicit boundary.