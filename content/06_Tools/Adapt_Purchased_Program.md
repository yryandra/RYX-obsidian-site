---
id: "ryx.tool.adapt_purchased_program"
title: "Adapt Purchased Program"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/programs.js"
  - "ryx-brain/src/programCatalog.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H05"
  - "H08"
  - "H11"
---

# Adapt Purchased Program

## Purpose

Return a selected marketplace-session draft within confirmed equipment and source-content limits.

## When RYX Uses It

Explicit app adapt/Add to my training workflow.

## Inputs

userId, programId and confirmed equipment/level profile.

## Output

Existing route returns purchase/program/day/adaptedCard/adaptations/coachMessage/action; any generated gap fill must be labelled as a suggestion.

## Permissions

Authenticated self actor; connected-client context uses the checked snapshot, not cross-user self-service writes.

## Constraints

Do not prescribe unavailable equipment or impersonate absent source weeks/days. Current hook may create a stub purchase; it has no payment verification or automatic week advancement. Fixed bodyweight/home swaps and first-day fallback still require future H11 alignment.

## Failure Behaviour

Current route reports missing/unknown program errors. A required unknown equipment/source gap is identified rather than silently filled. No claim of assigned-program replacement or verified payment.

## Related Brain Rules

[[Athlete_Profile#Confirmed equipment]]; [[Programs#Missing weeks and days]]; [[Companion_Mode#Trainer ownership]]; [[Trainer_Approval_Model#Trainer suggests, trainer approves]]

## Implementation Source

POST /api/ryx/programs/adapt; adaptProgramToUser. Existing hook is NOT YET ALIGNED with the intended equipment/gap constraints.

The current chat model has no registered autonomous function-calling tools. This note separates the existing app/backend contract from canonical intended constraints requiring later alignment.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/server.js` — Complete file (729 lines)
- `ryx-brain/src/programs.js` — Complete file (245 lines)
- `ryx-brain/src/programCatalog.js` — Complete file (223 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
