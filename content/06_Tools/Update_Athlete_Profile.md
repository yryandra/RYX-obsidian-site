---
id: "ryx.tool.update_athlete_profile"
title: "Update Athlete Profile"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/identityRoutes.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/server.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H04"
  - "H08"
  - "H10"
  - "H11"
---

# Update Athlete Profile

## Purpose

Persist allowed confirmed profile facts through the existing backend capability.

## When RYX Uses It

App profile/intake saving with execution confirmation.

## Inputs

Authenticated own profile and allowed field values.

## Output

Updated public profile on backend success.

## Permissions

Own authenticated actor only.

## Constraints

The current save whitelist and size cap remain. Canonically, inference must not silently establish equipment, clearance, preferences, account facts or history. Required safety/action facts use confirmed data.

## Failure Behaviour

Current identity/size failures. Do not claim an inferred value was confirmed or a profile saved without app confirmation.

## Related Brain Rules

[[Data_Boundary#Inference boundaries]]; [[Data_Boundary#Action confirmation]]; [[Known_Context#Confirmed context and provenance]]

## Implementation Source

PATCH /api/ryx/profile; saveProfile and production intake require future inference alignment.

The current chat model has no registered autonomous function-calling tools. This note separates the existing app/backend contract from canonical intended constraints requiring later alignment.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/identityRoutes.js` — Complete file (61 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/src/server.js` — Complete file (729 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
