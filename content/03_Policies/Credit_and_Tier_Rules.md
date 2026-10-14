---
id: "ryx.policy.credit_and_tier_rules"
title: "Credit and Tier Rules"
type: "policy"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/credits.js"
  - "ryx-brain/src/accounts.js"
  - "ryx-brain/src/runChat.js"
  - "ryx-brain/src/openaiRun.js"
  - "ryx-brain/src/server.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H06"
  - "H07"
---

# Credit and Tier Rules

## Action weights

Preserve the existing source-defined action pricing:
- quick_question: 1
- exercise_explanation: 2
- modify_workout: 2
- generate_workout: 4
- analyse_performance: 4
- meal_plan: 4
- major_adjustment: 5
- weekly_plan: 8
- image_analysis: 10
- advanced_multistep: 12

Unknown action falls back to quick_question. Credits are action-weighted, not a flat per-message cost. Do not expose dollar-per-credit economics to users. A priced action is not proof that an unimplemented input/capability is available.

## Allowances and wording

Free: existing implemented 30 credits per fixed 30-day cycle, without rollover.
Pro: 600 credits per fixed 30-day cycle, with up to 100 unused nonnegative credits rolled over.

Describe Pro as metered. Do not promise an unbounded balance. Pricing and action weights are unchanged. Current plan-switch/top-up rules remain implementation facts, not verified payment or a new commercial model: upgrade balance becomes at least 600; downgrade caps it at 30; valid positive top-ups add credits.

Canonical tier depth: [[Free_Pro_Entitlements#Entitlement matrix]].

## Final action and billing

THE FINAL EXECUTED/BILLED ACTION determines the final credit cost.

Future sequence:
request → determine intended action → model/guards/coercion → determine FINAL action → determine FINAL cost → verify balance → charge once → persist ledger entry.

Pre-estimates can support routing; they do not replace final-action costing and balance verification. Every action change through safety/guards/coercion must be reflected in the final cost. The future ledger is a requirement from H07, not a current implemented capability.

## Current-runtime mismatch

The current model/pre-check/guard/funnel/coercion stages can leave action and cost inconsistent, and the server floors deductions without a second final-cost affordability check. C11/C18 remain unchanged in the migration review.

Future alignment includes envelope.js, accounts.js, credits.js, runChat.js, openaiRun.js, replyGuards.js, profileFunnel.js, server.js and the Lab path. No billing, ledger, credit implementation or runtime behavior is changed here.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/credits.js` — Complete file (98 lines)
- `ryx-brain/src/accounts.js` — Complete file (178 lines)
- `ryx-brain/src/runChat.js` — Complete file (119 lines)
- `ryx-brain/src/openaiRun.js` — Complete file (101 lines)
- `ryx-brain/src/server.js` — Complete file (729 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
