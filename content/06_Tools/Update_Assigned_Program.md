---
id: "ryx.tool.update_assigned_program"
title: "Update Assigned Program"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "trainer"
source_files:
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/identityRoutes.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H02"
  - "H03"
  - "H04"
  - "H05"
  - "H06"
  - "H07"
  - "H08"
  - "H10"
  - "H11"
  - "H12"
---

# Update Assigned Program

## Contract and rule authority

The contract below describes an existing app/backend capability; canonical intended constraints are owned by [[Brain_Architecture#Global instruction precedence]], [[Data_Access#Authenticated identity and access]], [[Data_Boundary#Data truth precedence]], [[Data_Boundary#Action confirmation]], [[Response_Principles#Request-specific sufficiency and deliver-first]], [[Free_Pro_Entitlements#Entitlement matrix]], [[Companion_Mode#Trainer ownership]], [[Trainer_Approval_Model#Trainer suggests, trainer approves]], [[Safety#Research statement and professional review]], [[Crisis_Handling#Terminal safety path]] and [[Athlete_Profile#Confirmed equipment]].

Current implementation limitations do not override those owners. A generic trainer greeting is independent of client selection; athlete-specific operations still require authorization. No absent ledger, memory, medical-clearance inference or autonomous model tool is promised.

# Update Assigned Program

## Purpose

Write an explicitly submitted full program as next version.

## When RYX Uses It

The app submits a reviewed trainer replacement.

## Inputs

athleteId,card,expectedVersion.

## Output

Next immutable assigned program revision.

## Permissions

Only actively connected trainer.

## Constraints

Full card validation; expectedVersion must equal latest version. No implicit merge of omitted days.

## Failure Behaviour

403 wrong role/relationship; 400 invalid card; 409 stale version, reload/review.

## Related Brain Rules

[[Trainer_Approval_Model]] · [[Programs]]

## Implementation Source

PUT /api/ryx/athletes/:athleteId/program; writeProgram.

This is an app/backend capability. The inspected chat model has no registered function-calling tools; it may explain/request a user action but cannot invoke this autonomously.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/src/identityRoutes.js` — Complete file (61 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
