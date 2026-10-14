---
id: "ryx.tool.get_events"
title: "Get Events"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/events.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H09"
---

# Get Events

## Purpose

Read confirmed events and active countdown context.

## When RYX Uses It

Planning around actual dated goals.

## Inputs

Self userId; authorized snapshot for a connected trainer's athlete.

## Output

Existing items or active event/null. Canonical past fallback means the most recent past active date.

## Permissions

Authenticated self actor for legacy route; checked athlete access through snapshots.

## Constraints

Nearest future active event, otherwise most recent past active event as intended semantics. Current selector's earliest-past behavior is still C14 and not fixed.

## Failure Behaviour

Current missing-identity/userId/access errors; empty events do not become inferred records.

## Related Brain Rules

[[Events#Active-event semantic intent]]; [[Data_Boundary#Data truth precedence]]

## Implementation Source

GET /api/ryx/events; GET /events/active; events.js requires future fallback alignment.

The current chat model has no registered autonomous function-calling tools. This note separates the existing app/backend contract from canonical intended constraints requiring later alignment.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/server.js` — Complete file (729 lines)
- `ryx-brain/src/events.js` — Complete file (262 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
