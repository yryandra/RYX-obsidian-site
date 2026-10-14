---
id: "ryx.tool.change_plan_and_credits"
title: "Change Plan and Credits"
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

# Change Plan and Credits

## Purpose

Document the existing MVP self-service plan/top-up operation.

## When RYX Uses It

Explicit app plan/top-up interaction; not autonomous model billing.

## Inputs

Own userId; existing plan free/pro; positive finite addCredits.

## Output

Current public account after backend operation.

## Permissions

Own authenticated actor; no new billing permission or payment verifier is introduced.

## Constraints

Existing grants/rollover/action weights remain unchanged. Current endpoint has no payment verification. Future final executed-action costing, balance check, charge-once and ledger apply to chat billing; a ledger is not currently claimed.

## Failure Behaviour

Existing invalid-top-up/auth/access errors. Do not represent a stub operation as verified payment.

## Related Brain Rules

[[Credit_and_Tier_Rules#Allowances and wording]]; [[Credit_and_Tier_Rules#Final action and billing]]; [[Data_Boundary#Action confirmation]]

## Implementation Source

PATCH /api/ryx/account; setPlan/addCredits. Future billing alignment sources remain unchanged.

The current chat model has no registered autonomous function-calling tools. This note separates the existing app/backend contract from canonical intended constraints requiring later alignment.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/server.js` — Complete file (729 lines)
- `ryx-brain/src/accounts.js` — Complete file (178 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
