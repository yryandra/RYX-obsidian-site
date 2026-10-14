---
id: "ryx.tool.approve_program_draft"
title: "Approve Program Draft"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "trainer"
source_files:
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/identityRoutes.js"
  - "ryx-landing/src/lib/identityApi.js"
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
  - "H07"
  - "H08"
  - "H10"
  - "H11"
  - "H12"
---

# Approve Program Draft

## Contract and rule authority

The contract below describes an existing app/backend capability; canonical intended constraints are owned by [[Brain_Architecture#Global instruction precedence]], [[Data_Access#Authenticated identity and access]], [[Data_Boundary#Data truth precedence]], [[Data_Boundary#Action confirmation]], [[Response_Principles#Request-specific sufficiency and deliver-first]], [[Free_Pro_Entitlements#Entitlement matrix]], [[Companion_Mode#Trainer ownership]], [[Trainer_Approval_Model#Trainer suggests, trainer approves]], [[Safety#Research statement and professional review]], [[Crisis_Handling#Terminal safety path]] and [[Athlete_Profile#Confirmed equipment]].

Current implementation limitations do not override those owners. A generic trainer greeting is independent of client selection; athlete-specific operations still require authorization. No absent ledger, memory, medical-clearance inference or autonomous model tool is promised.

# Approve Program Draft

## Purpose

Apply the exact saved server draft after explicit trainer approval.

## When RYX Uses It

Trainer presses the app Approve action.

## Inputs

Authenticated draft owner; draftId.

## Output

Next program revision with exact draft card.

## Permissions

Draft-owning connected trainer; relation rechecked.

## Constraints

Uses stored draft/base version; cannot substitute edited client content in approve call. Chat approval wording alone has no effect.

## Failure Behaviour

404 foreign/missing draft; 403 revoked access; 409 already applied/stale. Reload/revise before approval.

## Related Brain Rules

[[Trainer_Approval_Model]]

## Implementation Source

POST /api/ryx/program-drafts/:id/approve; approveProgramDraft; approveDraft frontend wrapper.

This is an app/backend capability. The inspected chat model has no registered function-calling tools; it may explain/request a user action but cannot invoke this autonomously.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/src/identityRoutes.js` — Complete file (61 lines)
- `ryx-landing/src/lib/identityApi.js` — Complete file (83 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
