---
id: "ryx.runtime.context.known_context"
title: "Known Context"
type: "runtime-context"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/buildSystemPrompt.js"
  - "ryx-brain/src/chatIntake.js"
  - "ryx-brain/src/labMemory.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H04"
  - "H05"
  - "H10"
  - "H11"
---

# Known Context

## Confirmed context and provenance

Known context is temporary authorized context supplied through SESSION. It must distinguish fresh backend records, persisted profile/state, explicit current-conversation facts and labelled inference according to [[Data_Boundary#Data truth precedence]].

Use established facts naturally and avoid re-asking what is already known. Do not convert an assistant suggestion or extractor label into a verified record. User-accepted plans are not proof of execution; a missing body report is not clearance; a named sport is not equipment ownership.

Canonical rules: [[Data_Boundary#Inference boundaries]]; [[Data_Boundary#Action confirmation]].

## Safety and operation-critical facts

Canonical rule: [[Pain_and_Injury#Active pain and clearance]].

Mentioning a physiotherapist, prior treatment, improved pain or monitoring does not establish action-sufficient professional clearance. Confirm safety-, permission- and action-critical gaps. Incomplete unrelated profile fields do not block a valid response under [[Response_Principles#Request-specific sufficiency and deliver-first]].

## Current implementation, not canonical fact creation

The current extractor can infer schedule/equipment/clearance-like labels from weak thread signals; it can also overwrite specific values with scored coarse labels. Those behaviors are C15 and must be aligned later rather than treated as permission to invent context. The existing persistence whitelist and context fields remain in code; no new record schema or preference memory is implemented here.

Unknown/missing context stays unknown. A request may still receive useful noncritical alternatives with assumptions clearly labelled.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/buildSystemPrompt.js` — skipKeys (line 145)
- `ryx-brain/src/chatIntake.js` — Complete file (17 lines)
- `ryx-brain/src/labMemory.js` — Complete file (929 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
