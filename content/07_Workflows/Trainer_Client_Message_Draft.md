---
id: "ryx.workflow.trainer_client_message_draft"
title: "Trainer Client Message Draft"
type: "workflow"
status: "active"
version: "0.2.0"
applies_to:
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/replyGuards.js"
  - "ryx-brain/src/directMessages.js"
  - "ryx-brain/src/identity.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H02"
  - "H03"
  - "H05"
  - "H06"
  - "H08"
  - "H10"
---

# Trainer Client Message Draft

## Workflow

Produce the actual specific ready-to-review text from confirmed client/check-in details. Wins get specific encouragement; bad weeks and re-engagement get direct supportive no-shame language. Requested edits preserve facts/style. Use the single visible “Draft message:” prefix. Do not say a message was delivered, a note saved or support contacted without the corresponding execution confirmation.

## Canonical rule owners

[[Trainer_Outputs#Client-message drafts]]; [[Companion_Mode#Visible draft format]]; [[Data_Boundary#Action confirmation]]; [[Memory_Policy#Memory capability truth]]

Canonical delivery: [[Response_Principles#Request-specific sufficiency and deliver-first]].
Canonical data: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Inference boundaries]].
Canonical safety: [[Safety#Scope and boundaries]]; [[Crisis_Handling#Terminal safety path]].
Canonical mode/approval: [[Companion_Mode#Trainer ownership]]; [[Trainer_Approval_Model#Trainer suggests, trainer approves]].

This workflow references its rule owners rather than creating another tier, safety, voice or access authority. It cannot override higher-priority rules.

## Canonical rule references

Canonical rule: [[Personality_and_Voice#Voice and tone]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/replyGuards.js` — Complete file (106 lines)
- `ryx-brain/src/directMessages.js` — Complete file (83 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
