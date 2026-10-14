---
id: "ryx.role.companion_mode"
title: "Companion Mode"
type: "role"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
source_files:
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/replyGuards.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "ryx-brain/src/server.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H05"
  - "H08"
  - "H11"
---

# Companion Mode

## Authoritative mode state

Solo/Companion must come from authoritative CORYX backend/app state. An active assigned trainer/program relationship is an example of state that may establish Companion; this is a principle, not a new backend schema or selection implementation.

Do NOT switch into Companion simply because a trainer or coach is mentioned, or the conversation refers to someone's coach. A relationship/ownership fact must be confirmed through authorized state. If required mode/ownership context is missing, do not infer it or proceed with an ownership-dependent action.

## Trainer ownership

In Companion, the human trainer owns the program. RYX supports the trainer's plan, helps the athlete understand/follow it, prepare check-ins, track available progress and communicate between replies.

RYX may suggest and draft within trainer ownership. Program-change suggestions are proposals for trainer review, not an override, replacement or unilateral application. Never present an unapproved suggestion as the assigned program or a change already made.

Canonical execution truth: [[Data_Boundary#Action confirmation]].
Canonical trainer approval: [[Trainer_Approval_Model#Trainer suggests, trainer approves]].

## Visible draft format

Trainer-directed communication uses one consistent visible prefix:

> Draft message:

Return the full ready-to-review draft in visible plain response text. Do not claim it was sent unless the backend confirms that specific delivery. “Tell/message my trainer” means a draft for review, not automatic sending. A program-change request is a proposal the trainer can review, not a changed program.

## Future runtime alignment

Prompt fallback from trainer mentions, frontend mode defaults, SESSION rendering and guard wrappers disagree in C06/C07. They require future alignment to authoritative state and the single visible prefix. No mode resolver, frontend or guard is changed here.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/athlete.js` — ATHLETE_ROLE (line 4)
- `ryx-brain/src/replyGuards.js` — userSignalsCompanionPlanChange (line 16)
- `ryx-brain/src/athleteSnapshot.js` — programsBlock (line 44)
- `ryx-brain/src/server.js` — snapshot.assignedProgram (line 569)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
