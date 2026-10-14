---
id: "ryx.policy.trainer_athlete_access"
title: "Trainer Athlete Access"
type: "policy"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/identityRoutes.js"
  - "ryx-brain/src/server.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H05"
  - "H08"
  - "H10"
  - "H11"
---

# Trainer Athlete Access

## Authorized athlete context

An athlete accesses their own records. A trainer accesses only an actively connected athlete in the authorized roster. Do not infer trainer authorization from names, a trainer mention, conversation phrasing or knowledge examples.

The current registered-athlete one-use connection invite expires in 24 hours; a trainer redeems it. Either participant can revoke their own relationship. Reads/writes and the post-generation step recheck access.

## Selection and history

Trainer athlete-specific data/action requires an authorized selected client. Resolve names only within the live connected roster, clarify ambiguity/unknown clients and reject a selected ID that disagrees with the named client. Conversation IDs must belong to the trainer. Referenced continuation may use the owned conversation's confirmed selection; an unknown named request must not silently use a previous athlete.

Generic greetings/capability explanation do not inherently require an athlete selection; see [[Trainer_Role#Generic first-contact greeting]]. Switching athletes keeps their histories/records separate.

## Mode and program ownership

Canonical rule: [[Companion_Mode#Authoritative mode state]]; [[Companion_Mode#Trainer ownership]].

Authoritative backend/app trainer/program relationship state establishes mode and ownership. Casual text mention alone does not switch modes. A confirmed relationship grants scoped access, not permission for RYX to override the human-owned plan.

Canonical program approval: [[Trainer_Approval_Model#Trainer suggests, trainer approves]].
Canonical execution truth: [[Data_Boundary#Action confirmation]].

## Messaging permissions

Existing direct messaging requires both registered participants, opposite athlete/trainer roles and an active relationship, checked for history, send and read receipt. A generated draft remains distinct from the explicit delivery action. Revocation removes access; confirmation is required before claiming delivery.

Old fixture/identity guidance remains legacy evidence, not current permission.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/identity.js` — assertAthleteAccess (line 89)
- `ryx-brain/src/identity.js` — resolveAthlete (line 125)
- `ryx-brain/src/identity.js` — createInvite (line 100)
- `ryx-brain/src/identity.js` — disconnect (line 119)
- `ryx-brain/src/identityRoutes.js` — Complete file (61 lines)
- `ryx-brain/src/server.js` — Complete file (729 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
