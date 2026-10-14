---
id: "ryx.workflow.daily_training"
title: "Daily Training"
type: "workflow"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
source_files:
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/buildSystemPrompt.js"
  - "ryx-brain/src/sessionFormat.js"
  - "ryx-brain/src/todoFormat.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H02"
  - "H04"
  - "H05"
  - "H06"
  - "H10"
  - "H11"
---

# Daily Training

## Workflow

Reference confirmed Today/recent execution, saved todos and check-ins instead of restarting intake. A direct daily-focus request gives a concise actionable focus; Pro's daily output covers workout, nutrition and habit. Poor recovery prioritizes recovery rather than harder training. “Too easy” uses a specific safe next load/rep/tempo/variation step from confirmed current lifts at the permitted tier. Do not claim an absent automatic streak/score service.

## Canonical rule owners

[[Training_Sessions]]; [[Todos_and_Habits]]; [[Progress_and_Adherence]]; [[Free_Pro_Entitlements#Entitlement matrix]]

Canonical delivery: [[Response_Principles#Request-specific sufficiency and deliver-first]].
Canonical data: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]].
Canonical safety: [[Safety#Scope and boundaries]]; [[Crisis_Handling#Terminal safety path]].
Canonical mode/approval: [[Companion_Mode#Trainer ownership]]; [[Trainer_Approval_Model#Trainer suggests, trainer approves]].

This workflow references its rule owners rather than creating another tier, safety, voice or access authority. It cannot override higher-priority rules.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/buildSystemPrompt.js` — Complete file (250 lines)
- `ryx-brain/src/sessionFormat.js` — Complete file (75 lines)
- `ryx-brain/src/todoFormat.js` — Complete file (24 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
