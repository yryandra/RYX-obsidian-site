---
id: "ryx.core.brain_architecture"
title: "Brain Architecture"
type: "core"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/buildSystemPrompt.js"
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/runChat.js"
  - "ryx-brain/src/openaiRun.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "package.json"
  - "scripts/dev.mjs"
  - "web/src/pages/CoachPage.jsx"
  - "web/src/lib/brainHealth.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H02"
  - "H05"
  - "H07"
  - "H08"
  - "H12"
---

# Brain Architecture

## Global instruction precedence

Higher-priority rules always win. Lower-priority content must never weaken or override higher-priority rules.

1. Safety
2. Authentication, authorization and data-access rules
3. Core RYX rules
4. Role rules — Athlete; Trainer
5. Mode rules — Solo; Companion
6. Tier rules — Free; Pro
7. Domain and workflow rules
8. Tool-use instructions
9. Retrieved knowledge
10. Examples, presentation and response formatting

Body Map cannot override active-pain safety. Response formatting cannot override terminal crisis handling. Retrieved sports knowledge cannot override CORYX access permissions. Tier behavior cannot override safety. A card instruction cannot hide a mandatory safety statement.

## Brain and live context

Obsidian holds RYX knowledge, instructions and intended behavior. RYX, CMS and iOS are intended to use one shared CORYX backend/API and database. Live application/user records remain outside the vault.

RYX combines canonical brain instructions with authorized live CORYX context to produce a response or proposal. An output draft, human approval and backend-confirmed execution are distinct stages.

Canonical rule: [[Data_Boundary#Data truth precedence]].
Canonical rule: [[Response_Principles#Request-specific sufficiency and deliver-first]].

## Prompt composition and precedence are different

The existing runtime assembles CORE → ROLE → TIER → SESSION → RESPONSE_DIRECTIVE, with conversation messages supplied separately. Its storage remains SQLite plus legacy domain JSON. This is a description of current implementation, not a new hierarchy or proof of Obsidian integration.

A future compiler must apply the instruction hierarchy above even when the physical prompt order differs. Compile canonical ownership once; linked topic projections must not become repeated independent authorities. Knowledge units must retain provenance under [[Knowledge_System#Future retrieval contract]].

## Intended response and safety pipeline

Request → authenticated identity and authorized context → request-specific sufficiency → canonical instructions and relevant knowledge → model output → normal guards/intake/card coercion/formatting → final safety enforcement → determine final action and cost → verify balance → charge once and persist the ledger entry.

Crisis handling is a terminal safety path: once triggered, ordinary coaching, intake, cards and commerce cannot resume or alter that response. The future runtime needs final safety enforcement AFTER all normal response coercion. The charging sequence is an intended future contract; no ledger or pipeline changes have been implemented.

Canonical rules: [[Crisis_Handling#Terminal safety path]]; [[Credit_and_Tier_Rules#Final action and billing]].

## Historical audit and candidate

[[RYX_Brain_v0.1.0]] is the unchanged migration manifest. Exact pre-review note text is retained in [[RYX_Brain_v0.1.0_Notes_Snapshot]]. [[MIGRATION_REVIEW]] and [[MIGRATION_MAP]] remain unchanged.

[[RYX_Brain_v0.2.0]] defines reviewed intended behavior. [[RYX_BRAIN_DECISIONS]] records the approved H01–H12 decisions and required future runtime alignment. Runtime status: NOT YET INTEGRATED.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/buildSystemPrompt.js` — buildSystemPrompt (line 21)
- `ryx-brain/src/server.js` — app.post('/api/ryx/chat' (line 498)
- `ryx-brain/src/runChat.js` — Complete file (119 lines)
- `ryx-brain/src/openaiRun.js` — Complete file (101 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)
- `package.json` — Complete file (16 lines)
- `scripts/dev.mjs` — Complete file (24 lines)
- `web/src/pages/CoachPage.jsx` — Complete file (34 lines)
- `web/src/lib/brainHealth.js` — Complete file (12 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
