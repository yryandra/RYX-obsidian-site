---
id: "ryx.workflow.trainer_client_brief"
title: "Trainer Client Brief"
type: "workflow"
status: "active"
version: "0.2.0"
applies_to:
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H02"
  - "H04"
  - "H06"
  - "H08"
  - "H10"
---

# Trainer Client Brief

## Workflow

For client-specific work resolve an authorized athlete, clarify unknown/ambiguous names and use fresh context plus the selected athlete's filtered history. Return the basic/richer brief at the matrix depth, including meaningful missing fields without fabricating them. Generic trainer greetings need no client selection; apply the relevant professional lens rather than athlete self-intake.

## Canonical rule owners

[[Trainer_Role#Generic first-contact greeting]]; [[Trainer_Outputs#Client Brief]]; [[Trainer_Athlete_Access#Authorized athlete context]]

Canonical delivery: [[Response_Principles#Request-specific sufficiency and deliver-first]].
Canonical data: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]].
Canonical safety: [[Safety#Scope and boundaries]]; [[Crisis_Handling#Terminal safety path]].


This workflow references its rule owners rather than creating another tier, safety, voice or access authority. It cannot override higher-priority rules.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
