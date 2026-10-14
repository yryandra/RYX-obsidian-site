---
id: "ryx.policy.crisis_handling"
title: "Crisis Handling"
type: "policy"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/replyGuards.js"
  - "ryx-brain/src/profileFunnel.js"
  - "ryx-brain/src/server.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H02"
---

# Crisis Handling

## Terminal safety path

CRISIS HANDLING IS A TERMINAL SAFETY PATH.

Immediate self-harm signals, suicidal ideation or mental-health crisis require stopping the normal fitness/coaching flow. Preserve the original scope, including concerning hopelessness statements; a narrow phrase matcher is not the whole policy.

Once triggered:
- stop ordinary fitness/coaching flow;
- do not run intake questions;
- do not generate workout/program cards or tasks;
- do not upsell, refer to commerce or suggest products;
- do not append unrelated questions or a normal coaching sign-off;
- do not return to normal coaching within the same response;
- allow no lower-priority rule to change the crisis response.

## Response expectations

Prioritize immediate safety and appropriate urgent support with concise, calm and caring language. Preserve the existing short 2–4-sentence expectation: urge immediate emergency/crisis/trusted-person support and make clear that a fitness assistant cannot handle the crisis. Do not prescribe training, discuss unnecessary fitness details or attempt crisis counseling. Do not end with a coaching question.

This defines response behavior; it does not add a new crisis-counseling or emergency-service capability.

## Future final safety enforcement

The future runtime requires a final safety enforcement stage AFTER all normal response coercion, including intake/funnel, card repair and final formatting. It must preserve the terminal path and prevent lower-priority content from being appended or reintroduced. An emergency keyword alone is not proof that the full output meets the policy.

Production runtime: NOT YET ALIGNED. No guard/server changes are made here. C02/C03 remain in [[MIGRATION_REVIEW]]; exact historical fallback text is retained in [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/core.js` — SAFETY (line 68)
- `ryx-brain/src/replyGuards.js` — userSignalsCrisis (line 12)
- `ryx-brain/src/replyGuards.js` — applyReplyGuards (line 29)
- `ryx-brain/src/profileFunnel.js` — Complete file (638 lines)
- `ryx-brain/src/server.js` — Complete file (729 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
