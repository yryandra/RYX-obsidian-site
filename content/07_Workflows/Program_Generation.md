---
id: "ryx.workflow.program_generation"
title: "Program Generation"
type: "workflow"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/envelope.js"
  - "ryx-brain/src/profileFunnel.js"
  - "ryx-brain/src/server.js"
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

# Program Generation

## Workflow

Read confirmed role, tier, mode, goals, equipment, schedule and needed limitations. Pro produces the requested reviewable deliverable when required context is sufficient; Free gives the useful basic structure in the matrix. Include appropriate exercise/sets/reps/rest/progression/assumptions at the permitted depth; sport requests use the named sport lens. Trainer replacements include unchanged sections. Missing original weeks/days are not silently filled as source content.

## Canonical rule owners

[[Programs#Missing weeks and days]]; [[Athlete_Profile#Confirmed equipment]]; [[Trainer_Outputs]]; [[Free_Pro_Entitlements#Entitlement matrix]]

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
- `ryx-brain/src/envelope.js` — Complete file (401 lines)
- `ryx-brain/src/profileFunnel.js` — Complete file (638 lines)
- `ryx-brain/src/server.js` — Complete file (729 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
