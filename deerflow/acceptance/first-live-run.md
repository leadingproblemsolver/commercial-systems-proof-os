# First Live Run Acceptance

Use this before scheduling or expanding the worker catalog.

## Input
Choose exactly one live GTM Engineer, Solutions Engineer, technical founder/operator, or foreign-code opportunity with a reachable external reviewer.

## Acceptance path

### 1. Acquire
Run `market-role-scout` with `/market-scan`.

PASS only if at least one candidate has:
- original source URL;
- identifiable owner/reviewer;
- observable need/problem;
- plausible overlap with existing proof/capabilities.

### 2. Route
Run the lead agent with `/route-opportunity` against the candidate register and current proof inventory.

PASS only if exactly one transition is selected with:
- target;
- live problem;
- existing proof;
- action;
- receipt sought;
- kill condition.

### 3. Execute
Choose one path:
- engineering -> `engineering-proof`;
- recipient/application -> `target-delivery`;
- existing relationship -> `warm-access`.

PASS only if execution terminates in a bounded state, not an open-ended plan.

### 4. Verify
Run `proof-judge` with `/verify-proof`.

PASS only if:
- every public/external claim maps to a receipt;
- evidence state is explicit;
- limitations are explicit;
- inspectable surface is named.

### 5. Release gate
For direct recipient work, validate through `direct-delivery-ops` when wired.
For public distribution, validate through `chat-to-post-engine` when wired.

PASS only if release state remains `AWAITING_HUMAN_APPROVAL` before a human action.

### 6. External consequence
Human performs the selected external action: submit, send, comment, open PR, request inspection, publish, or otherwise expose the proof to the selected real reviewer.

Record the exact external surface/receipt. Do not infer response.

### 7. Settle
Run `/settle-run`.

PASS only if the run records:
- what changed in reality;
- evidence created;
- behavior/access changes if any;
- assumptions killed;
- next external/irreversible transition.

## Integration acceptance

The DeerFlow layer is accepted only when one full run completes:

`live signal -> route -> bounded execution -> verified receipt -> real external exposure -> settlement`

## Expansion rule
Do not add schedules, more workers, CRM writes, autonomous sends/publishing, or high-volume scanning until this acceptance run passes once.