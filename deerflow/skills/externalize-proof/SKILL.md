---
name: externalize-proof
description: Turn one verified proof object into the smallest audience-specific distribution package without publishing.
allowed-tools: Read Grep Glob Bash
---

# Externalize Proof

## Preconditions
- a verified proof object exists;
- the audience is concrete;
- the expected response is concrete.

If any precondition is absent, return `KILL_EXTERNALIZATION`.

## Output
```yaml
audience:
why_they_care:
proof_reference:
channel:
artifact:
cta:
expected_response:
release_state: AWAITING_HUMAN_APPROVAL
```

## Rules
- Use the source proof claims verbatim in substance; do not inflate them.
- Prefer a direct message, maintainer/engineer surface, targeted role owner, or relevant community over generic reach.
- Use `chat-to-post-engine` where available for evidence-boundary validation.
- Do not publish or imply publication.
- Kill channels with no identifiable audience or external consequence.
