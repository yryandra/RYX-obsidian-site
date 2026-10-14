---
id: "ryx.knowledge.knowledge_system"
title: "Knowledge System"
type: "knowledge"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/knowledge/README.md"
  - "ryx-brain/src/knowledge/retrieve.js"
  - "ryx-brain/src/knowledge/wedgeRouter.js"
  - "ryx-brain/src/knowledge/wedgeLoader.js"
  - "ryx-brain/src/knowledge/wedgeFormat.js"
  - "ryx-brain/src/knowledge/formDemos.js"
  - "ryx-brain/src/knowledge/nicheMap.js"
  - "RYX_Wedge_Knowledge_Bases_v1/index.json"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H04"
  - "H06"
  - "H11"
  - "H12"
---

# Knowledge System

## Knowledge layers and scope

Preserve all 14 wedge knowledge sources with their complete structured meaning, stable KB IDs, claim IDs where present, source references, caveats, safety boundaries and taxonomy. Preserve the movement cue/regression library, demo catalog and membership metadata. Do not flatten away a recommendation's caveat or evidence strength.

Stored source richness is distinct from what current runtime retrieval actually projects. Retention in the vault is not proof every field reaches the model.

## Provenance and evidence

Each retrieved knowledge unit remains machine-identifiable with stable provenance. Keep its note ID, original knowledge/claim identifiers where they exist, source/source-area references, applicable niche/domain, caveats, safety constraints and content together. Do not invent citations, claim IDs, stronger evidence or a later verification date.

Niche-specific knowledge can displace generic domain advice only within [[Brain_Architecture#Global instruction precedence]]. It cannot override safety, authorization, core, role, mode, tier, domain/workflow or tool constraints. It does not create a user fact under [[Data_Boundary#Data truth precedence]].

## Future retrieval contract

The future compiler/retrieval system should return units carrying:
- note_id;
- knowledge_id / claim_id where the source provides them;
- source references and source area;
- applicable niche/domain and existing taxonomy;
- caveats;
- safety constraints;
- content, preserving structured meaning and evidence-strength wording.

A unit must not lose a safety caveat during chunking, ranking, truncation or response projection. Missing original IDs remain missing rather than being fabricated as source claims. Resolve applicable guidance against confirmed context/equipment and the canonical instruction hierarchy.

This is an intended contract. No compiler, embeddings, new retriever, schema-validation service or source-refresh integration is implemented here.

## Current runtime, documented separately

Current retrieval uses keyword/profile substring routing, compact formatters and media scoring rather than the complete future contract. It can omit claim/source IDs, slice arrays/objects, truncate strings and leave rich sport/performance/return sections out. The indexed stored KBs are retained fully; exact current routing/media implementation references are reference_only notes.

Role-specific selection currently returns wedge/demos for trainers, and additional supporting movements for athletes. Ranking scores are not strict confirmed-equipment or authorization checks. Future use must apply [[Athlete_Profile#Confirmed equipment]] and approved data/access boundaries.

C21/C22 remain in [[MIGRATION_REVIEW]]. Source verification dates remain unchanged; this phase adds no scientific revalidation claim.

## Browse knowledge

Fitness: [[General]], [[Bodybuilding]], [[Calisthenics]], [[CrossFit]], [[Powerlifting]].
Sports: [[Football]], [[Basketball]], [[Swimming]], [[Padel]], [[Tennis]], [[Golf]], [[Combat]].
Wellness: [[Rehab_and_Therapy]], [[Yoga_and_Mind_Body]].
Supporting: [[Exercise_Library]], [[Exercise_Media_Catalog]], [[Form_Demos_By_Wedge]].

Reference-only implementation/source metadata: [[Wedge_Index]], [[Wedge_Schema]], [[Wedge_Routing_Reference]], [[Exercise_Media_Rules]], [[Legacy_Playbooks]], [[Marketplace_Program_Templates]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/knowledge/README.md` — Complete file (71 lines)
- `ryx-brain/src/knowledge/retrieve.js` — Complete file (161 lines)
- `ryx-brain/src/knowledge/wedgeRouter.js` — Complete file (154 lines)
- `ryx-brain/src/knowledge/wedgeLoader.js` — Complete file (54 lines)
- `ryx-brain/src/knowledge/wedgeFormat.js` — Complete file (210 lines)
- `ryx-brain/src/knowledge/formDemos.js` — Complete file (104 lines)
- `ryx-brain/src/knowledge/nicheMap.js` — Complete file (70 lines)
- `RYX_Wedge_Knowledge_Bases_v1/index.json` — Complete file (107 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
