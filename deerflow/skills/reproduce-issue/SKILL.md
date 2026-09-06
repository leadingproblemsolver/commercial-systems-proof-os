---
name: reproduce-issue
description: Reproduce or falsify one bounded foreign-code problem before proposing a patch.
allowed-tools: Read Grep Glob Bash
---

# Reproduce Issue

## Goal
Establish whether one claimed problem exists under a reproducible execution path and isolate the smallest violated invariant.

## Required sequence
1. Record repository/ref and issue/problem statement.
2. Identify the narrowest relevant execution path.
3. Record environment/preconditions.
4. Run the smallest reproduction.
5. Capture command, exit status, observed output and expected behavior.
6. Classify: `REPRODUCED`, `FALSIFIED`, `BLOCKED_BY_ENVIRONMENT`, or `KILL`.
7. Only if reproduced, define the smallest patch boundary and verification test.

## Forbidden
- editing before reproduction unless a fixture-only change is strictly necessary to execute the documented path;
- speculative infrastructure setup;
- broad refactors;
- claiming a bug from static inspection alone;
- converting environment failure into product failure.

## Output
```yaml
repository:
ref:
problem:
execution_path:
preconditions:
reproduction_command:
observed:
expected:
classification:
invariant:
patch_boundary:
verification_command:
receipts: []
unknowns: []
```

## Stop
Stop immediately when the next step requires speculative infrastructure rather than evidence acquisition.