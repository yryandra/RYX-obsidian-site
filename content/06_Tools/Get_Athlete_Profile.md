---
id: "ryx.tool.get_athlete_profile"
title: "Get Athlete Profile"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/identityRoutes.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/athleteSnapshot.js"
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

# Get Athlete Profile

## Contract and rule authority

The contract below describes an existing app/backend capability; canonical intended constraints are owned by [[Brain_Architecture#Global instruction precedence]], [[Data_Access#Authenticated identity and access]], [[Data_Boundary#Data truth precedence]], [[Data_Boundary#Action confirmation]], [[Response_Principles#Request-specific sufficiency and deliver-first]], [[Free_Pro_Entitlements#Entitlement matrix]], [[Companion_Mode#Trainer ownership]], [[Trainer_Approval_Model#Trainer suggests, trainer approves]], [[Safety#Research statement and professional review]], [[Crisis_Handling#Terminal safety path]] and [[Athlete_Profile#Confirmed equipment]].

Current implementation limitations do not override those owners. A generic trainer greeting is independent of client selection; athlete-specific operations still require authorization. No absent ledger, memory, medical-clearance inference or autonomous model tool is promised.

# Get Athlete Profile

## Purpose

Read the authenticated profile or authorized athlete profile.

## When RYX Uses It

Use established goal/level/equipment/schedule/injury context before intake or advice.

## Inputs

Authenticated actor; athleteId for snapshot-based cross-user reading.

## Output

auth/me returns the current user/profile; a snapshot returns athlete {id,name,profile}.

## Permissions

Athlete owner or actively connected trainer; backend checks relationship and canonical athlete identity.

## Constraints

No standalone public lookup by display name; names are not authorization.

## Failure Behaviour

Unauthenticated 401; unauthorized/missing athlete 403. Missing fields remain missing.

## Related Brain Rules

[[Data_Access]] · [[Athlete_Profile]] · [[Known_Context]]

## Implementation Source

GET /api/ryx/auth/me; GET /api/ryx/athletes/:athleteId/snapshot.

This is an app/backend capability. The inspected chat model has no registered function-calling tools; it may explain/request a user action but cannot invoke this autonomously.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/identityRoutes.js` — Complete file (61 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
