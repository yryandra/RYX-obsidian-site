---
id: "ryx.knowledge.wedge_index"
title: "Wedge Index"
type: "knowledge"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "RYX_Wedge_Knowledge_Bases_v1/index.json"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
decision_ids:
  - "H08"
  - "H12"
---

# Wedge Index

## Reference status

Retained historical/source evidence, excluded from the candidate manifest. It is not an independent canonical instruction or claim of a new passing run. See [[RYX_BRAIN_DECISIONS]] for intended rules and [[Knowledge_System#Future retrieval contract]] / [[Eval_System#Production-quality evaluation contract]] for future integration.

# Wedge Index

Original collection/version/verification metadata, indexed KB IDs, routing groups and intended implementation notes. Relative JSON paths below refer to the original repository collection; the corresponding navigable vault notes are listed in [[Knowledge_System]].

## Collection

RYX Wedge Knowledge Bases

## Version

1.0.0

## Verified Through

2026-07-28

## Files

- Item 1:
  - **path**: fitness/bodybuilding.json
  - **kb_id**: ryx.fitness.bodybuilding.v1
  - **niche**: Bodybuilding
- Item 2:
  - **path**: fitness/calisthenics.json
  - **kb_id**: ryx.fitness.calisthenics.v1
  - **niche**: Calisthenics
- Item 3:
  - **path**: fitness/crossfit.json
  - **kb_id**: ryx.fitness.crossfit.v1
  - **niche**: CrossFit
- Item 4:
  - **path**: fitness/powerlifting.json
  - **kb_id**: ryx.fitness.powerlifting.v1
  - **niche**: Powerlifting
- Item 5:
  - **path**: sports/football.json
  - **kb_id**: ryx.sports.football.v1
  - **niche**: Football
- Item 6:
  - **path**: sports/basketball.json
  - **kb_id**: ryx.sports.basketball.v1
  - **niche**: Basketball
- Item 7:
  - **path**: sports/swimming.json
  - **kb_id**: ryx.sports.swimming.v1
  - **niche**: Swimming
- Item 8:
  - **path**: sports/padel.json
  - **kb_id**: ryx.sports.padel.v1
  - **niche**: Padel
- Item 9:
  - **path**: sports/tennis.json
  - **kb_id**: ryx.sports.tennis.v1
  - **niche**: Tennis
- Item 10:
  - **path**: sports/golf.json
  - **kb_id**: ryx.sports.golf.v1
  - **niche**: Golf
- Item 11:
  - **path**: sports/combat.json
  - **kb_id**: ryx.sports.combat.v1
  - **niche**: Combat sports
- Item 12:
  - **path**: fitness/general.json
  - **kb_id**: ryx.fitness.general.v1
  - **niche**: General fitness
- Item 13:
  - **path**: wellness/rehab.json
  - **kb_id**: ryx.wellness.rehab.v1
  - **niche**: Rehab & therapy
- Item 14:
  - **path**: wellness/yoga.json
  - **kb_id**: ryx.wellness.yoga.v1
  - **niche**: Yoga & mind-body

## Routing

- **fitness**:
  - bodybuilding
  - calisthenics
  - crossfit
  - powerlifting
  - general
- **sports**:
  - football
  - basketball
  - swimming
  - padel
  - tennis
  - golf
  - combat
- **wellness**:
  - rehab
  - yoga
- **multi_wedge_rule**: Retrieve the primary niche plus shared evidence when a query spans strength, nutrition, injury risk, or competition.

## Implementation Notes

- Chunk at meaningful object boundaries; preserve claim_id and source_ids.
- Filter by niche, intent, athlete level, population, and ruleset.
- Never detach a recommendation from its caveat, evidence strength, or safety escalation.
- Run JSON Schema validation and source-refresh checks in CI.

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
{
  "collection": "RYX Wedge Knowledge Bases",
  "version": "1.0.0",
  "verified_through": "2026-07-28",
  "files": [
    {
      "path": "fitness/bodybuilding.json",
      "kb_id": "ryx.fitness.bodybuilding.v1",
      "niche": "Bodybuilding"
    },
    {
      "path": "fitness/calisthenics.json",
      "kb_id": "ryx.fitness.calisthenics.v1",
      "niche": "Calisthenics"
    },
    {
      "path": "fitness/crossfit.json",
      "kb_id": "ryx.fitness.crossfit.v1",
      "niche": "CrossFit"
    },
    {
      "path": "fitness/powerlifting.json",
      "kb_id": "ryx.fitness.powerlifting.v1",
      "niche": "Powerlifting"
    },
    {
      "path": "sports/football.json",
      "kb_id": "ryx.sports.football.v1",
      "niche": "Football"
    },
    {
      "path": "sports/basketball.json",
      "kb_id": "ryx.sports.basketball.v1",
      "niche": "Basketball"
    },
    {
      "path": "sports/swimming.json",
      "kb_id": "ryx.sports.swimming.v1",
      "niche": "Swimming"
    },
    {
      "path": "sports/padel.json",
      "kb_id": "ryx.sports.padel.v1",
      "niche": "Padel"
    },
    {
      "path": "sports/tennis.json",
      "kb_id": "ryx.sports.tennis.v1",
      "niche": "Tennis"
    },
    {
      "path": "sports/golf.json",
      "kb_id": "ryx.sports.golf.v1",
      "niche": "Golf"
    },
    {
      "path": "sports/combat.json",
      "kb_id": "ryx.sports.combat.v1",
      "niche": "Combat sports"
    },
    {
      "path": "fitness/general.json",
      "kb_id": "ryx.fitness.general.v1",
      "niche": "General fitness"
    },
    {
      "path": "wellness/rehab.json",
      "kb_id": "ryx.wellness.rehab.v1",
      "niche": "Rehab & therapy"
    },
    {
      "path": "wellness/yoga.json",
      "kb_id": "ryx.wellness.yoga.v1",
      "niche": "Yoga & mind-body"
    }
  ],
  "routing": {
    "fitness": [
      "bodybuilding",
      "calisthenics",
      "crossfit",
      "powerlifting",
      "general"
    ],
    "sports": [
      "football",
      "basketball",
      "swimming",
      "padel",
      "tennis",
      "golf",
      "combat"
    ],
    "wellness": [
      "rehab",
      "yoga"
    ],
    "multi_wedge_rule": "Retrieve the primary niche plus shared evidence when a query spans strength, nutrition, injury risk, or competition."
  },
  "implementation_notes": [
    "Chunk at meaningful object boundaries; preserve claim_id and source_ids.",
    "Filter by niche, intent, athlete level, population, and ruleset.",
    "Never detach a recommendation from its caveat, evidence strength, or safety escalation.",
    "Run JSON Schema validation and source-refresh checks in CI."
  ]
}
```

## Source reference

- `RYX_Wedge_Knowledge_Bases_v1/index.json` — Complete file (107 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
