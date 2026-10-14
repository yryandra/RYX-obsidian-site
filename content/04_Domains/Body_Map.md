---
id: "ryx.domain.body_map"
title: "Body Map"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/docs/body-map.md"
  - "ryx-brain/src/bodymap.js"
  - "ryx-brain/src/bodymapFormat.js"
  - "ryx-brain/src/bodymapRegions.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "ryx-brain/src/prompts/core.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H03"
  - "H04"
  - "H09"
---

# Body Map

## Current authoritative domain model

The implemented catalog contains 34 current zones with legacy aliases under [[Body_Region_Catalog]]. The older 23-coarse-region document is a stale/legacy reference, not the canonical schema.

Body reports are subjective regional signals, not diagnoses. Current fields include region/side, note, loggedAt and feelType: soreness, tightness, pain, stiffness, swelling or other. The implementation defaults an unknown feelType to soreness.

## Original and normalized intensity

Original intensityScale is 5 or 10, with reportedIntensity retained. Heatmap representation converts/rounds to 1–10. Preserve both the athlete's original rating and normalized representation; never present normalized 6/10 as if the user originally reported 6/10 when the original was 3/5.

Current normalized labels are 1–3 mild, 4–6 moderate, 7–10 severe. The seven-day snapshot aggregates count, peak, mean and latest time by normalized region. Displayed latest feel type and window-peak intensity need not describe the same individual report.

## Interpretation under safety

Canonical rule: [[Pain_and_Injury#Active pain and clearance]].
Canonical research/referral rule: [[Safety#Research statement and professional review]].

Safety takes precedence over Body Map optimization. Flagged regions do not establish a diagnosis or permission for clearance-dependent modification. Do not treat “physio”, prior treatment, improved pain, monitoring or an absent report as clearance. General non-diagnostic guidance stays distinct from cleared rehabilitation.

Canonical data rule: [[Data_Boundary#Inference boundaries]]. Body-map state cannot be inferred into a saved/confirmed report.

## Context and current-runtime alignment

Existing region display caps are 6 Free / 12 Pro; current snapshot appends up to 20 original-scale reports. These presentation caps are not access authorization. The pain-message guard may offer a Body Map widget, but saved records and the current message matcher are distinct.

Current bodymapFormat modification wording still needs alignment to the higher safety rule. No body-map records, API changes or schema changes are created here.

## Canonical rule references

Canonical rule: [[Data_Boundary#Data truth precedence]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/docs/body-map.md` — Complete file (86 lines)
- `ryx-brain/src/bodymap.js` — Complete file (195 lines)
- `ryx-brain/src/bodymapFormat.js` — Complete file (54 lines)
- `ryx-brain/src/bodymapRegions.js` — Complete file (106 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)
- `ryx-brain/src/prompts/core.js` — Complete file (147 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
