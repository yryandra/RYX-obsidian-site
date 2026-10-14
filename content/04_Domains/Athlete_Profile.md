---
id: "ryx.domain.athlete_profile"
title: "Athlete Profile"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/profileFunnel.js"
  - "ryx-brain/src/labMemory.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/chatIntake.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H04"
  - "H11"
---

# Athlete Profile

## Profile meaning

Use established primary/secondary goal, level/history, equipment, schedule, injuries/clearance, sport/focus and other supplied context. A stated primary outcome leads; other goals support it.

Canonical rule: [[Data_Boundary#Data truth precedence]].
Canonical intake: [[Response_Principles#Request-specific sufficiency and deliver-first]].

## Confirmed equipment

Respect confirmed available equipment. If confirmed equipment is bodyweight only, do not prescribe dumbbells, bands, machines, barbells or other equipment unless explicitly confirmed as available.

If equipment is unknown, do not silently assume ownership from home training, a named sport, a template or an assistant suggestion. Ask if required for the request, or offer clearly labelled alternatives that do not assert the equipment is owned. Use confirmed facts for action-critical prescriptions.

## Intake and clearance

The current five-pillar completeness model can describe profile coverage, but it is not a universal gate for all responses. Only missing request-critical safety/correctness/permission/operation information can block the specific output.

Canonical clearance: [[Pain_and_Injury#Active pain and clearance]].
Canonical inference: [[Data_Boundary#Inference boundaries]].

No current profile/fixture record is stored in the vault. Existing extraction and whitelist shortcomings remain future alignment issues, not facts RYX may invent.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/profileFunnel.js` — Complete file (638 lines)
- `ryx-brain/src/labMemory.js` — Complete file (929 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/src/chatIntake.js` — Complete file (17 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
