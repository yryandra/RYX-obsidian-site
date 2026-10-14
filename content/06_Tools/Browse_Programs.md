---
id: "ryx.tool.browse_programs"
title: "Browse Programs"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/programCatalog.js"
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

# Browse Programs

## Contract and rule authority

The contract below describes an existing app/backend capability; canonical intended constraints are owned by [[Brain_Architecture#Global instruction precedence]], [[Data_Access#Authenticated identity and access]], [[Data_Boundary#Data truth precedence]], [[Data_Boundary#Action confirmation]], [[Response_Principles#Request-specific sufficiency and deliver-first]], [[Free_Pro_Entitlements#Entitlement matrix]], [[Companion_Mode#Trainer ownership]], [[Trainer_Approval_Model#Trainer suggests, trainer approves]], [[Safety#Research statement and professional review]], [[Crisis_Handling#Terminal safety path]] and [[Athlete_Profile#Confirmed equipment]].

Current implementation limitations do not override those owners. A generic trainer greeting is independent of client selection; athlete-specific operations still require authorization. No absent ledger, memory, medical-clearance inference or autonomous model tool is promised.

# Browse Programs

## Purpose

Read static marketplace summaries or full templates.

## When RYX Uses It

User explores expert structured blocks.

## Inputs

Authenticated actor; optional programId detail.

## Output

Catalog items/count; full program detail.

## Permissions

Authenticated product session; route has no additional tier condition.

## Constraints

Three seed programs; no creator-upload service. Static templates are not an assigned trainer program.

## Failure Behaviour

404 unknown program; 401 without identity.

## Related Brain Rules

[[Programs]] · [[Marketplace_Program_Templates]]

## Implementation Source

GET /api/ryx/programs; GET /programs/:id.

This is an app/backend capability. The inspected chat model has no registered function-calling tools; it may explain/request a user action but cannot invoke this autonomously.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/server.js` — Complete file (729 lines)
- `ryx-brain/src/programCatalog.js` — Complete file (223 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
