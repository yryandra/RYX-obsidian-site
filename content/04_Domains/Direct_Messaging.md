---
id: "ryx.domain.direct_messaging"
title: "Direct Messaging"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/docs/shared-athlete-data.md"
  - "ryx-brain/src/directMessages.js"
  - "ryx-brain/src/liveEvents.js"
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H05"
  - "H08"
  - "H10"
---

# Direct Messaging

## Draft and delivery distinction

Canonical rule: [[Companion_Mode#Visible draft format]]; [[Trainer_Approval_Model#Trainer suggests, trainer approves]]; [[Data_Boundary#Action confirmation]].

RYX provides ready-to-review communication. Delivery is a separate explicit app action; an Athlete or Trainer saying “send it” in RYX chat is not evidence it was delivered.

## Existing backend contract

Both participants must be registered, have opposite athlete/trainer roles and an active relationship. History reads, sends and read receipts recheck access. Messages persist for offline recipients; authenticated SSE notifies inbox changes and clients fetch authorized records. Reconnection reconciles persisted messages.

Text is nonblank and at most 4,000 characters. kind is message or checkin. clientId is 1–80 word/hyphen characters; repeat sender/clientId with identical peer/content/kind is idempotent, conflicting reuse returns 409. History is 100 messages per page with before cursor. Inbox/history fetch alone does not mark read; the explicit read receipt does.

Revocation blocks access and logout invalidates the live stream. DM bodies are not automatically part of standard RYX SESSION or memory. No new sender, messaging permission, delivery automation or memory service is introduced.

## Canonical rule references

Canonical rule: [[Data_Boundary#Data truth precedence]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/docs/shared-athlete-data.md` — Complete file (138 lines)
- `ryx-brain/src/directMessages.js` — Complete file (83 lines)
- `ryx-brain/src/liveEvents.js` — Complete file (9 lines)
- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
