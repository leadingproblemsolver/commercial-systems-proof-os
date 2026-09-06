# Remaining Operator Checklist

Everything below requires local environment access, account credentials, repo creation/forking, or a human external action.

## A. Runtime bootstrap — required now

- [ ] Fork `bytedance/deer-flow` into the `leadingproblemsolver` account.
- [ ] Clone the fork locally.
- [ ] Run DeerFlow setup (`make setup`).
- [ ] Use Docker sandbox mode for execution.
- [ ] Run `make doctor` until clean.
- [ ] Choose/configure one primary model provider.
- [ ] Configure one live search provider.
- [ ] Enable one tracing provider (Langfuse or LangSmith).

## B. Bring this control pack into DeerFlow — required now

From `leadingproblemsolver/commercial-systems-proof-os/deerflow/`:

- [ ] Copy/merge `config.fragment.yaml` into DeerFlow's `config.yaml`.
- [ ] Copy each `skills/*` directory into DeerFlow's custom/enabled skills path.
- [ ] Confirm DeerFlow discovers:
  - `market-scan`
  - `route-opportunity`
  - `reproduce-issue`
  - `verify-proof`
  - `prepare-direct-delivery`
  - `route-warm-access`
  - `externalize-proof`
  - `settle-run`
- [ ] Confirm custom subagents appear:
  - `market-role-scout`
  - `engineering-proof`
  - `proof-judge`
  - `target-delivery`
  - `warm-access`
  - `externalizer`
  - `settler`

## C. Wire deterministic authorities — first integration wave

Create only the minimum adapters/wrappers needed for DeerFlow to invoke existing CLIs.

### `market-intel-pipeline`
- [ ] Clone locally.
- [ ] Verify fixture ingest/export works.
- [ ] Configure one live source credential (Apify or Reddit/PRAW).
- [ ] Expose a bounded command wrapper that accepts query/source/limit and returns normalized evidence JSON/JSONL.

### `cgebs-execution-kernel`
- [ ] Clone locally.
- [ ] Run the documented complete-block smoke path.
- [ ] Expose bounded wrapper commands for validate/start/complete/review/history.
- [ ] Keep CGEBS authoritative for one-active-thread and proof-before-complete semantics.

### `direct-delivery-ops`
- [ ] Clone locally.
- [ ] Run `init`, `validate`, and `manifest` on a fixture workspace.
- [ ] Expose bounded wrapper commands for workspace validation and approval-state inspection.
- [ ] Preserve the hard stop before send.

## D. Engineering execution — required for repo proof path

- [ ] Configure Codex ACP and/or Claude Code ACP in DeerFlow.
- [ ] Keep automatic permission approval OFF initially.
- [ ] Verify the ACP agent can inspect one disposable/test repository.
- [ ] Verify it cannot silently merge/publish without the human action you expect.

## E. First real acceptance run — do before any scaling

Use `acceptance/first-live-run.md`.

- [ ] Select one live GTM Engineer / Solutions Engineer / technical founder / foreign-code opportunity.
- [ ] Run acquisition.
- [ ] Route exactly one transition.
- [ ] Execute one bounded path.
- [ ] Verify proof.
- [ ] Human performs the external action.
- [ ] Record the exact external receipt/surface.
- [ ] Settle the run.

PASS only when the full path completes:

`live signal -> route -> bounded execution -> verified receipt -> real external exposure -> settlement`

## F. Only after first PASS

- [ ] Add morning scheduled `market-role-scout` run.
- [ ] Add evening scheduled `settler` run.
- [ ] Connect Slack/Telegram only if it reduces interaction friction.
- [ ] Add CRM/email/calendar MCP/API access only for a tested workflow.
- [ ] Promote any write/send action only after repeated manual success and explicit acceptance criteria.

## Explicitly defer

- [ ] No autonomous email/DM sending.
- [ ] No autonomous LinkedIn/X publishing.
- [ ] No autonomous PR merge.
- [ ] No 1,000+ signal/prospect scan.
- [ ] No new generic content/idea workers.
- [ ] No DeerFlow core fork modifications unless the first live loop proves a missing runtime capability.
- [ ] No second orchestration framework.

## Handoff back to ChatGPT

Once A + B are complete, return these exact receipts:

1. DeerFlow fork URL.
2. `make doctor` result.
3. names of the discovered custom skills.
4. names of the discovered custom subagents.
5. chosen model/search/tracing providers.
6. any exact setup error text.

With those receipts, the next step is to finalize the CLI/MCP adapter layer and run the first live acceptance transition.