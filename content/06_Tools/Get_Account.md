---
id: "ryx.tool.get_account"
title: "Get Account"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/accounts.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H07"
  - "H08"
---

# Get Account

## Purpose

Read current authoritative plan, balance and cycle context.

## When RYX Uses It

Backend tier/credit gating and account display.

## Inputs

Authenticated self userId.

## Output

Existing plan/tier/credits/creditsTotal/cycleStartedAt/nextRefreshAt/updatedAt.

## Permissions

Own authenticated actor.

## Constraints

Current read can create Free defaults or refresh a due cycle. Allowances and wording are owned centrally; no unbounded-balance claim or invented commercial entitlement.

## Failure Behaviour

Current identity/userId/access failures; client claims do not replace backend account facts.

## Related Brain Rules

[[Credit_and_Tier_Rules#Allowances and wording]]; [[Data_Boundary#Data truth precedence]]

## Implementation Source

GET /api/ryx/account; getAccount/publicAccount. Future final billing/ledger is separate.

The current chat model has no registered autonomous function-calling tools. This note separates the existing app/backend contract from canonical intended constraints requiring later alignment.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/server.js` — Complete file (729 lines)
- `ryx-brain/src/accounts.js` — Complete file (178 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
