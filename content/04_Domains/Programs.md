---
id: "ryx.domain.programs"
title: "Programs"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/docs/program-marketplace.md"
  - "ryx-brain/src/programCatalog.js"
  - "ryx-brain/src/programs.js"
  - "ryx-brain/src/programFormat.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-landing/src/App.jsx"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H05"
  - "H06"
  - "H08"
  - "H11"
---

# Programs

## Program sources and ownership

An assigned trainer-controlled program and a purchased marketplace template are distinct sources. The current assigned version is authoritative over marketplace and older conversation context; its human ownership governs Companion proposals.

Canonical rules: [[Companion_Mode#Trainer ownership]]; [[Trainer_Approval_Model#Trainer suggests, trainer approves]].
Canonical entitlement: [[Free_Pro_Entitlements#Entitlement matrix]].

## Confirmed equipment and adjustments

Canonical equipment rule: [[Athlete_Profile#Confirmed equipment]].

Adapt only to confirmed available equipment. Bodyweight-only does not imply dumbbells or bands. Unknown equipment calls for a required question or explicitly labelled alternatives, not an ownership assumption. Safety and mode control apply before adaptation.

## Missing weeks and days

Do not silently invent or reuse a missing week/day as if it came from the original trainer or purchased program. Identify what is actually stored and what is missing. Declared duration alone is not proof that every week exists.

If RYX fills a gap, label the added content explicitly as an RYX-generated suggestion/draft, subject to Solo/Companion/Trainer control and tier. A trainer replacement draft remains complete and reviewable; no unapproved gap fill becomes an assigned program.

## Current backend facts and future alignment

The existing marketplace has three static programs, stub purchases and a rule-based selected-day adaptation hook. It can create a stub purchase as a side effect; other active purchases can be paused. It does not verify payments, automatically generate absent weeks or advance week/day from workout completion.

The hook's bodyweight/home DB swaps and first-week/day fallback are C16 and H11 alignment issues. Exact templates and historical implementation are reference_only material in [[Marketplace_Program_Templates]] and the archive, not canonical instructions to invent missing source content.

Assigned program writes still require connected-trainer permission and an expected version; stale drafts reject with 409. No program store, API, payment or adaptation implementation changes occur here.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/docs/program-marketplace.md` — Complete file (112 lines)
- `ryx-brain/src/programCatalog.js` — Complete file (223 lines)
- `ryx-brain/src/programs.js` — Complete file (245 lines)
- `ryx-brain/src/programFormat.js` — Complete file (28 lines)
- `ryx-brain/src/identity.js` — Complete file (203 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)
- `ryx-brain/src/prompts/trainer.js` — Complete file (205 lines)
- `ryx-landing/src/App.jsx` — Complete file (3315 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
