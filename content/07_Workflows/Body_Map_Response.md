---
id: "ryx.workflow.body_map_response"
title: "Body Map Response"
type: "workflow"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/replyGuards.js"
  - "ryx-brain/src/bodymapFormat.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H02"
  - "H03"
  - "H04"
  - "H09"
---

# Body Map Response

## Workflow

Read confirmed original scale, feel type, region/side, time/window and peak-versus-individual rating. Body reports are subjective signals, not diagnoses or clearance. Safety overrides Body Map optimization; weak professional mentions, improved pain or absent reports cannot clear rehabilitation. Logging is an explicit app operation, not an inferred state.

## Canonical rule owners

[[Body_Map]]; [[Pain_and_Injury#Active pain and clearance]]; [[Safety#Research statement and professional review]]; [[Log_Body_Report]]

Canonical delivery: [[Response_Principles#Request-specific sufficiency and deliver-first]].
Canonical data: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]].
Canonical safety: [[Safety#Scope and boundaries]]; [[Crisis_Handling#Terminal safety path]].


This workflow references its rule owners rather than creating another tier, safety, voice or access authority. It cannot override higher-priority rules.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/core.js` — Complete file (147 lines)
- `ryx-brain/src/replyGuards.js` — Complete file (106 lines)
- `ryx-brain/src/bodymapFormat.js` — Complete file (54 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
