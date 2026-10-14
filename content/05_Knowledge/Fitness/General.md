---
id: "ryx.fitness.general.v1"
title: "General fitness"
type: "knowledge"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "RYX_Wedge_Knowledge_Bases_v1/fitness/general.json"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
kb_id: "ryx.fitness.general.v1"
knowledge_verified_through: "2026-08-01"
canonical: true
decision_ids:
  - "H04"
  - "H11"
  - "H12"
---

# General fitness

## Canonical interpretation and retained source

Canonical rule: [[Knowledge_System#Provenance and evidence]]; [[Knowledge_System#Future retrieval contract]]. Apply [[Brain_Architecture#Global instruction precedence]], [[Data_Boundary#Data truth precedence]], [[Pain_and_Injury#Active pain and clearance]] and [[Athlete_Profile#Confirmed equipment]] before using this lower-priority knowledge. Complete source payloads below remain unchanged; they do not create user facts or override safety/access/tier constraints.

# General fitness

## How to read this knowledge

Foundational strength, conditioning, and movement quality for recreational athletes and general population training.

Start with Scope, Quality Rules For Ryx and Safety And Escalation; then read the programming, nutrition, recovery and niche sections that fit the request. This migration retains the whole source, including material the current SESSION formatter omits/truncates. Original kb_id, claim_id, source_ids, evidence_strength, dates and safety caveats are preserved. The source's verification date has not been advanced and its scientific/rules claims have not been independently revalidated.

[[Knowledge_System]] explains selection and limits. [[Safety]] remains highest priority.

## Kb Metadata

- **kb_id**: ryx.fitness.general.v1
- **title**: RYX General Fitness Wedge Knowledge Base
- **category**: Fitness
- **niche**: General fitness
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

- **definition**: Foundational strength, conditioning, and movement quality for recreational athletes and general population training.
- **included**:
  - (empty array)
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
  - **statement**: Prioritize movement quality over load until technique is consistent.
  - **evidence_strength**: moderate
  - **applies_to**: healthy_adults
  - **last_verified**: 2026-08-01
  - **source_ids**:
    - (empty array)
- Item 2:
  - **claim_id**: principle_2
  - **statement**: Progress one variable at a time: load, volume, complexity, or density.
  - **evidence_strength**: moderate
  - **applies_to**: healthy_adults
  - **last_verified**: 2026-08-01
  - **source_ids**:
    - (empty array)
- Item 3:
  - **claim_id**: principle_3
  - **statement**: Match exercise selection to available equipment and training history.
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

- Use catalog form demo titles when explaining exercises.
- Offer home and gym alternatives when equipment is limited.

## Form Demos

- Item 1:
  - **exercise_id**: ab-wheel
- Item 2:
  - **exercise_id**: band-pull-apart
- Item 3:
  - **exercise_id**: barbell-snatch
- Item 4:
  - **exercise_id**: bench-press
- Item 5:
  - **exercise_id**: bicep-curl
- Item 6:
  - **exercise_id**: bird-dog
- Item 7:
  - **exercise_id**: box-step-up
- Item 8:
  - **exercise_id**: bulgarian-split-squat
- Item 9:
  - **exercise_id**: cable-fly
- Item 10:
  - **exercise_id**: calf-raise
- Item 11:
  - **exercise_id**: chin-tuck
- Item 12:
  - **exercise_id**: chin-up
- Item 13:
  - **exercise_id**: dead-bug
- Item 14:
  - **exercise_id**: deadlift
- Item 15:
  - **exercise_id**: dip
- Item 16:
  - **exercise_id**: dumbbell-bench-press
- Item 17:
  - **exercise_id**: face-pull
- Item 18:
  - **exercise_id**: football-throw
- Item 19:
  - **exercise_id**: front-squat
- Item 20:
  - **exercise_id**: glute-bridge
- Item 21:
  - **exercise_id**: goblet-squat
- Item 22:
  - **exercise_id**: good-morning
- Item 23:
  - **exercise_id**: hip-cars
- Item 24:
  - **exercise_id**: hip-hinge-drill
- Item 25:
  - **exercise_id**: hip-thrust
- Item 26:
  - **exercise_id**: hollow-body-hold
- Item 27:
  - **exercise_id**: incline-push-up
- Item 28:
  - **exercise_id**: indoor-cycling
- Item 29:
  - **exercise_id**: inverted-row
- Item 30:
  - **exercise_id**: lat-pulldown
- Item 31:
  - **exercise_id**: lateral-raise
- Item 32:
  - **exercise_id**: leg-curl
- Item 33:
  - **exercise_id**: leg-press
- Item 34:
  - **exercise_id**: lunge
- Item 35:
  - **exercise_id**: pallof-press
- Item 36:
  - **exercise_id**: plank
- Item 37:
  - **exercise_id**: power-clean
- Item 38:
  - **exercise_id**: pull-up
- Item 39:
  - **exercise_id**: push-up
- Item 40:
  - **exercise_id**: rdl
- Item 41:
  - **exercise_id**: row
- Item 42:
  - **exercise_id**: rowing-machine
- Item 43:
  - **exercise_id**: running-form
- Item 44:
  - **exercise_id**: shoulder-press
- Item 45:
  - **exercise_id**: side-plank
- Item 46:
  - **exercise_id**: spanish-squat
- Item 47:
  - **exercise_id**: squat
- Item 48:
  - **exercise_id**: step-up
- Item 49:
  - **exercise_id**: thoracic-rotation
- Item 50:
  - **exercise_id**: tricep-pushdown
- Item 51:
  - **exercise_id**: volley-smash
- Item 52:
  - **exercise_id**: volleyball-serve
- Item 53:
  - **exercise_id**: volleyball-set

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
    "kb_id": "ryx.fitness.general.v1",
    "title": "RYX General Fitness Wedge Knowledge Base",
    "category": "Fitness",
    "niche": "General fitness",
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
    "definition": "Foundational strength, conditioning, and movement quality for recreational athletes and general population training.",
    "included": [],
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
      "statement": "Prioritize movement quality over load until technique is consistent.",
      "evidence_strength": "moderate",
      "applies_to": "healthy_adults",
      "last_verified": "2026-08-01",
      "source_ids": []
    },
    {
      "claim_id": "principle_2",
      "statement": "Progress one variable at a time: load, volume, complexity, or density.",
      "evidence_strength": "moderate",
      "applies_to": "healthy_adults",
      "last_verified": "2026-08-01",
      "source_ids": []
    },
    {
      "claim_id": "principle_3",
      "statement": "Match exercise selection to available equipment and training history.",
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
    "Use catalog form demo titles when explaining exercises.",
    "Offer home and gym alternatives when equipment is limited."
  ],
  "form_demos": [
    {
      "exercise_id": "ab-wheel"
    },
    {
      "exercise_id": "band-pull-apart"
    },
    {
      "exercise_id": "barbell-snatch"
    },
    {
      "exercise_id": "bench-press"
    },
    {
      "exercise_id": "bicep-curl"
    },
    {
      "exercise_id": "bird-dog"
    },
    {
      "exercise_id": "box-step-up"
    },
    {
      "exercise_id": "bulgarian-split-squat"
    },
    {
      "exercise_id": "cable-fly"
    },
    {
      "exercise_id": "calf-raise"
    },
    {
      "exercise_id": "chin-tuck"
    },
    {
      "exercise_id": "chin-up"
    },
    {
      "exercise_id": "dead-bug"
    },
    {
      "exercise_id": "deadlift"
    },
    {
      "exercise_id": "dip"
    },
    {
      "exercise_id": "dumbbell-bench-press"
    },
    {
      "exercise_id": "face-pull"
    },
    {
      "exercise_id": "football-throw"
    },
    {
      "exercise_id": "front-squat"
    },
    {
      "exercise_id": "glute-bridge"
    },
    {
      "exercise_id": "goblet-squat"
    },
    {
      "exercise_id": "good-morning"
    },
    {
      "exercise_id": "hip-cars"
    },
    {
      "exercise_id": "hip-hinge-drill"
    },
    {
      "exercise_id": "hip-thrust"
    },
    {
      "exercise_id": "hollow-body-hold"
    },
    {
      "exercise_id": "incline-push-up"
    },
    {
      "exercise_id": "indoor-cycling"
    },
    {
      "exercise_id": "inverted-row"
    },
    {
      "exercise_id": "lat-pulldown"
    },
    {
      "exercise_id": "lateral-raise"
    },
    {
      "exercise_id": "leg-curl"
    },
    {
      "exercise_id": "leg-press"
    },
    {
      "exercise_id": "lunge"
    },
    {
      "exercise_id": "pallof-press"
    },
    {
      "exercise_id": "plank"
    },
    {
      "exercise_id": "power-clean"
    },
    {
      "exercise_id": "pull-up"
    },
    {
      "exercise_id": "push-up"
    },
    {
      "exercise_id": "rdl"
    },
    {
      "exercise_id": "row"
    },
    {
      "exercise_id": "rowing-machine"
    },
    {
      "exercise_id": "running-form"
    },
    {
      "exercise_id": "shoulder-press"
    },
    {
      "exercise_id": "side-plank"
    },
    {
      "exercise_id": "spanish-squat"
    },
    {
      "exercise_id": "squat"
    },
    {
      "exercise_id": "step-up"
    },
    {
      "exercise_id": "thoracic-rotation"
    },
    {
      "exercise_id": "tricep-pushdown"
    },
    {
      "exercise_id": "volley-smash"
    },
    {
      "exercise_id": "volleyball-serve"
    },
    {
      "exercise_id": "volleyball-set"
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

- `RYX_Wedge_Knowledge_Bases_v1/fitness/general.json` — Complete file (296 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
