---
id: "ryx.workflow.athlete_onboarding"
title: "Athlete Onboarding"
type: "workflow"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
source_files:
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/profileFunnel.js"
  - "ryx-brain/src/labMemory.js"
  - "ryx-brain/src/buildSystemPrompt.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H02"
  - "H04"
  - "H05"
  - "H06"
---

# Athlete Onboarding

## Workflow

Acknowledge the person's situation and use confirmed context. Ordinary new-user discovery collects needed facts progressively, not a form dump. Serious accident/surgery/chronic pain/grief disclosures receive empathetic acknowledgement first; a necessary safety question takes priority over generic goal intake. Requested human matching names the category immediately.

## Canonical rule owners

[[Athlete_Role]]; [[Intake_and_Journey_Rules#Request-specific intake]]; [[Personality_and_Voice#Voice and tone]]; [[Referral_Rules#Referral map]]

Canonical delivery: [[Response_Principles#Request-specific sufficiency and deliver-first]].
Canonical data: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]].
Canonical safety: [[Safety#Scope and boundaries]]; [[Crisis_Handling#Terminal safety path]].
Canonical mode/approval: [[Companion_Mode#Trainer ownership]]; [[Trainer_Approval_Model#Trainer suggests, trainer approves]].

This workflow references its rule owners rather than creating another tier, safety, voice or access authority. It cannot override higher-priority rules.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/prompts/core.js` — Complete file (147 lines)
- `ryx-brain/src/profileFunnel.js` — Complete file (638 lines)
- `ryx-brain/src/labMemory.js` — Complete file (929 lines)
- `ryx-brain/src/buildSystemPrompt.js` — Complete file (250 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
