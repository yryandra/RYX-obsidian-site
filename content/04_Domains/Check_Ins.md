---
id: "ryx.domain.check_ins"
title: "Check Ins"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/docs/checkins.md"
  - "ryx-brain/src/checkins.js"
  - "ryx-brain/src/checkinFormat.js"
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H02"
  - "H04"
  - "H06"
  - "H10"
---

# Check Ins

## Data meaning and current schema

Dated self-reports capture weightKg, energy, sleepHours, sleepQuality, adherence and note. Current normalization bounds weight to 30–300 kg, energy/sleep quality to 1–5, sleep to 0–14 hours and note to 500 characters; adherence is full/partial/missed. Upsert is per athlete/date and preserves omitted update fields. Missing values are not zero.

Current formatted depth is 4 rows Free / 12 Pro. Pro's simple current trends compare available latest/oldest numeric weights and average energy across supplied rows, not a clinical causal model. The snapshot can fetch up to 30 and notes are shortened in the formatter.

## Canonical interpretation

Canonical judgment: [[Progress_and_Adherence]].
Canonical output depth: [[Free_Pro_Entitlements#Entitlement matrix]].
Canonical trainer format: [[Trainer_Outputs#Check-in Analysis]].
Canonical data truth: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]].
Canonical safety: [[Safety#Scope and boundaries]]; [[Crisis_Handling#Terminal safety path]].

Use supplied signals without inventing check-in values, current pain status or successful logging. Saving requires [[Save_Check_In]] and the confirmation rule in [[Data_Boundary#Action confirmation]].

## Canonical rule references

Canonical rule: [[Free_Pro_Entitlements#Useful basic value]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/docs/checkins.md` — Complete file (22 lines)
- `ryx-brain/src/checkins.js` — Complete file (131 lines)
- `ryx-brain/src/checkinFormat.js` — Complete file (44 lines)
- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
