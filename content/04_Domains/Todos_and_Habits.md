---
id: "ryx.domain.todos_and_habits"
title: "Todos and Habits"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/docs/todos.md"
  - "ryx-brain/src/todos.js"
  - "ryx-brain/src/todoFormat.js"
  - "ryx-brain/src/envelope.js"
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H02"
  - "H04"
  - "H06"
  - "H10"
---

# Todos and Habits

## Existing record meaning

Todos are saved items with text, done/doneAt, source user/coach and optional origin metadata. Blank/open duplicate items are ignored case-insensitively. Completing/editing/deleting an item is an explicit app operation.

The current context shows 8 open items Free / 12 Pro and can append up to 10 completed items. These caps describe formatting, not authorization or a new persistent analytics engine.

## Canonical suggestions and use

Suggest up to five short actionable saveable items when useful; the user confirms before saving. Reference relevant saved tasks naturally rather than dumping the entire list. Do not mark tasks done yourself or infer completed habits/streaks from encouragement.

Canonical rules: [[Data_Boundary#Action confirmation]]; [[Data_Boundary#Inference boundaries]]; [[Free_Pro_Entitlements#Entitlement matrix]]; [[Memory_Policy#Memory capability truth]].

Crisis is terminal under [[Crisis_Handling#Terminal safety path]] and cannot acquire a task list. Safety-, equipment- and mode-dependent advice retains its canonical owners.

## Canonical rule references

Canonical rule: [[Data_Boundary#Data truth precedence]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/docs/todos.md` — Complete file (40 lines)
- `ryx-brain/src/todos.js` — Complete file (131 lines)
- `ryx-brain/src/todoFormat.js` — Complete file (24 lines)
- `ryx-brain/src/envelope.js` — Complete file (401 lines)
- `ryx-brain/src/prompts/athlete.js` — Complete file (176 lines)
- `ryx-brain/src/athleteSnapshot.js` — Complete file (49 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
