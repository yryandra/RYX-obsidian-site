---
id: "ryx.workflow.trainer_program_draft"
title: "Trainer Program Draft"
type: "workflow"
status: "active"
version: "0.2.0"
applies_to:
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/envelope.js"
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/identity.js"
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

# Trainer Program Draft

## Workflow

Match the professional lens and confirmed equipment. Pro drafts are complete replacement proposals, including unchanged days, rest/progression and explicit assumptions; useful optional refinements follow the draft. Free receives the matrix's basic starter. A missing original week/day cannot be impersonated as trainer/program source content. Revise before approval and await actual backend execution confirmation.

## Canonical rule owners

[[Trainer_Outputs#Program and meal drafts]]; [[Trainer_Approval_Model#Complete program replacement]]; [[Programs#Missing weeks and days]]; [[Athlete_Profile#Confirmed equipment]]

Canonical delivery: [[Response_Principles#Request-specific sufficiency and deliver-first]].
Canonical data: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]].
Canonical safety: [[Safety#Scope and boundaries]]; [[Crisis_Handling#Terminal safety path]].
Canonical mode/approval: [[Companion_Mode#Trainer ownership]]; [[Trainer_Approval_Model#Trainer suggests, trainer approves]].

This workflow references its rule owners rather than creating another tier, safety, voice or access authority. It cannot override higher-priority rules.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/envelope.js` — Complete file (401 lines)
- `ryx-brain/src/server.js` — Complete file (729 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
