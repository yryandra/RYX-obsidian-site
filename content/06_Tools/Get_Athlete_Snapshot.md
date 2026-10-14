---
id: "ryx.tool.get_athlete_snapshot"
title: "Get Athlete Snapshot"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/athleteSnapshot.js"
  - "ryx-brain/src/identityRoutes.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/server.js"
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

# Get Athlete Snapshot

## Contract and rule authority

The contract below describes an existing app/backend capability; canonical intended constraints are owned by [[Brain_Architecture#Global instruction precedence]], [[Data_Access#Authenticated identity and access]], [[Data_Boundary#Data truth precedence]], [[Data_Boundary#Action confirmation]], [[Response_Principles#Request-specific sufficiency and deliver-first]], [[Free_Pro_Entitlements#Entitlement matrix]], [[Companion_Mode#Trainer ownership]], [[Trainer_Approval_Model#Trainer suggests, trainer approves]], [[Safety#Research statement and professional review]], [[Crisis_Handling#Terminal safety path]] and [[Athlete_Profile#Confirmed equipment]].

Current implementation limitations do not override those owners. A generic trainer greeting is independent of client selection; athlete-specific operations still require authorization. No absent ledger, memory, medical-clearance inference or autonomous model tool is promised.

# Get Athlete Snapshot

## Purpose

Read all relevant shared athlete stores fresh.

## When RYX Uses It

At each production RYX turn after authorized athlete selection.

## Inputs

actor and canonical athleteId.

## Output

Snapshot schema in Athlete_Snapshot, including current program and fetchedAt.

## Permissions

Athlete owner or actively connected trainer; backend checks relationship and canonical athlete identity.

## Constraints

No per-trainer copy/cache; formatter caps and raw additions differ by tier.

## Failure Behaviour

403 for missing/unconnected athlete; chat rechecks access after generation.

## Related Brain Rules

[[Athlete_Snapshot]] · [[Trainer_Athlete_Access]] · [[SESSION]]

## Implementation Source

GET /api/ryx/athletes/:athleteId/snapshot; buildAthleteSnapshot/snapshotContext.

This is an app/backend capability. The inspected chat model has no registered function-calling tools; it may explain/request a user action but cannot invoke this autonomously.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)
- `ryx-brain/src/identityRoutes.js` — Complete file (61 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/src/server.js` — Complete file (729 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
