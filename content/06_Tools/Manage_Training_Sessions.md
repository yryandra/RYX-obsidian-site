---
id: "ryx.tool.manage_training_sessions"
title: "Manage Training Sessions"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/sessions.js"
  - "ryx-brain/src/sessionFormat.js"
  - "ryx-landing/src/App.jsx"
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

# Manage Training Sessions

## Contract and rule authority

The contract below describes an existing app/backend capability; canonical intended constraints are owned by [[Brain_Architecture#Global instruction precedence]], [[Data_Access#Authenticated identity and access]], [[Data_Boundary#Data truth precedence]], [[Data_Boundary#Action confirmation]], [[Response_Principles#Request-specific sufficiency and deliver-first]], [[Free_Pro_Entitlements#Entitlement matrix]], [[Companion_Mode#Trainer ownership]], [[Trainer_Approval_Model#Trainer suggests, trainer approves]], [[Safety#Research statement and professional review]], [[Crisis_Handling#Terminal safety path]] and [[Athlete_Profile#Confirmed equipment]].

Current implementation limitations do not override those owners. A generic trainer greeting is independent of client selection; athlete-specific operations still require authorization. No absent ledger, memory, medical-clearance inference or autonomous model tool is promised.

# Manage Training Sessions

## Purpose

Create a manual/card session, update execution/notes or delete it.

## When RYX Uses It

App training actions; the live athlete frontend also automatically creates a planned Today session when a workout card arrives. RYX reflects confirmed state.

## Inputs

userId; title/card/action/exercises/scheduledDate/status/notes; sessionId for updates; exerciseId/exerciseStatus for execution.

## Output

session or ok confirmation.

## Permissions

Authenticated actor only; supplied userId must match the actor. Connected trainers read another athlete through the checked snapshot, not the legacy self-service route.

## Constraints

Create is planned unless in_progress. Card conversion needs a workout card and parsed rows; same unfinished card title/date may reuse. All done/skipped rows can complete in-progress session.

## Failure Behaviour

400 cannot create from card; 404 missing update/delete target; do not claim completion before confirmation.

## Related Brain Rules

[[Training_Sessions]] · [[Output_and_Card_Behaviour]]

## Implementation Source

POST /sessions; PATCH/DELETE /sessions/:id.

This is an app/backend capability. The inspected chat model has no registered function-calling tools; it may explain/request a user action but cannot invoke this autonomously.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/server.js` — Complete file (729 lines)
- `ryx-brain/src/sessions.js` — Complete file (206 lines)
- `ryx-brain/src/sessionFormat.js` — Complete file (75 lines)
- `ryx-landing/src/App.jsx` — Complete file (3315 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
