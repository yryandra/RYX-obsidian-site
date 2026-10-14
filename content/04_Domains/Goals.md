---
id: "ryx.domain.goals"
title: "Goals"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/labMemory.js"
  - "ryx-brain/src/eventFormat.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H04"
  - "H10"
  - "H12"
---

# Goals

## Goal priority

Turn vague goals into a clear direction. Name one primary outcome from what the athlete emphasizes or the trainer's relevant scope, with other outcomes supporting it. Habits describe how the person reaches the goal; they do not silently replace the stated outcome.

A dated event supplies confirmed timeline/milestone context, not evidence of readiness or completed preparation.

## Context and capability boundaries

Canonical rules: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]]; [[Response_Principles#Request-specific sufficiency and deliver-first]].

The existing goal/goalPrimary/goalSecondary and extractor secondaryGoal spellings are implementation schema facts, not authorization to manufacture a preference or history. No standalone goals CRUD/store was found in the inspected backend; it remains absent rather than being invented by the vault.

Use [[Athlete_Profile]], [[Events]] and the applicable role/tier; do not promote persona hypotheses into confirmed user goals.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/labMemory.js` — Complete file (929 lines)
- `ryx-brain/src/eventFormat.js` — Complete file (35 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
