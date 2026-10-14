---
id: "ryx.policy.data_access"
title: "Data Access"
type: "policy"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/identityRoutes.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/server.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H04"
  - "H05"
  - "H08"
---

# Data Access

## Authenticated identity and access

Current authenticated CORYX identity and relationship checks are the canonical direction. Role and actor identity come from authenticated backend state, not a display name, localStorage identifier, fixture reference or user-supplied role claim.

Legacy domain routes remain self-service: supplied userId must match the actor. Cross-user athlete reads use checked snapshot/program access; cross-user program writes use the connected-trainer operation. Tier and credit balance are account-derived.

Canonical access: [[Trainer_Athlete_Access#Authorized athlete context]].
Canonical data truth: [[Data_Boundary#Data truth precedence]].

## Confirmed execution

Canonical rule: [[Data_Boundary#Action confirmation]].

Permission, a generated draft and execution are distinct. Backend confirmation is needed before claims of sends, writes, saves or completed tasks. Recommending contact with support is allowed within scope; claiming support was contacted requires execution confirmation.

## Current restrictions and legacy material

Ordinary product endpoints require authenticated identity. Diagnostic report listing and knowledge stats are not ordinary user capabilities; Lab's local same-origin exception outside production is a developer implementation boundary, not no-auth access guidance.

Old fixture/localStorage/no-auth instructions are legacy/reference_only historical evidence in the archived snapshot and migration findings C12/C13. They are not canonical access instructions. No auth, API, database or role behavior is changed here.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/core.js` — CONTEXT_AND_CONTROL (line 109)
- `ryx-brain/src/identityRoutes.js` — Complete file (61 lines)
- `ryx-brain/src/identity.js` — assertAthleteAccess (line 89)
- `ryx-brain/src/server.js` — req.actor.role (line 501)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
