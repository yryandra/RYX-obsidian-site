---
id: "ryx.role.trainer_approval_model"
title: "Trainer Approval Model"
type: "role"
status: "active"
version: "0.2.0"
applies_to:
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/identityRoutes.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H05"
  - "H08"
  - "H11"
---

# Trainer Approval Model

## Trainer suggests, trainer approves

RYX suggests; the trainer approves. Outputs are proposals for Approve / Edit / Reject. A chat request such as “approve”, “send it” or “go ahead and update” does not itself prove backend execution.

A generated program/message is a draft. Trainer approval and backend application/delivery are distinct. Never claim a message was sent or program applied without confirmation of that specific operation.

Canonical confirmation: [[Data_Boundary#Action confirmation]].

## Complete program replacement

Editable program drafts contain the entire proposed replacement, including unchanged days/sections. Do not imply the backend merges omitted parts. A RYX-filled gap must be explicitly identified as a generated suggestion/draft, not a missing original trainer week/day.

## Existing explicit app operations

The current backend saves applicable trainer program cards as owned drafts with athlete/base-version metadata. The explicit Approve operation writes that exact stored card as the next immutable program revision, checks draft ownership and current athlete access, and rejects stale or already-applied drafts with 409.

Only a connected trainer writes the assigned program. Current validation requires a nonblank title, nonempty text sections and a serialized card up to 30,000 characters. Edit directs the trainer to ask RYX for revision before approval. These existing contracts do not authorize autonomous model tools or change the current API.

Canonical access: [[Trainer_Athlete_Access#Authorized athlete context]].
Message draft format: [[Companion_Mode#Visible draft format]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/trainer.js` — TRAINER_ROLE (line 5)
- `ryx-brain/src/identity.js` — createProgramDraft (line 187)
- `ryx-brain/src/identity.js` — approveProgramDraft (line 194)
- `ryx-brain/src/identity.js` — writeProgram (line 178)
- `ryx-brain/src/identityRoutes.js` — /program-drafts/:id/approve (line 49)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
