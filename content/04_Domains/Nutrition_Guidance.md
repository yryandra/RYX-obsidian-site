---
id: "ryx.domain.nutrition_guidance"
title: "Nutrition Guidance"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/knowledge/wedgeFormat.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H03"
  - "H04"
  - "H06"
  - "H12"
---

# Nutrition Guidance

## Existing guidance scope

Support sustainable goal-based meal structure, protein/hydration, food swaps and practical adherence. Nutrition-only needs receive the appropriate narrower expert/lens; preserve existing personalization for eating-out, schedule, travel and Ramadan at the permitted Pro depth.

Canonical safety: [[Safety#Scope and boundaries]]; [[Safety#Research statement and professional review]].
Canonical referral: [[Referral_Rules#Referral map]].
Canonical entitlement: [[Free_Pro_Entitlements#Entitlement matrix]].
Canonical trainer output: [[Trainer_Outputs#Program and meal drafts]].

## Data and evidence

Use confirmed context and clearly labelled noncritical assumptions. Do not turn dietary preferences, body metrics or check-in values into facts through inference.

Canonical rules: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]]; [[Knowledge_System#Provenance and evidence]].

Niche nutrition claims, caveats and evidence strength remain intact in source knowledge. No new nutrition science, target values, clinical scope or commercial feature is added here. Basic Free protein/hydration guidance and mandatory safety wording remain visible.

## Canonical rule references

Canonical rule: [[Free_Pro_Entitlements#Useful basic value]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/prompts/core.js` — Complete file (147 lines)
- `ryx-brain/src/knowledge/wedgeFormat.js` — Complete file (210 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
