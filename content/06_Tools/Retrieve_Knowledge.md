---
id: "ryx.tool.retrieve_knowledge"
title: "Retrieve Knowledge"
type: "tool"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/knowledge/retrieve.js"
  - "ryx-brain/src/knowledge/wedgeRouter.js"
  - "ryx-brain/src/knowledge/wedgeFormat.js"
  - "ryx-brain/src/runChat.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H04"
  - "H11"
  - "H12"
---

# Retrieve Knowledge

## Purpose

Select relevant knowledge with stable provenance for future aligned context.

## When RYX Uses It

Backend retrieval for a request, subordinate to the global hierarchy.

## Inputs

Request/domain/niche and confirmed authorized context; no inference treated as a user record.

## Output

Future units carry note ID, existing knowledge/claim IDs, sources/source areas, niche/taxonomy, caveats, safety constraints and content.

## Permissions

Curated knowledge retrieval does not grant access to athlete records or permit autonomous actions.

## Constraints

Current substring routing/compact projection are not the full future contract. Preserve provenance/caveats rather than silently dropping them; enforce confirmed equipment.

## Failure Behaviour

Missing knowledge remains missing; no fabricated citations, source dates or loading claim. Current absent/malformed-source errors remain implementation.

## Related Brain Rules

[[Knowledge_System#Future retrieval contract]]; [[Knowledge_System#Provenance and evidence]]; [[Brain_Architecture#Global instruction precedence]]

## Implementation Source

retrieveRyxKnowledge/withKnowledgeContext exist; future provenance/selection alignment is not implemented and no model tool registry is added.

The current chat model has no registered autonomous function-calling tools. This note separates the existing app/backend contract from canonical intended constraints requiring later alignment.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/knowledge/retrieve.js` — Complete file (161 lines)
- `ryx-brain/src/knowledge/wedgeRouter.js` — Complete file (154 lines)
- `ryx-brain/src/knowledge/wedgeFormat.js` — Complete file (210 lines)
- `ryx-brain/src/runChat.js` — Complete file (119 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
