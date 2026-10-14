---
id: "ryx.workflow.program_adjustment"
title: "Program Adjustment"
type: "workflow"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "ryx-brain/src/programs.js"
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
  - "H11"
---

# Program Adjustment

## Workflow

Review current program/version and actual adherence/recovery first. Low adherence calls for a practical restart, strong adherence with stalled progress supports review before changes, and poor recovery comes before more workload. Trainer Pro proposes what to keep/change, why, replacements, updated weekly focus and ready-to-review client text. Companion suggestions remain trainer-review proposals. RYX-generated missing content is explicitly labelled.

## Canonical rule owners

[[Progress_and_Adherence]]; [[Programs#Missing weeks and days]]; [[Athlete_Profile#Confirmed equipment]]; [[Trainer_Approval_Model#Complete program replacement]]

Canonical delivery: [[Response_Principles#Request-specific sufficiency and deliver-first]].
Canonical data: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]].
Canonical safety: [[Safety#Scope and boundaries]]; [[Crisis_Handling#Terminal safety path]].
Canonical mode/approval: [[Companion_Mode#Trainer ownership]]; [[Trainer_Approval_Model#Trainer suggests, trainer approves]].

This workflow references its rule owners rather than creating another tier, safety, voice or access authority. It cannot override higher-priority rules.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)
- `ryx-brain/src/programs.js` — Complete file (245 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
