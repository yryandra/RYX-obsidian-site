---
id: "ryx.policy.memory_policy"
title: "Memory Policy"
type: "policy"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/labMemory.js"
  - "ryx-brain/src/labSessions.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H04"
  - "H06"
  - "H10"
  - "H12"
---

# Memory Policy

## Memory capability truth

Promise only implemented memory/context capabilities. Pro does not create an unlimited or durable trainer-style/client-note memory store. Tier depth in [[Free_Pro_Entitlements#Entitlement matrix]] does not change what has actually been persisted or supplied.

## Context categories

- Current conversation context: messages/context actually provided for this request.
- Recent conversation history: existing persisted trainer conversation turns selected for the owned conversation and athlete; the inspected loader supplies at most 24 turns and is not tier-dependent.
- Persisted RYX memory: only actual saved records supported by the backend. A separate durable preference/client-note memory service is not implemented in the inspected path.
- CORYX profile/data: persisted profiles, current program revisions and fresh authorized domain records, governed by [[Data_Boundary#Data truth precedence]].
- Future long-term preference memory: planned/unimplemented; not a current capability or subscription promise.

Use prior approved changes, client facts and style preferences only when they are actually present in authorized supplied context. Do not say history/preferences were loaded, remembered indefinitely or saved without confirmation.

## Existing persistence and limitations

The existing saved profile whitelist includes goal, goalPrimary, goalSecondary, level, equipment, daysPerWeek, schedule, injuries, sport, trainingFocus, category, specialization, experience and lastFunnelGapId, with a 10,000-character serialized cap. Trainer turns and assigned program revisions persist separately. Other inferred intake fields are not thereby a durable memory record.

Snapshot formatter caps and appended records are described in [[Athlete_Snapshot]]. Lab scores/assumption logs are diagnostics, not production memory facts or personas.

Canonical inference and confirmation rules: [[Data_Boundary#Inference boundaries]]; [[Data_Boundary#Action confirmation]].

## Future alignment

Remove unsupported long-term style/client-note promises from prompt/tier copy and make supplied context/persistence truthful. No preference store, retention policy, client-note save route or memory service is implemented by this phase.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/trainer.js` — TRAINER_FREE (line 150)
- `ryx-brain/src/prompts/trainer.js` — TRAINER_PAID (line 167)
- `ryx-brain/src/prompts/core.js` — CONTEXT_AND_CONTROL (line 109)
- `ryx-brain/src/identity.js` — trainerHistory (line 157)
- `ryx-brain/src/identity.js` — saveProfile (line 81)
- `ryx-brain/src/labMemory.js` — Complete file (929 lines)
- `ryx-brain/src/labSessions.js` — Complete file (345 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
