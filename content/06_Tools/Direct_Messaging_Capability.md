---
id: "ryx.tool.direct_messaging_capability"
title: "Direct Messaging Capability"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/directMessages.js"
  - "ryx-brain/src/liveEvents.js"
  - "ryx-brain/src/identityRoutes.js"
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

# Direct Messaging Capability

## Contract and rule authority

The contract below describes an existing app/backend capability; canonical intended constraints are owned by [[Brain_Architecture#Global instruction precedence]], [[Data_Access#Authenticated identity and access]], [[Data_Boundary#Data truth precedence]], [[Data_Boundary#Action confirmation]], [[Response_Principles#Request-specific sufficiency and deliver-first]], [[Free_Pro_Entitlements#Entitlement matrix]], [[Companion_Mode#Trainer ownership]], [[Trainer_Approval_Model#Trainer suggests, trainer approves]], [[Safety#Research statement and professional review]], [[Crisis_Handling#Terminal safety path]] and [[Athlete_Profile#Confirmed equipment]].

Current implementation limitations do not override those owners. A generic trainer greeting is independent of client selection; athlete-specific operations still require authorization. No absent ledger, memory, medical-clearance inference or autonomous model tool is promised.

# Direct Messaging Capability

## Purpose

Deliver persistent user-sent messages and read receipts, read authorized inbox/history.

## When RYX Uses It

User explicitly sends a reviewed message in DM; RYX draft itself remains unsent.

## Inputs

peerId; text,kind,clientId for send; before for paging; throughId for receipt.

## Output

Saved message; inbox items/unread counts; pageditems/hasMore; read confirmation; inbox-only SSE notifications.

## Permissions

Both registered, opposite roles and active relationship; auth refreshed on live events/heartbeats.

## Constraints

Nonblank text <=4000; kind message/checkin; clientId 1–80 word/hyphen characters; idempotent retries; 100/page. History reads do not mark read. RYX SESSION does not automatically include DM bodies.

## Failure Behaviour

401 auth/revoked login; 403 peer/relationship; 400 invalid payload/cursor; 409 reused ID with different content. Persisted messages survive offline recipients.

## Related Brain Rules

[[Direct_Messaging]] · [[Trainer_Approval_Model]] · [[Memory_Policy]]

## Implementation Source

GET /messages/inbox,/messages/stream,/messages/:peerId; POST /messages/:peerId,/messages/:peerId/read.

This is an app/backend capability. The inspected chat model has no registered function-calling tools; it may explain/request a user action but cannot invoke this autonomously.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/directMessages.js` — Complete file (83 lines)
- `ryx-brain/src/liveEvents.js` — Complete file (9 lines)
- `ryx-brain/src/identityRoutes.js` — Complete file (61 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
