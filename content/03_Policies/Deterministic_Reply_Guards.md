---
id: "ryx.policy.deterministic_reply_guards"
title: "Deterministic Reply Guards"
type: "policy"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/replyGuards.js"
  - "ryx-brain/src/runChat.js"
  - "ryx-brain/src/server.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H02"
  - "H03"
  - "H04"
  - "H05"
  - "H06"
  - "H07"
  - "H08"
---

# Deterministic Reply Guards

## Canonical enforcement requirements

This note specifies intended enforcement obligations for a future aligned pipeline. It is not a claim that replyGuards.js already implements them.

Canonical rules:
- [[Crisis_Handling#Terminal safety path]]
- [[Safety#Research statement and professional review]]
- [[Pain_and_Injury#Active pain and clearance]]
- [[Companion_Mode#Trainer ownership]]
- [[Companion_Mode#Visible draft format]]
- [[Trainer_Approval_Model#Trainer suggests, trainer approves]]
- [[Data_Boundary#Action confirmation]]
- [[Free_Pro_Entitlements#Entitlement matrix]]
- [[Credit_and_Tier_Rules#Final action and billing]]

## Final safety enforcement

After normal response coercion/formatting, enforce the complete visible output against the canonical safety rules. Crisis stays terminal, with no questions/cards/tasks/commerce reintroduced. Validate the full research sentence and its visible position before relevant guidance; preserve required referral separately. Card content, notes and lead must not bypass mode ownership, safety or confirmed execution.

## Existing behavior and alignment

The migrated guard triggers, conditional prefix checks, hardcoded crisis/leg-day messages and unscoped approval suffix are historical evidence in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]]. They no longer define competing canonical instructions. No regex, guard ordering, billing recalculation or runtime file has been modified in this phase.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/replyGuards.js` — Complete file (106 lines)
- `ryx-brain/src/runChat.js` — Complete file (119 lines)
- `ryx-brain/src/server.js` — Complete file (729 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
