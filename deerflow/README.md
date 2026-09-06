# DeerFlow Execution Control Plane

This directory is the bootstrap surface for running the existing proof / GTM system through one DeerFlow control plane.

## Architecture

`live signal -> ref-router -> one selected transition -> specialist worker -> deterministic authority -> proof judge -> human-controlled externalization -> settlement`

DeerFlow is the orchestration/cognition shell. Existing repositories remain deterministic authority boundaries.

## Existing authorities

- `leadingproblemsolver/market-intel-pipeline` — source-linked acquisition and normalization.
- `leadingproblemsolver/cgebs-execution-kernel` — one-active-thread lifecycle, proof-before-complete, immutable execution state.
- `leadingproblemsolver/direct-delivery-ops` — target/evidence/artifact/approval gate; must stop before sending.
- `leadingproblemsolver/chat-to-post-engine` — evidence-bounded public artifact compiler; never autonomously publishes.
- `leadingproblemsolver/commercial-systems-proof-os` — public proof-state registry and claim-boundary surface.

## Runtime workers

1. `ref-router` — choose exactly one highest-information external transition.
2. `market-role-scout` — acquire live source-linked role, founder, workflow and repo signals.
3. `engineering-proof` — reproduce/falsify a bounded foreign-code problem, patch only after reproduction.
4. `target-delivery` — convert verified proof into a recipient-specific intervention/application draft.
5. `proof-judge` — reject unsupported claims and emit one canonical proof object.
6. `warm-access` — route existing relationships toward workflow access, inspection, referral or concrete opportunity.
7. `externalizer` — transform only verified proof into audience-specific distribution; no autonomous publish.
8. `settler` — reconcile receipts, access changes, killed assumptions and next transition.

## Hard invariants

- One active deep execution transition at a time.
- No worker may claim delivery, publication, deployment, adoption, KPI impact or revenue without a recorded receipt.
- External sends/publishes/merges remain human-controlled until separately promoted.
- Subagents are used only for context isolation or genuinely independent parallel work.
- No new product/project may be created from a scout result unless the router selects it against existing proof/assets and an external consequence.
- Every substantial run terminates in one of: external receipt, verified capability gain, falsified hypothesis, explicit kill.

## Bootstrap order

1. Fork/clone DeerFlow 2.x and complete `make setup`.
2. Copy `config.fragment.yaml` into the DeerFlow config and resolve model/tool names.
3. Copy `skills/*` into DeerFlow's enabled custom-skill path.
4. Register the custom subagents from the config fragment.
5. Wire the three deterministic authorities first: market-intel, CGEBS, direct-delivery.
6. Wire Codex/Claude ACP for repository execution.
7. Run `acceptance/first-live-run.md` against one real GTM/Solutions/engineering opportunity.
8. Only after one successful loop, add schedules for scout and settlement.

## Definition of integrated

The integration is not complete when DeerFlow starts. It is complete when one live external signal is acquired, routed to one transition, executed through an existing authority, verified into a proof receipt, exposed to a real external reviewer/recipient, and settled with the resulting state change.
