---
id: "ryx.sports.golf.v1"
title: "Golf"
type: "knowledge"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "RYX_Wedge_Knowledge_Bases_v1/sports/golf.json"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
kb_id: "ryx.sports.golf.v1"
knowledge_verified_through: "2026-08-01"
canonical: true
decision_ids:
  - "H04"
  - "H11"
  - "H12"
---

# Golf

## Canonical interpretation and retained source

Canonical rule: [[Knowledge_System#Provenance and evidence]]; [[Knowledge_System#Future retrieval contract]]. Apply [[Brain_Architecture#Global instruction precedence]], [[Data_Boundary#Data truth precedence]], [[Pain_and_Injury#Active pain and clearance]] and [[Athlete_Profile#Confirmed equipment]] before using this lower-priority knowledge. Complete source payloads below remain unchanged; they do not create user facts or override safety/access/tier constraints.

# Golf

## How to read this knowledge

Rotational power sport requiring hip mobility, thoracic rotation, and repeatable swing mechanics.

Start with Scope, Quality Rules For Ryx and Safety And Escalation; then read the programming, nutrition, recovery and niche sections that fit the request. This migration retains the whole source, including material the current SESSION formatter omits/truncates. Original kb_id, claim_id, source_ids, evidence_strength, dates and safety caveats are preserved. The source's verification date has not been advanced and its scientific/rules claims have not been independently revalidated.

[[Knowledge_System]] explains selection and limits. [[Safety]] remains highest priority.

## Kb Metadata

- **kb_id**: ryx.sports.golf.v1
- **title**: RYX Golf Wedge Knowledge Base
- **category**: Sports
- **niche**: Golf
- **version**: 1.0.0
- **language**: en
- **created_at**: 2026-08-01
- **knowledge_cutoff_verified**: 2026-08-01
- **intended_use**:
  - retrieval_augmented_generation
  - coach_copilot
  - athlete_education
- **not_intended_use**:
  - medical_diagnosis
  - emergency_care
  - replacement_for_qualified_coach_or_clinician

## Scope

- **definition**: Rotational power sport requiring hip mobility, thoracic rotation, and repeatable swing mechanics.
- **included**:
  - full_swing
  - short_game
  - mobility
- **excluded_or_separate**:
  - (empty array)

## Retrieval Taxonomy

- **intents**:
  - learn
  - technique_help
  - plan
  - recovery
  - injury_risk
  - return_to_sport
- **athlete_levels**:
  - novice
  - beginner
  - intermediate
  - advanced
- **contexts**:
  - general_health
  - recreation
  - performance
  - rehabilitation_adjacent

## Minimum User Profile

- goals
- training_age
- injury_and_medical_history
- equipment_and_facilities

## Universal Principles

- Item 1:
  - **claim_id**: principle_1
  - **statement**: Mobility and stability precede speed — do not chase club head speed with poor sequencing.
  - **evidence_strength**: moderate
  - **applies_to**: healthy_adults
  - **last_verified**: 2026-08-01
  - **source_ids**:
    - (empty array)
- Item 2:
  - **claim_id**: principle_2
  - **statement**: Train rotation and anti-rotation for transfer to the swing.
  - **evidence_strength**: moderate
  - **applies_to**: healthy_adults
  - **last_verified**: 2026-08-01
  - **source_ids**:
    - (empty array)

## Programming Engine

- **workflow**:
  - clarify_goal_and_context
  - assess_readiness_and_contraindications
  - select_appropriate_progression
  - prescribe_with_form_cues
  - attach_form_demo_when_available
  - monitor_response_and_adjust
- **autoregulatory_rules**:
  - Item 1:
    - **if**: pain_is_sharp_or_increasing
    - **then**: stop_or_regress_and_screen
  - Item 2:
    - **if**: technique_breaks_down
    - **then**: reduce_load_or_complexity

## Nutrition And Hydration

- **principles**:
  - Item 1:
    - **claim_id**: hydration
    - **statement**: Support training with adequate hydration; adjust for heat and session length.
    - **evidence_strength**: moderate
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-08-01
    - **source_ids**:
      - (empty array)

## Safety And Escalation

- **coaching_boundary**: Do not diagnose injuries. Refer to qualified clinicians for pain, numbness, or red-flag symptoms.
- **when_to_refer**:
  - persistent_pain
  - neurological_symptoms
  - post_surgical_without_clearance

## Quality Rules For Ryx

- Use exact movement names from form_demos when explaining technique.
- Offer regressions before advanced variations.
- Pair verbal cues with available video demos when the user asks how to perform a movement.

## Form Demos

- Item 1:
  - **exercise_id**: golf-swing

## Sources

- Item 1:
  - **id**: RYX_MEDIA_CATALOG
  - **title**: RYX Exercise Media Catalog
  - **year**: 2026
  - **url**: https://github.com/coryxworld/ryx
  - **type**: internal

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
{
  "kb_metadata": {
    "kb_id": "ryx.sports.golf.v1",
    "title": "RYX Golf Wedge Knowledge Base",
    "category": "Sports",
    "niche": "Golf",
    "version": "1.0.0",
    "language": "en",
    "created_at": "2026-08-01",
    "knowledge_cutoff_verified": "2026-08-01",
    "intended_use": [
      "retrieval_augmented_generation",
      "coach_copilot",
      "athlete_education"
    ],
    "not_intended_use": [
      "medical_diagnosis",
      "emergency_care",
      "replacement_for_qualified_coach_or_clinician"
    ]
  },
  "scope": {
    "definition": "Rotational power sport requiring hip mobility, thoracic rotation, and repeatable swing mechanics.",
    "included": [
      "full_swing",
      "short_game",
      "mobility"
    ],
    "excluded_or_separate": []
  },
  "retrieval_taxonomy": {
    "intents": [
      "learn",
      "technique_help",
      "plan",
      "recovery",
      "injury_risk",
      "return_to_sport"
    ],
    "athlete_levels": [
      "novice",
      "beginner",
      "intermediate",
      "advanced"
    ],
    "contexts": [
      "general_health",
      "recreation",
      "performance",
      "rehabilitation_adjacent"
    ]
  },
  "minimum_user_profile": [
    "goals",
    "training_age",
    "injury_and_medical_history",
    "equipment_and_facilities"
  ],
  "universal_principles": [
    {
      "claim_id": "principle_1",
      "statement": "Mobility and stability precede speed — do not chase club head speed with poor sequencing.",
      "evidence_strength": "moderate",
      "applies_to": "healthy_adults",
      "last_verified": "2026-08-01",
      "source_ids": []
    },
    {
      "claim_id": "principle_2",
      "statement": "Train rotation and anti-rotation for transfer to the swing.",
      "evidence_strength": "moderate",
      "applies_to": "healthy_adults",
      "last_verified": "2026-08-01",
      "source_ids": []
    }
  ],
  "programming_engine": {
    "workflow": [
      "clarify_goal_and_context",
      "assess_readiness_and_contraindications",
      "select_appropriate_progression",
      "prescribe_with_form_cues",
      "attach_form_demo_when_available",
      "monitor_response_and_adjust"
    ],
    "autoregulatory_rules": [
      {
        "if": "pain_is_sharp_or_increasing",
        "then": "stop_or_regress_and_screen"
      },
      {
        "if": "technique_breaks_down",
        "then": "reduce_load_or_complexity"
      }
    ]
  },
  "nutrition_and_hydration": {
    "principles": [
      {
        "claim_id": "hydration",
        "statement": "Support training with adequate hydration; adjust for heat and session length.",
        "evidence_strength": "moderate",
        "applies_to": "healthy_adults",
        "last_verified": "2026-08-01",
        "source_ids": []
      }
    ]
  },
  "safety_and_escalation": {
    "coaching_boundary": "Do not diagnose injuries. Refer to qualified clinicians for pain, numbness, or red-flag symptoms.",
    "when_to_refer": [
      "persistent_pain",
      "neurological_symptoms",
      "post_surgical_without_clearance"
    ]
  },
  "quality_rules_for_ryx": [
    "Use exact movement names from form_demos when explaining technique.",
    "Offer regressions before advanced variations.",
    "Pair verbal cues with available video demos when the user asks how to perform a movement."
  ],
  "form_demos": [
    {
      "exercise_id": "golf-swing"
    }
  ],
  "sources": [
    {
      "id": "RYX_MEDIA_CATALOG",
      "title": "RYX Exercise Media Catalog",
      "year": 2026,
      "url": "https://github.com/coryxworld/ryx",
      "type": "internal"
    }
  ]
}
```

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `RYX_Wedge_Knowledge_Bases_v1/sports/golf.json` — Complete file (137 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
