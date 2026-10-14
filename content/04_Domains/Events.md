---
id: "ryx.domain.events"
title: "Events"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/docs/event-countdown.md"
  - "ryx-brain/src/events.js"
  - "ryx-brain/src/eventFormat.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H04"
  - "H09"
---

# Events

## Dated goal meaning

Events represent race, wedding, photoshoot, competition, vacation or custom dated goals, with active/completed/cancelled state and prep/taper/weigh-in/custom milestones. Creating an event currently marks previous active events completed.

## Active-event semantic intent

Prefer the nearest future active event. “Most recent past active event” means the active event with the most recent past date, not the earliest historical event. This is the canonical semantic intent approved in H09.

Current events.js selects the earliest active past event when all candidates are past; C14 remains a runtime mismatch. No selector code is modified.

## Existing milestones and interpretation

Preserve the existing generic milestone model:
- At 8+ weeks: base-building date at eventDate − weeks×7 + 7; peak block −28 days; taper −14.
- At 4–7 weeks: build phase −floor(weeks×7×0.6); taper −7.
- Shorter windows: final prep −max(3,floor(weeks×7×0.5)).
- Race/competition adds weigh-in/check-weight −2; wedding/photoshoot adds peak-look week −7.
- All add event week −3 and event day; generated past milestone dates are clamped to today, duplicate label/date pairs removed and dates sorted.

These existing scheduling labels do not add clinical or extreme-dieting scope. Within two weeks, prioritize recovery/taper/logistics rather than more volume, subject to safety and confirmed context. Align advice to actual milestones, not invented completion.

## Context and access

The current formatter displays 3 unfinished milestones Free / 6 Pro and completion count. Existing creation/update date validation differs; the brain does not claim those APIs were fixed here.

Canonical rules: [[Data_Boundary#Data truth precedence]]; [[Data_Boundary#Action confirmation]]; [[Safety#Scope and boundaries]]. No live event records are migrated.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/docs/event-countdown.md` — Complete file (73 lines)
- `ryx-brain/src/events.js` — Complete file (262 lines)
- `ryx-brain/src/eventFormat.js` — Complete file (35 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
