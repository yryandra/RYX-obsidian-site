---
id: "ryx.release.0.1.0"
title: "RYX Brain v0.1.0"
type: "release"
status: "active"
version: "0.1.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/buildSystemPrompt.js"
  - "ryx-brain/src/envelope.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "RYX_Wedge_Knowledge_Bases_v1/index.json"
last_reviewed: "2026-10-13"
---

# RYX Brain v0.1.0

RYX Brain v0.1.0 is a faithful extracted knowledge/behavior snapshot reviewed on 2026-10-13. This is a manifest, not a concatenated prompt or runtime loader. Original CORE/role/tier blocks retain their wording; domain/tool/workflow projections may repeat those rules for navigation. The migration review records conflicts without silently resolving them.

## Core

- [[01_Core/RYX_Identity|RYX Identity]]
- [[01_Core/Personality_and_Voice|Personality and Voice]]
- [[01_Core/Response_Principles|Response Principles]]
- [[01_Core/Brain_Architecture|Brain Architecture]]
- [[01_Core/Output_and_Card_Behaviour|Output and Card Behaviour]]

## Roles

- [[02_Roles/Athlete/Athlete_Role|Athlete Role]]
- [[02_Roles/Athlete/Solo_Mode|Solo Mode]]
- [[02_Roles/Athlete/Companion_Mode|Companion Mode]]
- [[02_Roles/Athlete/Athlete_Free|Athlete Free]]
- [[02_Roles/Athlete/Athlete_Pro|Athlete Pro]]
- [[02_Roles/Trainer/Trainer_Role|Trainer Role]]
- [[02_Roles/Trainer/Trainer_Outputs|Trainer Outputs]]
- [[02_Roles/Trainer/Trainer_Approval_Model|Trainer Approval Model]]
- [[02_Roles/Trainer/Trainer_Free|Trainer Free]]
- [[02_Roles/Trainer/Trainer_Pro|Trainer Pro]]

## Policies

- [[03_Policies/Safety|Safety]]
- [[03_Policies/Pain_and_Injury|Pain and Injury]]
- [[03_Policies/Crisis_Handling|Crisis Handling]]
- [[03_Policies/Referral_Rules|Referral Rules]]
- [[03_Policies/Data_Access|Data Access]]
- [[03_Policies/Trainer_Athlete_Access|Trainer Athlete Access]]
- [[03_Policies/Memory_Policy|Memory Policy]]
- [[03_Policies/RYX_Boundaries|RYX Boundaries]]
- [[03_Policies/Deterministic_Reply_Guards|Deterministic Reply Guards]]
- [[03_Policies/Credit_and_Tier_Rules|Credit and Tier Rules]]

## Domains

- [[04_Domains/Athlete_Profile|Athlete Profile]]
- [[04_Domains/Check_Ins|Check Ins]]
- [[04_Domains/Training_Sessions|Training Sessions]]
- [[04_Domains/Programs|Programs]]
- [[04_Domains/Body_Map|Body Map]]
- [[04_Domains/Todos_and_Habits|Todos and Habits]]
- [[04_Domains/Goals|Goals]]
- [[04_Domains/Events|Events]]
- [[04_Domains/Progress_and_Adherence|Progress and Adherence]]
- [[04_Domains/Direct_Messaging|Direct Messaging]]
- [[04_Domains/Nutrition_Guidance|Nutrition Guidance]]
- [[04_Domains/Body_Region_Catalog|Body Region Catalog]]

## Knowledge

- [[05_Knowledge/Fitness/General|General fitness]]
- [[05_Knowledge/Fitness/Bodybuilding|Bodybuilding]]
- [[05_Knowledge/Fitness/Calisthenics|Calisthenics]]
- [[05_Knowledge/Fitness/CrossFit|CrossFit]]
- [[05_Knowledge/Fitness/Powerlifting|Powerlifting]]
- [[05_Knowledge/Sports/Football|Football]]
- [[05_Knowledge/Sports/Basketball|Basketball]]
- [[05_Knowledge/Sports/Swimming|Swimming]]
- [[05_Knowledge/Sports/Padel|Padel]]
- [[05_Knowledge/Sports/Tennis|Tennis]]
- [[05_Knowledge/Sports/Golf|Golf]]
- [[05_Knowledge/Sports/Combat|Combat sports]]
- [[05_Knowledge/Wellness/Rehab_and_Therapy|Rehab & therapy]]
- [[05_Knowledge/Wellness/Yoga_and_Mind_Body|Yoga & mind-body]]
- [[05_Knowledge/Knowledge_System|Knowledge System]]
- [[05_Knowledge/Exercise_Library|Exercise Library]]
- [[05_Knowledge/Exercise_Media_Catalog|Exercise Media Catalog]]
- [[05_Knowledge/Form_Demos_By_Wedge|Form Demos by Wedge]]
- [[05_Knowledge/Wedge_Index|Wedge Index]]
- [[05_Knowledge/Wedge_Routing_Reference|Wedge Routing Reference]]
- [[05_Knowledge/Exercise_Media_Rules|Exercise Media Rules]]
- [[05_Knowledge/Marketplace_Program_Templates|Marketplace Program Templates]]

## Tools

- [[06_Tools/Get_Athlete_Profile|Get Athlete Profile]]
- [[06_Tools/Update_Athlete_Profile|Update Athlete Profile]]
- [[06_Tools/Get_Athlete_Snapshot|Get Athlete Snapshot]]
- [[06_Tools/Get_Connected_Clients|Get Connected Clients]]
- [[06_Tools/Manage_Trainer_Connection|Manage Trainer Connection]]
- [[06_Tools/Get_Check_Ins|Get Check Ins]]
- [[06_Tools/Save_Check_In|Save Check In]]
- [[06_Tools/Get_Training_Sessions|Get Training Sessions]]
- [[06_Tools/Manage_Training_Sessions|Manage Training Sessions]]
- [[06_Tools/Get_Current_Program|Get Current Program]]
- [[06_Tools/Draft_Program|Draft Program]]
- [[06_Tools/Update_Assigned_Program|Update Assigned Program]]
- [[06_Tools/Approve_Program_Draft|Approve Program Draft]]
- [[06_Tools/Get_Body_Map|Get Body Map]]
- [[06_Tools/Log_Body_Report|Log Body Report]]
- [[06_Tools/Get_Todos|Get Todos]]
- [[06_Tools/Add_Todo|Add Todo]]
- [[06_Tools/Update_or_Delete_Todo|Update or Delete Todo]]
- [[06_Tools/Get_Events|Get Events]]
- [[06_Tools/Manage_Events|Manage Events]]
- [[06_Tools/Browse_Programs|Browse Programs]]
- [[06_Tools/Get_Program_Library|Get Program Library]]
- [[06_Tools/Purchase_Program|Purchase Program]]
- [[06_Tools/Adapt_Purchased_Program|Adapt Purchased Program]]
- [[06_Tools/Draft_Message|Draft Message]]
- [[06_Tools/Direct_Messaging_Capability|Direct Messaging Capability]]
- [[06_Tools/Get_Account|Get Account]]
- [[06_Tools/Change_Plan_and_Credits|Change Plan and Credits]]
- [[06_Tools/Report_Conversation|Report Conversation]]
- [[06_Tools/Retrieve_Knowledge|Retrieve Knowledge]]
- [[06_Tools/Get_Exercise_Catalog|Get Exercise Catalog]]

## Workflows

- [[07_Workflows/Intake_and_Journey_Rules|Intake and Journey Rules]]
- [[07_Workflows/Athlete_Onboarding|Athlete Onboarding]]
- [[07_Workflows/Athlete_Check_In|Athlete Check In]]
- [[07_Workflows/Daily_Training|Daily Training]]
- [[07_Workflows/Program_Generation|Program Generation]]
- [[07_Workflows/Program_Adjustment|Program Adjustment]]
- [[07_Workflows/Body_Map_Response|Body Map Response]]
- [[07_Workflows/Trainer_Client_Brief|Trainer Client Brief]]
- [[07_Workflows/Trainer_Check_In_Analysis|Trainer Check In Analysis]]
- [[07_Workflows/Trainer_Program_Draft|Trainer Program Draft]]
- [[07_Workflows/Trainer_Client_Message_Draft|Trainer Client Message Draft]]

## Runtime Context

- [[09_Runtime_Context/SESSION|SESSION]]
- [[09_Runtime_Context/Athlete_Snapshot|Athlete Snapshot]]
- [[09_Runtime_Context/Known_Context|Known Context]]
- [[09_Runtime_Context/Data_Boundary|Data Boundary]]

Reference evaluations, legacy inactive playbooks, migration/admin guides, drafts/archive and historical outputs are excluded. Runtime context notes contribute interpretation/schema rules only; no runtime values are part of the release.

## Source reference

- `ryx-brain/src/prompts/core.js` — Complete file (147 lines)
- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/buildSystemPrompt.js` — Complete file (250 lines)
- `ryx-brain/src/envelope.js` — Complete file (401 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)
- `RYX_Wedge_Knowledge_Bases_v1/index.json` — Complete file (107 lines)

[[00_HOME|Back to the RYX Brain home]]
