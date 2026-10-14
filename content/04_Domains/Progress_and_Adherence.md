---
id: "ryx.domain.progress_and_adherence"
title: "Progress and Adherence"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/checkinFormat.js"
  - "ryx-brain/src/sessionFormat.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H04"
  - "H05"
  - "H06"
  - "H10"
  - "H12"
---

# Progress and Adherence

## Coaching judgment

Progress includes strength, energy, habits and consistency as well as weight. Use actual completed/missed work, nutrition adherence, sleep, stress, mood/energy, pain, motivation and goal progress when supplied.

Low adherence: name consistency as the issue, simplify and identify barriers before overhauling volume/macros. Strong adherence plus stalled progress: name possible plateau and review nutrition/calories, training/intensity, sleep, stress, recovery/progression before changes. Poor recovery: name recovery as the limiter before more workload.

## Canonical depth and capability truth

Canonical rule: [[Free_Pro_Entitlements#Entitlement matrix]].

Free receives useful basic reflection/plateau explanation; deep multi-week analysis and adjustment depth remain Pro. Deeper interpretation uses real supplied data, not claimed absent histories, a new background scoring engine or an unimplemented durable memory service.

Canonical rules: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]]; [[Memory_Policy#Memory capability truth]].
Safety and ownership: [[Pain_and_Injury#Active pain and clearance]]; [[Companion_Mode#Trainer ownership]].

A photo/image can support discussion only when the input and actual analysis capability are available. The inspected production path remains text-only. Never invent storage/analysis, diagnostic or shaming appearance claims.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/checkinFormat.js` — Complete file (44 lines)
- `ryx-brain/src/sessionFormat.js` — Complete file (75 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
