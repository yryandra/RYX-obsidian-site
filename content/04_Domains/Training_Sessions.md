---
id: "ryx.domain.training_sessions"
title: "Training Sessions"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/docs/sessions.md"
  - "ryx-brain/src/sessions.js"
  - "ryx-brain/src/sessionFormat.js"
  - "ryx-brain/src/cardLayout.js"
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "ryx-landing/src/App.jsx"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H02"
  - "H04"
  - "H05"
  - "H11"
---

# Training Sessions

## Execution records

Sessions represent planned, in_progress, completed or skipped training. Exercise outcomes are pending, done or skipped. Current app logic can complete an in-progress session when all exercises are done-or-skipped, so completed is not proof every exercise was performed.

The shared snapshot supplies current Today/recent logs and the latest finished session by completion order, including actual exercise outcomes/notes. Current display depth is documented in [[Athlete_Snapshot]].

## Interpretation and equipment

Use actual app-confirmed execution for adherence/reflection. Do not infer program completion, training history, scheduled work or equipment ownership.

Canonical rules: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Action confirmation]]; [[Athlete_Profile#Confirmed equipment]].
Canonical coaching interpretation: [[Progress_and_Adherence]].

## Cards, source content and gaps

The live athlete frontend can post an arriving workout card as a planned Today session and show a receipt after success. This is distinct from completing the workout, approving an assigned program or sending communication.

Card-to-session parsing currently includes all section items and may reuse an unfinished matching title/date. A missing trainer/template day is not silently completed by reusing or inventing source content; additions must be labelled RYX-generated drafts under [[Programs#Missing weeks and days]].

## Safety and request sufficiency

Canonical rules: [[Safety#Scope and boundaries]]; [[Crisis_Handling#Terminal safety path]]; [[Response_Principles#Request-specific sufficiency and deliver-first]].

Unrelated incomplete intake cannot strip a valid session response. No training prescription or planned card is introduced on a terminal crisis response. Current UTC date extraction and persistence remain unchanged.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/docs/sessions.md` — Complete file (36 lines)
- `ryx-brain/src/sessions.js` — Complete file (206 lines)
- `ryx-brain/src/sessionFormat.js` — Complete file (75 lines)
- `ryx-brain/src/cardLayout.js` — Complete file (48 lines)
- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)
- `ryx-landing/src/App.jsx` — Complete file (3315 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
