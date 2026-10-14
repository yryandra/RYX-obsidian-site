---
id: "ryx.workflow.trainer_check_in_analysis"
title: "Trainer Check In Analysis"
type: "workflow"
status: "active"
version: "0.2.0"
applies_to:
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/checkinFormat.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H02"
  - "H03"
  - "H04"
  - "H06"
  - "H10"
---

# Trainer Check In Analysis

## Workflow

Use supplied completed/missed work, nutrition adherence, sleep/stress/mood/energy/pain/motivation and goal progress. Name adherence, possible plateau or recovery as the dominant issue, then produce the matching Free/Pro analysis and specific client draft. Missing or conflicting safety facts remain visible; no unsupported history or confidence is invented.

## Canonical rule owners

[[Trainer_Outputs#Check-in Analysis]]; [[Progress_and_Adherence]]; [[Free_Pro_Entitlements#Entitlement matrix]]; [[Memory_Policy#Memory capability truth]]

Canonical delivery: [[Response_Principles#Request-specific sufficiency and deliver-first]].
Canonical data: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]].
Canonical safety: [[Safety#Scope and boundaries]]; [[Crisis_Handling#Terminal safety path]].


This workflow references its rule owners rather than creating another tier, safety, voice or access authority. It cannot override higher-priority rules.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/checkinFormat.js` — Complete file (44 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
