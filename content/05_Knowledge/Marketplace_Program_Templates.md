---
id: "ryx.knowledge.marketplace_program_templates"
title: "Marketplace Program Templates"
type: "knowledge"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/programCatalog.js"
  - "ryx-brain/src/programs.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
decision_ids:
  - "H08"
  - "H12"
---

# Marketplace Program Templates

## Reference status

Retained historical/source evidence, excluded from the candidate manifest. It is not an independent canonical instruction or claim of a new passing run. See [[RYX_BRAIN_DECISIONS]] for intended rules and [[Knowledge_System#Future retrieval contract]] / [[Eval_System#Production-quality evaluation contract]] for future integration.

# Marketplace Program Templates

These three static catalog training templates retain program IDs, titles, level/equipment, descriptions, tags and every stored week/day/card. Mock creator identity objects and commercial price labels are excluded. These are static curriculum templates, not user purchase or assigned-program records.

Declared durationWeeks may exceed stored weeks. getProgramDay chooses the requested stored week/day, falling back to first week/day when missing. Current adaptation operates on that selected day; it does not generate the absent weeks.

## 4-Week Hypertrophy Block

- **id**: prog-hypertrophy-4wk
- **title**: 4-Week Hypertrophy Block
- **tagline**: Upper/lower split with progressive volume for intermediate lifters.
- **durationWeeks**: 4
- **daysPerWeek**: 4
- **level**: Intermediate
- **equipment**: Full gym
- **tags**:
  - Hypertrophy
  - Upper/Lower
- **summary**: Four weeks of upper/lower training with RPE-guided progression. Built for size and strength in compound patterns.
- **weeks**:
  - Item 1:
    - **week**: 1
    - **focus**: Volume accumulation
    - **days**:
      - Item 1:
        - **id**: w1-upper-a
        - **label**: Mon
        - **title**: Upper A — Push focus
        - **card**:
          - **title**: Upper A — Push focus
          - **summary**: Week 1 · Hypertrophy block · Push emphasis
          - **sections**:
            - Item 1:
              - **heading**: Warm-up
              - **items**:
                - 5 min row + band pull-aparts
                - Scap push-ups × 10
            - Item 2:
              - **heading**: Main
              - **items**:
                - Barbell bench press — 4×8 @ RPE 7
                - Incline DB press — 3×10
                - Cable fly — 3×12
                - Tricep pushdown — 3×15
            - Item 3:
              - **heading**: Cool-down
              - **items**:
                - Chest stretch 60s/side
                - Tricep stretch 45s
      - Item 2:
        - **id**: w1-lower-a
        - **label**: Tue
        - **title**: Lower A — Squat focus
        - **card**:
          - **title**: Lower A — Squat focus
          - **summary**: Week 1 · Hypertrophy block · Squat emphasis
          - **sections**:
            - Item 1:
              - **heading**: Warm-up
              - **items**:
                - Bike 5 min
                - Goblet squat × 10
                - Hip flexor stretch 30s/side
            - Item 2:
              - **heading**: Main
              - **items**:
                - Back squat — 4×6 @ RPE 7
                - Romanian deadlift — 3×10
                - Leg press — 3×12
                - Calf raise — 4×15
      - Item 3:
        - **id**: w1-upper-b
        - **label**: Thu
        - **title**: Upper B — Pull focus
        - **card**:
          - **title**: Upper B — Pull focus
          - **summary**: Week 1 · Hypertrophy block · Pull emphasis
          - **sections**:
            - Item 1:
              - **heading**: Main
              - **items**:
                - Lat pulldown — 4×10
                - Barbell row — 3×8
                - Face pull — 3×15
                - Hammer curl — 3×12
      - Item 4:
        - **id**: w1-lower-b
        - **label**: Fri
        - **title**: Lower B — Hinge focus
        - **card**:
          - **title**: Lower B — Hinge focus
          - **summary**: Week 1 · Hypertrophy block · Posterior chain
          - **sections**:
            - Item 1:
              - **heading**: Main
              - **items**:
                - Trap-bar deadlift — 4×5 @ RPE 7
                - Bulgarian split squat — 3×10/leg
                - Leg curl — 3×12
                - Plank — 3×45s

## Beginner Strength Foundations

- **id**: prog-beginner-strength
- **title**: Beginner Strength Foundations
- **tagline**: Three days per week — learn the big lifts with safe progressions.
- **durationWeeks**: 6
- **daysPerWeek**: 3
- **level**: Beginner
- **equipment**: Home / dumbbells
- **tags**:
  - Strength
  - Beginner
- **summary**: Full-body sessions three times per week. Emphasis on movement quality, habit stacking, and gradual load.
- **weeks**:
  - Item 1:
    - **week**: 1
    - **focus**: Movement patterns
    - **days**:
      - Item 1:
        - **id**: w1-full-a
        - **label**: Mon
        - **title**: Full body A
        - **card**:
          - **title**: Full body A
          - **summary**: Week 1 · Beginner strength · Pattern learning
          - **sections**:
            - Item 1:
              - **heading**: Warm-up
              - **items**:
                - March in place 2 min
                - Arm circles + bodyweight squat × 10
            - Item 2:
              - **heading**: Main
              - **items**:
                - Goblet squat — 3×10
                - DB bench press — 3×10
                - DB row — 3×10/side
                - Glute bridge — 3×12
      - Item 2:
        - **id**: w1-full-b
        - **label**: Wed
        - **title**: Full body B
        - **card**:
          - **title**: Full body B
          - **summary**: Week 1 · Beginner strength · Hinge + push
          - **sections**:
            - Item 1:
              - **heading**: Main
              - **items**:
                - DB Romanian deadlift — 3×10
                - Push-up (incline if needed) — 3×8
                - Reverse lunge — 3×8/leg
                - Dead bug — 3×8/side
      - Item 3:
        - **id**: w1-full-c
        - **label**: Fri
        - **title**: Full body C
        - **card**:
          - **title**: Full body C
          - **summary**: Week 1 · Beginner strength · Pull + carry
          - **sections**:
            - Item 1:
              - **heading**: Main
              - **items**:
                - DB squat — 3×10
                - DB overhead press — 3×10
                - Single-arm row — 3×10/side
                - Farmer carry — 3×30s

## Half Marathon Prep — 8 Weeks

- **id**: prog-half-marathon
- **title**: Half Marathon Prep — 8 Weeks
- **tagline**: Build weekly mileage with strength maintenance and taper gates.
- **durationWeeks**: 8
- **daysPerWeek**: 4
- **level**: Intermediate
- **equipment**: Track / road + basic gym
- **tags**:
  - Running
  - Endurance
- **summary**: Structured run plan with easy, tempo, long, and strength sessions. Taper in final two weeks.
- **weeks**:
  - Item 1:
    - **week**: 1
    - **focus**: Base building
    - **days**:
      - Item 1:
        - **id**: w1-easy
        - **label**: Tue
        - **title**: Easy run + strides
        - **card**:
          - **title**: Easy run + strides
          - **summary**: Week 1 · Half marathon prep · Aerobic base
          - **sections**:
            - Item 1:
              - **heading**: Run
              - **items**:
                - Easy 5 km @ conversational pace
                - 4×20s strides with 60s walk recovery
            - Item 2:
              - **heading**: Strength (optional)
              - **items**:
                - Single-leg RDL — 2×10/leg
                - Calf raise — 2×15
                - Side plank — 2×30s/side
      - Item 2:
        - **id**: w1-tempo
        - **label**: Thu
        - **title**: Tempo intervals
        - **card**:
          - **title**: Tempo intervals
          - **summary**: Week 1 · Half marathon prep · Threshold work
          - **sections**:
            - Item 1:
              - **heading**: Run
              - **items**:
                - Warm-up 1.5 km easy
                - 3×5 min @ comfortably hard, 2 min jog between
                - Cool-down 1 km easy
      - Item 3:
        - **id**: w1-long
        - **label**: Sat
        - **title**: Long run
        - **card**:
          - **title**: Long run
          - **summary**: Week 1 · Half marathon prep · Endurance
          - **sections**:
            - Item 1:
              - **heading**: Run
              - **items**:
                - Long run 10 km easy — finish feeling like you could do 2 more km

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
[
  {
    "id": "prog-hypertrophy-4wk",
    "title": "4-Week Hypertrophy Block",
    "tagline": "Upper/lower split with progressive volume for intermediate lifters.",
    "durationWeeks": 4,
    "daysPerWeek": 4,
    "level": "Intermediate",
    "equipment": "Full gym",
    "tags": [
      "Hypertrophy",
      "Upper/Lower"
    ],
    "summary": "Four weeks of upper/lower training with RPE-guided progression. Built for size and strength in compound patterns.",
    "weeks": [
      {
        "week": 1,
        "focus": "Volume accumulation",
        "days": [
          {
            "id": "w1-upper-a",
            "label": "Mon",
            "title": "Upper A — Push focus",
            "card": {
              "title": "Upper A — Push focus",
              "summary": "Week 1 · Hypertrophy block · Push emphasis",
              "sections": [
                {
                  "heading": "Warm-up",
                  "items": [
                    "5 min row + band pull-aparts",
                    "Scap push-ups × 10"
                  ]
                },
                {
                  "heading": "Main",
                  "items": [
                    "Barbell bench press — 4×8 @ RPE 7",
                    "Incline DB press — 3×10",
                    "Cable fly — 3×12",
                    "Tricep pushdown — 3×15"
                  ]
                },
                {
                  "heading": "Cool-down",
                  "items": [
                    "Chest stretch 60s/side",
                    "Tricep stretch 45s"
                  ]
                }
              ]
            }
          },
          {
            "id": "w1-lower-a",
            "label": "Tue",
            "title": "Lower A — Squat focus",
            "card": {
              "title": "Lower A — Squat focus",
              "summary": "Week 1 · Hypertrophy block · Squat emphasis",
              "sections": [
                {
                  "heading": "Warm-up",
                  "items": [
                    "Bike 5 min",
                    "Goblet squat × 10",
                    "Hip flexor stretch 30s/side"
                  ]
                },
                {
                  "heading": "Main",
                  "items": [
                    "Back squat — 4×6 @ RPE 7",
                    "Romanian deadlift — 3×10",
                    "Leg press — 3×12",
                    "Calf raise — 4×15"
                  ]
                }
              ]
            }
          },
          {
            "id": "w1-upper-b",
            "label": "Thu",
            "title": "Upper B — Pull focus",
            "card": {
              "title": "Upper B — Pull focus",
              "summary": "Week 1 · Hypertrophy block · Pull emphasis",
              "sections": [
                {
                  "heading": "Main",
                  "items": [
                    "Lat pulldown — 4×10",
                    "Barbell row — 3×8",
                    "Face pull — 3×15",
                    "Hammer curl — 3×12"
                  ]
                }
              ]
            }
          },
          {
            "id": "w1-lower-b",
            "label": "Fri",
            "title": "Lower B — Hinge focus",
            "card": {
              "title": "Lower B — Hinge focus",
              "summary": "Week 1 · Hypertrophy block · Posterior chain",
              "sections": [
                {
                  "heading": "Main",
                  "items": [
                    "Trap-bar deadlift — 4×5 @ RPE 7",
                    "Bulgarian split squat — 3×10/leg",
                    "Leg curl — 3×12",
                    "Plank — 3×45s"
                  ]
                }
              ]
            }
          }
        ]
      }
    ]
  },
  {
    "id": "prog-beginner-strength",
    "title": "Beginner Strength Foundations",
    "tagline": "Three days per week — learn the big lifts with safe progressions.",
    "durationWeeks": 6,
    "daysPerWeek": 3,
    "level": "Beginner",
    "equipment": "Home / dumbbells",
    "tags": [
      "Strength",
      "Beginner"
    ],
    "summary": "Full-body sessions three times per week. Emphasis on movement quality, habit stacking, and gradual load.",
    "weeks": [
      {
        "week": 1,
        "focus": "Movement patterns",
        "days": [
          {
            "id": "w1-full-a",
            "label": "Mon",
            "title": "Full body A",
            "card": {
              "title": "Full body A",
              "summary": "Week 1 · Beginner strength · Pattern learning",
              "sections": [
                {
                  "heading": "Warm-up",
                  "items": [
                    "March in place 2 min",
                    "Arm circles + bodyweight squat × 10"
                  ]
                },
                {
                  "heading": "Main",
                  "items": [
                    "Goblet squat — 3×10",
                    "DB bench press — 3×10",
                    "DB row — 3×10/side",
                    "Glute bridge — 3×12"
                  ]
                }
              ]
            }
          },
          {
            "id": "w1-full-b",
            "label": "Wed",
            "title": "Full body B",
            "card": {
              "title": "Full body B",
              "summary": "Week 1 · Beginner strength · Hinge + push",
              "sections": [
                {
                  "heading": "Main",
                  "items": [
                    "DB Romanian deadlift — 3×10",
                    "Push-up (incline if needed) — 3×8",
                    "Reverse lunge — 3×8/leg",
                    "Dead bug — 3×8/side"
                  ]
                }
              ]
            }
          },
          {
            "id": "w1-full-c",
            "label": "Fri",
            "title": "Full body C",
            "card": {
              "title": "Full body C",
              "summary": "Week 1 · Beginner strength · Pull + carry",
              "sections": [
                {
                  "heading": "Main",
                  "items": [
                    "DB squat — 3×10",
                    "DB overhead press — 3×10",
                    "Single-arm row — 3×10/side",
                    "Farmer carry — 3×30s"
                  ]
                }
              ]
            }
          }
        ]
      }
    ]
  },
  {
    "id": "prog-half-marathon",
    "title": "Half Marathon Prep — 8 Weeks",
    "tagline": "Build weekly mileage with strength maintenance and taper gates.",
    "durationWeeks": 8,
    "daysPerWeek": 4,
    "level": "Intermediate",
    "equipment": "Track / road + basic gym",
    "tags": [
      "Running",
      "Endurance"
    ],
    "summary": "Structured run plan with easy, tempo, long, and strength sessions. Taper in final two weeks.",
    "weeks": [
      {
        "week": 1,
        "focus": "Base building",
        "days": [
          {
            "id": "w1-easy",
            "label": "Tue",
            "title": "Easy run + strides",
            "card": {
              "title": "Easy run + strides",
              "summary": "Week 1 · Half marathon prep · Aerobic base",
              "sections": [
                {
                  "heading": "Run",
                  "items": [
                    "Easy 5 km @ conversational pace",
                    "4×20s strides with 60s walk recovery"
                  ]
                },
                {
                  "heading": "Strength (optional)",
                  "items": [
                    "Single-leg RDL — 2×10/leg",
                    "Calf raise — 2×15",
                    "Side plank — 2×30s/side"
                  ]
                }
              ]
            }
          },
          {
            "id": "w1-tempo",
            "label": "Thu",
            "title": "Tempo intervals",
            "card": {
              "title": "Tempo intervals",
              "summary": "Week 1 · Half marathon prep · Threshold work",
              "sections": [
                {
                  "heading": "Run",
                  "items": [
                    "Warm-up 1.5 km easy",
                    "3×5 min @ comfortably hard, 2 min jog between",
                    "Cool-down 1 km easy"
                  ]
                }
              ]
            }
          },
          {
            "id": "w1-long",
            "label": "Sat",
            "title": "Long run",
            "card": {
              "title": "Long run",
              "summary": "Week 1 · Half marathon prep · Endurance",
              "sections": [
                {
                  "heading": "Run",
                  "items": [
                    "Long run 10 km easy — finish feeling like you could do 2 more km"
                  ]
                }
              ]
            }
          }
        ]
      }
    ]
  }
]
```

## Source reference

- `ryx-brain/src/programCatalog.js` — Complete file (223 lines)
- `ryx-brain/src/programs.js` — Complete file (245 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
