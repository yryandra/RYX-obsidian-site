---
id: "ryx.knowledge.wedge_schema"
title: "Wedge Schema"
type: "knowledge"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "RYX_Wedge_Knowledge_Bases_v1/ryx-wedge-kb.schema.json"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
decision_ids:
  - "H08"
  - "H12"
---

# Wedge Schema

## Reference status

Retained historical/source evidence, excluded from the candidate manifest. It is not an independent canonical instruction or claim of a new passing run. See [[RYX_BRAIN_DECISIONS]] for intended rules and [[Knowledge_System#Future retrieval contract]] / [[Eval_System#Production-quality evaluation contract]] for future integration.

# Wedge Schema

Original permissive JSON schema for wedge records. It describes KB metadata and source record requirements, not live athlete records. Current loader does not execute schema validation. Schema URL is an identifier retained from source, not evidence that a hosted validator was checked. This is a developer reference and is excluded from the production manifest.

## $Schema

https://json-schema.org/draft/2020-12/schema

## $Id

https://coryxworld.com/schemas/ryx-wedge-kb-v1.schema.json

## Title

RYX Wedge Knowledge Base

## Type

object

## Required

- kb_metadata
- scope
- retrieval_taxonomy
- minimum_user_profile
- universal_principles
- programming_engine
- nutrition_and_hydration
- safety_and_escalation
- quality_rules_for_ryx
- sources

## Properties

- **kb_metadata**:
  - **type**: object
  - **required**:
    - kb_id
    - title
    - category
    - niche
    - version
    - knowledge_cutoff_verified
- **sources**:
  - **type**: array
  - **items**:
    - **type**: object
    - **required**:
      - id
      - title
      - year
      - url
      - type

## AdditionalProperties

true

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
{
  "$schema": "https://json-schema.org/draft/2020-12/schema",
  "$id": "https://coryxworld.com/schemas/ryx-wedge-kb-v1.schema.json",
  "title": "RYX Wedge Knowledge Base",
  "type": "object",
  "required": [
    "kb_metadata",
    "scope",
    "retrieval_taxonomy",
    "minimum_user_profile",
    "universal_principles",
    "programming_engine",
    "nutrition_and_hydration",
    "safety_and_escalation",
    "quality_rules_for_ryx",
    "sources"
  ],
  "properties": {
    "kb_metadata": {
      "type": "object",
      "required": [
        "kb_id",
        "title",
        "category",
        "niche",
        "version",
        "knowledge_cutoff_verified"
      ]
    },
    "sources": {
      "type": "array",
      "items": {
        "type": "object",
        "required": [
          "id",
          "title",
          "year",
          "url",
          "type"
        ]
      }
    }
  },
  "additionalProperties": true
}
```

## Source reference

- `RYX_Wedge_Knowledge_Bases_v1/ryx-wedge-kb.schema.json` — Complete file (46 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
