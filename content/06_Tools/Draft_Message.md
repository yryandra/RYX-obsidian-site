---
id: "ryx.tool.draft_message"
title: "Draft Message"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/envelope.js"
  - "ryx-brain/src/replyGuards.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H05"
  - "H08"
  - "H10"
---

# Draft Message

## Purpose

Produce a ready-to-review communication draft.

## When RYX Uses It

Athlete/trainer communication requests using available authorized context.

## Inputs

Confirmed role/mode, current request and supplied client/check-in facts.

## Output

Full visible plain draft starting “Draft message:”; not a delivered message.

## Permissions

Output-generation capability only; authorization does not confer automatic delivery.

## Constraints

Use specific confirmed facts, preserve edits and human review. Program-change text is a proposal under trainer ownership, not an override.

## Failure Behaviour

Identify missing required context; do not invent history, authorization, saving or delivery.

## Related Brain Rules

[[Companion_Mode#Visible draft format]]; [[Trainer_Approval_Model#Trainer suggests, trainer approves]]; [[Data_Boundary#Action confirmation]]

## Implementation Source

Role/output prompts and replyGuards currently require format/mode alignment; no autonomous send tool.

The current chat model has no registered autonomous function-calling tools. This note separates the existing app/backend contract from canonical intended constraints requiring later alignment.

## Canonical rule references

Canonical rule: [[Companion_Mode#Trainer ownership]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-brain/src/envelope.js` — Complete file (401 lines)
- `ryx-brain/src/replyGuards.js` — Complete file (106 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
