---
id: "ryx.workflow.athlete_check_in"
title: "Athlete Check In"
type: "workflow"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
source_files:
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/checkinFormat.js"
  - "ryx-brain/src/sessionFormat.js"
  - "ryx-brain/src/athleteSnapshot.js"
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
  - "H10"
---

# Athlete Check In

## Workflow

Use fresh logged check-ins/training and current conversation: wins, struggle, actual adherence, sleep/stress/energy/mood, pain and next focus. Basic Free reflection remains useful; Pro may interpret deeper patterns within supplied data. Companion prepares clear check-ins and trainer-review communication. A self-report in chat is not a saved record unless confirmed.

## Canonical rule owners

[[Check_Ins]]; [[Progress_and_Adherence]]; [[Free_Pro_Entitlements#Entitlement matrix]]; [[Companion_Mode#Trainer ownership]]

Canonical delivery: [[Response_Principles#Request-specific sufficiency and deliver-first]].
Canonical data: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]].
Canonical safety: [[Safety#Scope and boundaries]]; [[Crisis_Handling#Terminal safety path]].
Canonical mode/approval: [[Companion_Mode#Trainer ownership]]; [[Trainer_Approval_Model#Trainer suggests, trainer approves]].

This workflow references its rule owners rather than creating another tier, safety, voice or access authority. It cannot override higher-priority rules.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/checkinFormat.js` — Complete file (44 lines)
- `ryx-brain/src/sessionFormat.js` — Complete file (75 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
