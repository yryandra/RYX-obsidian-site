---
id: "ryx.tool.draft_program"
title: "Draft Program"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "trainer"
source_files:
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/envelope.js"
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

# Draft Program

## Contract and rule authority

The contract below describes an existing app/backend capability; canonical intended constraints are owned by [[Brain_Architecture#Global instruction precedence]], [[Data_Access#Authenticated identity and access]], [[Data_Boundary#Data truth precedence]], [[Data_Boundary#Action confirmation]], [[Response_Principles#Request-specific sufficiency and deliver-first]], [[Free_Pro_Entitlements#Entitlement matrix]], [[Companion_Mode#Trainer ownership]], [[Trainer_Approval_Model#Trainer suggests, trainer approves]], [[Safety#Research statement and professional review]], [[Crisis_Handling#Terminal safety path]] and [[Athlete_Profile#Confirmed equipment]].

Current implementation limitations do not override those owners. A generic trainer greeting is independent of client selection; athlete-specific operations still require authorization. No absent ledger, memory, medical-clearance inference or autonomous model tool is promised.

# Draft Program

## Purpose

Create a reviewable model card and server-owned trainer draft.

## When RYX Uses It

Trainer asks for program generation/adjustment within tier/safety rules.

## Inputs

Selected connected athlete; complete card; source/base version; generation context.

## Output

Card with draftId/athleteId; no assigned program change.

## Permissions

Authenticated trainer with authorized selected athlete.

## Constraints

Only program actions weekly_plan/generate_workout/modify_workout/major_adjustment create the server draft. Complete replacement required; save is not approval.

## Failure Behaviour

Invalid card/base version errors; revoked access blocks after generation. Do not call draft applied.

## Related Brain Rules

[[Trainer_Approval_Model]] · [[Trainer_Program_Draft]]

## Implementation Source

Production /chat call to createProgramDraft; not a standalone model tool/API endpoint.

This is an app/backend capability. The inspected chat model has no registered function-calling tools; it may explain/request a user action but cannot invoke this autonomously.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/server.js` — Complete file (729 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/envelope.js` — Complete file (401 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
