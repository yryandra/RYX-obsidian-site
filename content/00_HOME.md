---
id: ryx.navigation.home
title: RYX Brain
type: core
status: reference_only
version: 0.2.0
applies_to:
  - athlete
  - trainer
source_files:
  - ryx-brain/src/prompts/core.js
  - ryx-brain/src/buildSystemPrompt.js
  - CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md
last_reviewed: 2026-10-14
canonical: false
jotbird_link: https://share.jotbird.com/spicy-stellar-chili-pepper
jotbird_expires: 2026-11-13
---

# RYX Brain

## Start here

[[RYX_Identity|Meet ryx]] · [[Personality_and_Voice#Voice and tone|Voice and tone]] · [[Brain_Architecture#Global instruction precedence|Which rules win]] · [[Safety|Safety]]

## Releases and status

Migration baseline:
[[RYX_Brain_v0.1.0]]

Reviewed candidate:
[[RYX_Brain_v0.2.0]]

Decision record:
[[RYX_BRAIN_DECISIONS]]

Runtime status:
NOT YET INTEGRATED

The candidate defines intended behavior; it does not claim production code already follows every decision. The migration manifest and audit are unchanged. Exact before-review notes are in [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Roles

Athlete → [[Athlete_Role]] → [[Solo_Mode]] / [[Companion_Mode]] → [[Athlete_Free]] / [[Athlete_Pro]].
Trainer → [[Trainer_Role]] → [[Trainer_Approval_Model]] → [[Trainer_Free]] / [[Trainer_Pro]].
Both use [[Free_Pro_Entitlements|One entitlement matrix]].

## Data and knowledge

[[Data_Boundary#Data truth precedence|Data truth priority]] · [[Known_Context]] · [[SESSION]] · [[Athlete_Snapshot]] · [[Knowledge_System]] · [[Exercise_Library]]

## Domains and workflows

[[Athlete_Profile]] · [[Check_Ins]] · [[Training_Sessions]] · [[Programs]] · [[Body_Map]] · [[Todos_and_Habits]] · [[Goals]] · [[Events]] · [[Progress_and_Adherence]] · [[Direct_Messaging]]

[[Athlete_Onboarding]] · [[Athlete_Check_In]] · [[Daily_Training]] · [[Program_Generation]] · [[Program_Adjustment]] · [[Body_Map_Response]]

[[Trainer_Client_Brief]] · [[Trainer_Check_In_Analysis]] · [[Trainer_Program_Draft]] · [[Trainer_Client_Message_Draft]] · [[06_Tools/README|Backend capability guide]]

## Review before implementation

[[CANONICALIZATION_REVIEW]] · [[MIGRATION_REVIEW]] · [[MIGRATION_MAP]] · [[Eval_System]] · [[Coverage]] · [[00_README]]

No runtime loader, provider change, API change, database change or deployment has been performed.

## Source reference

- `ryx-brain/src/prompts/core.js`
- `ryx-brain/src/buildSystemPrompt.js`

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
