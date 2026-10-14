---
id: "ryx.release.0.2.0"
title: "RYX Brain v0.2.0"
type: "release"
status: "review"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/buildSystemPrompt.js"
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/runChat.js"
  - "ryx-brain/src/openaiRun.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "package.json"
  - "scripts/dev.mjs"
  - "web/src/pages/CoachPage.jsx"
  - "web/src/lib/brainHealth.js"
  - "ryx-brain/src/envelope.js"
  - "ryx-brain/src/cardCoerce.js"
  - "ryx-brain/src/cardLayout.js"
  - "ryx-brain/src/formatCoachReply.js"
  - "ryx-landing/src/lib/cardLayout.js"
  - "ryx-landing/src/components/cards/RyxContentCard.jsx"
  - "ryx-landing/src/App.jsx"
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/replyGuards.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/identityRoutes.js"
  - "ryx-brain/src/credits.js"
  - "ryx-brain/src/accounts.js"
  - "ryx-brain/src/profileFunnel.js"
  - "ryx-brain/src/labMemory.js"
  - "ryx-brain/src/labSessions.js"
  - "ryx-brain/src/bodymapFormat.js"
  - "ryx-brain/src/programs.js"
  - "ryx-brain/docs/backlog.md"
  - "ryx-brain/src/chatIntake.js"
  - "ryx-brain/docs/body-map.md"
  - "ryx-brain/src/bodymap.js"
  - "ryx-brain/src/bodymapRegions.js"
  - "ryx-brain/docs/checkins.md"
  - "ryx-brain/src/checkins.js"
  - "ryx-brain/src/checkinFormat.js"
  - "ryx-brain/docs/shared-athlete-data.md"
  - "ryx-brain/src/directMessages.js"
  - "ryx-brain/src/liveEvents.js"
  - "ryx-brain/docs/event-countdown.md"
  - "ryx-brain/src/events.js"
  - "ryx-brain/src/eventFormat.js"
  - "ryx-brain/src/knowledge/wedgeFormat.js"
  - "ryx-brain/docs/program-marketplace.md"
  - "ryx-brain/src/programCatalog.js"
  - "ryx-brain/src/programFormat.js"
  - "ryx-brain/src/sessionFormat.js"
  - "ryx-brain/docs/todos.md"
  - "ryx-brain/src/todos.js"
  - "ryx-brain/src/todoFormat.js"
  - "ryx-brain/docs/sessions.md"
  - "ryx-brain/src/sessions.js"
  - "ryx-brain/src/knowledge/data/exercises.json"
  - "ryx-brain/src/knowledge/data/exerciseMediaCatalog.json"
  - "RYX_Wedge_Knowledge_Bases_v1/fitness/bodybuilding.json"
  - "RYX_Wedge_Knowledge_Bases_v1/fitness/calisthenics.json"
  - "RYX_Wedge_Knowledge_Bases_v1/fitness/crossfit.json"
  - "RYX_Wedge_Knowledge_Bases_v1/fitness/general.json"
  - "RYX_Wedge_Knowledge_Bases_v1/fitness/powerlifting.json"
  - "ryx-brain/src/knowledge/data/formDemosByWedge.json"
  - "ryx-brain/src/knowledge/README.md"
  - "ryx-brain/src/knowledge/retrieve.js"
  - "ryx-brain/src/knowledge/wedgeRouter.js"
  - "ryx-brain/src/knowledge/wedgeLoader.js"
  - "ryx-brain/src/knowledge/formDemos.js"
  - "ryx-brain/src/knowledge/nicheMap.js"
  - "RYX_Wedge_Knowledge_Bases_v1/index.json"
  - "RYX_Wedge_Knowledge_Bases_v1/sports/basketball.json"
  - "RYX_Wedge_Knowledge_Bases_v1/sports/combat.json"
  - "RYX_Wedge_Knowledge_Bases_v1/sports/football.json"
  - "RYX_Wedge_Knowledge_Bases_v1/sports/golf.json"
  - "RYX_Wedge_Knowledge_Bases_v1/sports/padel.json"
  - "RYX_Wedge_Knowledge_Bases_v1/sports/swimming.json"
  - "RYX_Wedge_Knowledge_Bases_v1/sports/tennis.json"
  - "RYX_Wedge_Knowledge_Bases_v1/wellness/rehab.json"
  - "RYX_Wedge_Knowledge_Bases_v1/wellness/yoga.json"
  - "ryx-landing/src/lib/identityApi.js"
  - "ryx-brain/src/reports.js"
  - "ryx-brain/docs/reports.md"
last_reviewed: "2026-10-14"
canonical: false
---

# RYX Brain v0.2.0

This release defines reviewed intended RYX behaviour.
Production runtime is not yet aligned with all decisions in this release.

This is a CANDIDATE reviewed brain release, not production activation or a concatenated prompt. Apply the global hierarchy and compile canonical rule owners once. Runtime interpretation notes are listed with Domains; they contain schema/rules, not live records.

## Core

- [[01_Core/Brain_Architecture]]
- [[01_Core/Output_and_Card_Behaviour]]
- [[01_Core/Personality_and_Voice]]
- [[01_Core/Response_Principles]]
- [[01_Core/RYX_Identity]]

## Roles

- [[02_Roles/Athlete/Athlete_Free]]
- [[02_Roles/Athlete/Athlete_Pro]]
- [[02_Roles/Athlete/Athlete_Role]]
- [[02_Roles/Athlete/Companion_Mode]]
- [[02_Roles/Athlete/Solo_Mode]]
- [[02_Roles/Trainer/Trainer_Approval_Model]]
- [[02_Roles/Trainer/Trainer_Free]]
- [[02_Roles/Trainer/Trainer_Outputs]]
- [[02_Roles/Trainer/Trainer_Pro]]
- [[02_Roles/Trainer/Trainer_Role]]

## Policies

- [[03_Policies/Credit_and_Tier_Rules]]
- [[03_Policies/Crisis_Handling]]
- [[03_Policies/Data_Access]]
- [[03_Policies/Deterministic_Reply_Guards]]
- [[03_Policies/Free_Pro_Entitlements]]
- [[03_Policies/Memory_Policy]]
- [[03_Policies/Pain_and_Injury]]
- [[03_Policies/Referral_Rules]]
- [[03_Policies/RYX_Boundaries]]
- [[03_Policies/Safety]]
- [[03_Policies/Trainer_Athlete_Access]]

## Domains

- [[04_Domains/Athlete_Profile]]
- [[04_Domains/Body_Map]]
- [[04_Domains/Body_Region_Catalog]]
- [[04_Domains/Check_Ins]]
- [[04_Domains/Direct_Messaging]]
- [[04_Domains/Events]]
- [[04_Domains/Goals]]
- [[04_Domains/Nutrition_Guidance]]
- [[04_Domains/Programs]]
- [[04_Domains/Progress_and_Adherence]]
- [[04_Domains/Todos_and_Habits]]
- [[04_Domains/Training_Sessions]]
- [[09_Runtime_Context/Athlete_Snapshot]]
- [[09_Runtime_Context/Data_Boundary]]
- [[09_Runtime_Context/Known_Context]]
- [[09_Runtime_Context/SESSION]]

## Knowledge

- [[05_Knowledge/Exercise_Library]]
- [[05_Knowledge/Exercise_Media_Catalog]]
- [[05_Knowledge/Fitness/Bodybuilding]]
- [[05_Knowledge/Fitness/Calisthenics]]
- [[05_Knowledge/Fitness/CrossFit]]
- [[05_Knowledge/Fitness/General]]
- [[05_Knowledge/Fitness/Powerlifting]]
- [[05_Knowledge/Form_Demos_By_Wedge]]
- [[05_Knowledge/Knowledge_System]]
- [[05_Knowledge/Sports/Basketball]]
- [[05_Knowledge/Sports/Combat]]
- [[05_Knowledge/Sports/Football]]
- [[05_Knowledge/Sports/Golf]]
- [[05_Knowledge/Sports/Padel]]
- [[05_Knowledge/Sports/Swimming]]
- [[05_Knowledge/Sports/Tennis]]
- [[05_Knowledge/Wellness/Rehab_and_Therapy]]
- [[05_Knowledge/Wellness/Yoga_and_Mind_Body]]

## Tools

- [[06_Tools/Adapt_Purchased_Program]]
- [[06_Tools/Add_Todo]]
- [[06_Tools/Approve_Program_Draft]]
- [[06_Tools/Browse_Programs]]
- [[06_Tools/Change_Plan_and_Credits]]
- [[06_Tools/Direct_Messaging_Capability]]
- [[06_Tools/Draft_Message]]
- [[06_Tools/Draft_Program]]
- [[06_Tools/Get_Account]]
- [[06_Tools/Get_Athlete_Profile]]
- [[06_Tools/Get_Athlete_Snapshot]]
- [[06_Tools/Get_Body_Map]]
- [[06_Tools/Get_Check_Ins]]
- [[06_Tools/Get_Connected_Clients]]
- [[06_Tools/Get_Current_Program]]
- [[06_Tools/Get_Events]]
- [[06_Tools/Get_Exercise_Catalog]]
- [[06_Tools/Get_Program_Library]]
- [[06_Tools/Get_Todos]]
- [[06_Tools/Get_Training_Sessions]]
- [[06_Tools/Log_Body_Report]]
- [[06_Tools/Manage_Events]]
- [[06_Tools/Manage_Trainer_Connection]]
- [[06_Tools/Manage_Training_Sessions]]
- [[06_Tools/Purchase_Program]]
- [[06_Tools/Report_Conversation]]
- [[06_Tools/Retrieve_Knowledge]]
- [[06_Tools/Save_Check_In]]
- [[06_Tools/Update_Assigned_Program]]
- [[06_Tools/Update_Athlete_Profile]]
- [[06_Tools/Update_or_Delete_Todo]]

## Workflows

- [[07_Workflows/Athlete_Check_In]]
- [[07_Workflows/Athlete_Onboarding]]
- [[07_Workflows/Body_Map_Response]]
- [[07_Workflows/Daily_Training]]
- [[07_Workflows/Intake_and_Journey_Rules]]
- [[07_Workflows/Program_Adjustment]]
- [[07_Workflows/Program_Generation]]
- [[07_Workflows/Trainer_Check_In_Analysis]]
- [[07_Workflows/Trainer_Client_Brief]]
- [[07_Workflows/Trainer_Client_Message_Draft]]
- [[07_Workflows/Trainer_Program_Draft]]
