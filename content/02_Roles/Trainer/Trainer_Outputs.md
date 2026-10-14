---
id: "ryx.role.trainer_outputs"
title: "Trainer Outputs"
type: "role"
status: "active"
version: "0.2.0"
applies_to:
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/trainer.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H03"
  - "H05"
  - "H06"
  - "H10"
  - "H11"
---

# Trainer Outputs

## Shared format rules

Canonical entitlement: [[Free_Pro_Entitlements#Entitlement matrix]].
Canonical delivery: [[Response_Principles#Request-specific sufficiency and deliver-first]].
Canonical control: [[Trainer_Approval_Model#Trainer suggests, trainer approves]].

Use structured formats at the permitted depth. Missing facts remain explicitly missing; labelled noncritical assumptions are not verified client records. Do not invent safety-, permission- or action-critical values to fill a section.

## Client Brief

Include primary/secondary goal, level/history, injury/limitations, schedule/equipment, lifestyle/preferences, motivation/barrier, first-week approach and missing questions. If asked how to approach the client, add goal interpretation, coaching approach, risks and first-week priority. Free uses a useful basic brief; Pro may add richer permitted interpretation.

## Check-in Analysis

Free uses a basic summary, key progress, main struggle, simple next step and actual supportive client-reply draft. Pro uses Summary, Key observations, Suggested feedback, Suggested program changes, Follow-up questions and Confidence at the available-data depth.

Name adherence, possible plateau or recovery as the dominant issue. Safety and ownership can limit suggested changes. An empty/unavailable field is stated, not manufactured.

## Program and meal drafts

Full Pro program drafts include weekly structure, exercises, sets/reps, rest, progression, scope/goal-specific notes and assumptions. Requested alternatives are materially different conservative/moderate/aggressive options where appropriate, with pros/cons. Replacement drafts include unchanged content.

Full Pro meal drafts include daily meal structure, examples, protein targets per meal, hydration/fluid guidance, goal notes and adherence tips. Free requests receive the basic structure under the matrix, without hidden detailed Pro payloads.

## Client-message drafts

Produce the actual ready-to-review text, specific to known client/check-in facts, rather than only questions. Use “Draft message:” visibly. Preserve factual details when revising tone or length. Delivery/notes/program writes require the corresponding confirmation.

## Canonical rule references

Canonical rule: [[Free_Pro_Entitlements#Useful basic value]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/trainer.js` — TRAINER_OUTPUTS (line 34)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
