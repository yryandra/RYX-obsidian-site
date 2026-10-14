---
id: "ryx.runtime.context.session"
title: "SESSION"
type: "runtime-context"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/buildSystemPrompt.js"
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "ryx-brain/src/runChat.js"
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
  - "H08"
  - "H10"
  - "H12"
---

# SESSION

## Runtime context, not permanent brain knowledge

SESSION is live request context supplied by the shared backend. It contains no permanent user record to store in Obsidian. Its content obeys [[Data_Boundary#Data truth precedence]] and the instruction hierarchy in [[Brain_Architecture#Global instruction precedence]].

## Required facts and optional context

Authenticated role/identity, account-derived tier/credits, authorized athlete/client context, authoritative mode/ownership and action-critical permissions come from confirmed backend/app state. A trainer mention does not switch modes or grant access.

Profile information, training log, todos, check-ins, event countdown, body reports, current program, conversation context and relevant retrieved knowledge are supplied when available. Unknown facts remain unknown; inference is labelled separately and cannot silently establish ownership, clearance, equipment or records.

## Request-specific sufficiency

Canonical rule: [[Response_Principles#Request-specific sufficiency and deliver-first]].

Open gaps, completeness percentage and next-funnel-step metadata describe current profile coverage, not a universal delivery gate. Only missing safety/correctness/permission/operation-critical context blocks the particular request. Pro delivery remains first; Free generation depth follows the central matrix.

Generic trainer greetings do not require client selection. Athlete-specific reads/actions do; see [[Trainer_Role#Generic first-contact greeting]].

## Safety and current program

Canonical rules: [[Crisis_Handling#Terminal safety path]]; [[Safety#Research statement and professional review]]; [[Companion_Mode#Trainer ownership]].

Fresh authorized athlete records and the current assigned program take precedence over stale chat within data rules. Original body reporting scales survive formatting. Safety can require review of a current pain signal even if prior profile context says no injury.

## Knowledge and output

Retrieved units follow [[Knowledge_System#Future retrieval contract]] and cannot override safety, authorization, role/mode or tier. Cards/formatting cannot hide required safety text. Conversation memory is limited to actual supplied/persisted context under [[Memory_Policy#Memory capability truth]].

Current renderer order, default modes, heuristic profile extraction and hint/gate behavior remain historical/current implementation in C01/C06/C15/C19/C21. The future runtime must align; no prompt assembly or loader changes are applied.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/buildSystemPrompt.js` — Complete file (250 lines)
- `ryx-brain/src/server.js` — Complete file (729 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)
- `ryx-brain/src/runChat.js` — Complete file (119 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
