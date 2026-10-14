---
id: "ryx.eval.eval_system"
title: "Eval System"
type: "eval"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/eval.js"
  - "ryx-brain/src/evalOpenai.js"
  - "ryx-brain/src/labSessions.js"
  - "ryx-brain/src/labInsights.js"
  - "ryx-brain/test/shared-ryx.test.js"
  - "ryx-brain/test/messaging.test.js"
  - "ryx-brain/package.json"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
decision_ids:
  - "H01"
  - "H02"
  - "H03"
  - "H04"
  - "H05"
  - "H06"
  - "H07"
  - "H08"
  - "H09"
  - "H10"
  - "H11"
  - "H12"
---

# Eval System

## Production-quality evaluation contract

Production-quality RYX evaluation must eventually exercise the COMPLETE user-visible pipeline:
brain prompt → runtime context → retrieval → model output → deterministic guards → funnel/intake → card coercion → final formatting → final safety enforcement.

Include relevant authorization/mode/tier, app-confirmed execution and final-action/cost assertions where the tested request uses them. Raw provider output alone is not proof of production behavior.

## Current tests and their limits

The existing Anthropic evaluator requests a raw provider reply and bypasses retrieval, structured envelope and guards/server processing. The OpenAI-named evaluator calls runRyxChat but does not reproduce all server/Lab postprocessing; configured provider selection can differ. Existing research gates check a prefix, and Lab diagnostic wording can pass without the full exact sentence/order. No current result from those paths is labelled full-pipeline proof here.

Existing isolated HTTP tests cover identity, shared context, named/pronoun selection, program approval/version conflicts, revocation, DM/offline/read-receipt behavior and persistence with an injected model. They remain unchanged. No paid/live-model run is performed in this phase.

## Canonical candidate acceptance

- A request with sufficient required context gets useful tier-appropriate output despite unrelated incomplete profile fields.
- Crisis stays terminal after every normal processing stage; no question/card/task/commerce reappears.
- The full canonical research sentence is visible before relevant guidance, and required referral is independent of prefix presence or note locking.
- Active-pain clearance is not inferred from weak mentions or thread defaults.
- Casual trainer/coach mention does not establish mode or authorization; backend/app state does.
- Free gets the central matrix's visible useful basic output; Pro-only detail is not generated-and-hidden for Free.
- Credit wording and final action/cost follow the existing source weights and intended final balance/charge/ledger sequence.
- Generic trainer greeting is independent of athlete selection; athlete-specific access/action is scoped.
- Memory claims match actual supplied/persisted capabilities.
- Equipment prescriptions and missing program content obey confirmed context and explicit draft labelling.
- Original body reporting scales and the 34-zone schema are preserved; past-active-event meaning is most recent past date.
- Retrieval units preserve stable source/claim provenance, caveats and safety constraints.

These are future full-pipeline acceptance expectations from H01–H12, not assertions that current source already passes them.

## Existing scenario evidence

[[Athlete_Scenarios]], [[Trainer_Scenarios]], [[Exercise_Media_Scenarios]] and the original [[Coverage]] remain reference_only evaluation evidence. Original IDs/user/should/accept texts survive. Existing fixture/profile values remain excluded from the vault; fixture-backed replay requires external original setup.

Historical expected text that conflicts with v0.2.0 does not override the decision record. A future implementation should add/update test expectations explicitly with provenance rather than count old raw-model checks as successful canonical validation.

## Source reference

- `ryx-brain/src/eval.js` — Complete file (190 lines)
- `ryx-brain/src/evalOpenai.js` — Complete file (212 lines)
- `ryx-brain/src/labSessions.js` — Complete file (345 lines)
- `ryx-brain/src/labInsights.js` — Complete file (234 lines)
- `ryx-brain/test/shared-ryx.test.js` — Complete file (212 lines)
- `ryx-brain/test/messaging.test.js` — Complete file (144 lines)
- `ryx-brain/package.json` — Complete file (32 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
