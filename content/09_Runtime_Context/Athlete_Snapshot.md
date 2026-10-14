---
id: "ryx.runtime.context.athlete_snapshot"
title: "Athlete Snapshot"
type: "runtime-context"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/athleteSnapshot.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/docs/shared-athlete-data.md"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H04"
  - "H05"
  - "H06"
  - "H09"
  - "H10"
  - "H11"
---

# Athlete Snapshot

## Shared authorized context

The existing snapshot is read fresh after authorization for both roles, without a per-trainer data copy or cross-request snapshot cache. Use only the selected authorized athlete.

Canonical rule: [[Data_Boundary#Data truth precedence]]; [[Trainer_Athlete_Access#Authorized athlete context]].

## Schema and current context depth

Schema only: athlete {id,name,profile}; fetchedAt; sessions up to 50; lastSession by completed/skipped completion timestamp; todaySessions up to 10; checkins up to 30; todos up to 100; events; activeEvent; seven-day bodymap; purchases; latest assignedProgram.

Existing formatter display caps:
- training rows: 5 Free / 14 Pro, plus Today;
- check-ins: 4 Free / 12 Pro, with Pro trends;
- open todos: 8 Free / 12 Pro;
- event unfinished milestones: 3 Free / 6 Pro;
- Body Map regions: 6 Free / 12 Pro;
- active marketplace purchases when no assigned program: 2 Free / 5 Pro.

Current raw additions include the latest finished session, up to 10 completed todos, up to 20 original-scale body reports and a serialized assigned program without those display caps. These are implementation facts, not authorization rules or a new entitlement promise.

## Interpretation constraints

Preserve original scales and actual outcomes; completed can include skipped exercises. Assigned trainer ownership remains authoritative. Missing snapshot values do not become inferred records, clearance, equipment or completion. Confirmed app execution is distinct from a model draft.

Canonical rules: [[Data_Boundary#Inference boundaries]]; [[Data_Boundary#Action confirmation]]; [[Athlete_Profile#Confirmed equipment]]; [[Companion_Mode#Trainer ownership]].

No snapshot values/user records are migrated. Current extraction/mode/context limits remain future alignment concerns in the decision record.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/docs/shared-athlete-data.md` — Complete file (138 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
