---
id: "ryx.navigation.tools"
title: "RYX Backend Capabilities"
type: "tool"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/identityRoutes.js"
  - "ryx-brain/src/runChat.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
---

# RYX backend capabilities

These notes describe existing backend/app contracts and intended canonical constraints requiring future alignment. Current chat has no registered autonomous model function-calling tools. A draft, approval and backend execution are distinct.

Canonical rules: [[Brain_Architecture#Global instruction precedence]]; [[Data_Boundary#Action confirmation]]; [[Free_Pro_Entitlements#Entitlement matrix]].

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

## Source reference

- `ryx-brain/src/server.js`
- `ryx-brain/src/identityRoutes.js`
- `ryx-brain/src/runChat.js`

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
