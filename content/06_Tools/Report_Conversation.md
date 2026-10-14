---
id: "ryx.tool.report_conversation"
title: "Report Conversation"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/reports.js"
  - "ryx-brain/src/identityRoutes.js"
  - "ryx-brain/docs/reports.md"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H08"
---

# Report Conversation

## Purpose

Persist a manually submitted review report through the existing app capability.

## When RYX Uses It

Explicit Report action or recommendation to contact support.

## Inputs

userId, valid reason, optional details/messages/role/plan.

## Output

Saved open report record when backend confirms it; no staff-review or delivery guarantee.

## Permissions

Authenticated self actor; diagnostic listing is not an ordinary user capability.

## Constraints

Current reasons/range/snapshot limits remain in code. No automatic staff escalation, email or webhook delivery is implemented. Recommending support contact differs from claiming it occurred.

## Failure Behaviour

Current invalid-reason/request/access errors. Do not claim saving, staff contact or review without the relevant confirmation.

## Related Brain Rules

[[RYX_Boundaries#Support, reporting and delivery]]; [[Data_Boundary#Action confirmation]]

## Implementation Source

POST /api/ryx/reports; diagnostic GET /reports blocked by current protectLegacyRoutes; old no-auth docs are legacy.

The current chat model has no registered autonomous function-calling tools. This note separates the existing app/backend contract from canonical intended constraints requiring later alignment.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/server.js` — Complete file (729 lines)
- `ryx-brain/src/reports.js` — Complete file (102 lines)
- `ryx-brain/src/identityRoutes.js` — Complete file (61 lines)
- `ryx-brain/docs/reports.md` — Complete file (39 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
