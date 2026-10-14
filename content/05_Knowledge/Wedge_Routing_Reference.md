---
id: "ryx.knowledge.wedge_routing_reference"
title: "Wedge Routing Reference"
type: "knowledge"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/knowledge/wedgeRouter.js"
  - "ryx-brain/src/knowledge/nicheMap.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
decision_ids:
  - "H08"
  - "H12"
---

# Wedge Routing Reference

## Reference status

Retained historical/source evidence, excluded from the candidate manifest. It is not an independent canonical instruction or claim of a new passing run. See [[RYX_BRAIN_DECISIONS]] for intended rules and [[Knowledge_System#Future retrieval contract]] / [[Eval_System#Production-quality evaluation contract]] for future integration.

# Wedge Routing Reference

These are the executed route keywords in declaration order; tie behavior follows that order. [[Knowledge_System]] explains their scoring. The niche-to-wedge and exercise-specific overrides are also preserved below.

## Route Table

- Item 1:
  - **slug**: fitness.bodybuilding
  - **kb_id**: ryx.fitness.bodybuilding.v1
  - **niche**: Bodybuilding
  - **terms**:
    - bodybuilding
    - bodybuilder
    - hypertrophy
    - physique
    - muscle gain
    - bulk
    - bulking
    - cutting
    - contest prep
    - posing
    - pump
    - aesthetic
- Item 2:
  - **slug**: fitness.calisthenics
  - **kb_id**: ryx.fitness.calisthenics.v1
  - **niche**: Calisthenics
  - **terms**:
    - calisthenics
    - bodyweight
    - pull-up
    - pullup
    - chin-up
    - muscle-up
    - handstand
    - planche
    - front lever
    - street workout
    - rings
- Item 3:
  - **slug**: fitness.crossfit
  - **kb_id**: ryx.fitness.crossfit.v1
  - **niche**: CrossFit
  - **terms**:
    - crossfit
    - cross fit
    - wod
    - metcon
    - amrap
    - emom
    - functional fitness
    - box jump
    - kipping
- Item 4:
  - **slug**: fitness.powerlifting
  - **kb_id**: ryx.fitness.powerlifting.v1
  - **niche**: Powerlifting
  - **terms**:
    - powerlifting
    - powerlift
    - squat bench deadlift
    - 1rm
    - one rep max
    - ipf
    - usapl
    - strength meet
    - competition squat
- Item 5:
  - **slug**: sports.football
  - **kb_id**: ryx.sports.football.v1
  - **niche**: Football
  - **terms**:
    - football
    - soccer
    - winger
    - striker
    - midfielder
    - pitch
    - match fitness
    - sprint
    - hamstring
- Item 6:
  - **slug**: sports.basketball
  - **kb_id**: ryx.sports.basketball.v1
  - **niche**: Basketball
  - **terms**:
    - basketball
    - hoops
    - court
    - vertical jump
    - dunk
    - nba
- Item 7:
  - **slug**: sports.swimming
  - **kb_id**: ryx.sports.swimming.v1
  - **niche**: Swimming
  - **terms**:
    - swimming
    - swim
    - pool
    - freestyle
    - backstroke
    - breaststroke
    - butterfly
    - lap
    - triathlon swim
- Item 8:
  - **slug**: sports.padel
  - **kb_id**: ryx.sports.padel.v1
  - **niche**: Padel
  - **terms**:
    - padel
    - bandeja
    - vibora
    - chiquita
    - fip
    - padel court
    - volley
    - overhead smash
- Item 9:
  - **slug**: sports.tennis
  - **kb_id**: ryx.sports.tennis.v1
  - **niche**: Tennis
  - **terms**:
    - tennis
    - forehand
    - backhand
    - serve
    - volley
    - racquet
    - racket
    - wta
    - atp
- Item 10:
  - **slug**: sports.golf
  - **kb_id**: ryx.sports.golf.v1
  - **niche**: Golf
  - **terms**:
    - golf
    - swing
    - driver
    - putt
    - fairway
    - iron shot
    - club head
- Item 11:
  - **slug**: sports.combat
  - **kb_id**: ryx.sports.combat.v1
  - **niche**: Combat sports
  - **terms**:
    - boxing
    - mma
    - bjj
    - jiu jitsu
    - jiujitsu
    - grappling
    - submission
    - triangle choke
    - jab
    - hook punch
    - martial arts
- Item 12:
  - **slug**: wellness.rehab
  - **kb_id**: ryx.wellness.rehab.v1
  - **niche**: Rehab & therapy
  - **terms**:
    - rehab
    - physio
    - physical therapy
    - injury
    - pain
    - recovery
    - foam roll
    - stretch
    - mobility drill
    - activation
    - mcgill
    - posture correction
- Item 13:
  - **slug**: wellness.yoga
  - **kb_id**: ryx.wellness.yoga.v1
  - **niche**: Yoga & mind-body
  - **terms**:
    - yoga
    - pilates
    - downward dog
    - sun salutation
    - warrior pose
    - breathwork
    - meditation breath
    - flexibility
    - mind-body
- Item 14:
  - **slug**: fitness.general
  - **kb_id**: ryx.fitness.general.v1
  - **niche**: General fitness
  - **terms**:
    - general fitness
    - workout
    - gym routine
    - full body
    - get fit
    - exercise
    - training session

## Niche Map

- **NICHE_TO_WEDGE**:
  - **strength-upper**: ryx.fitness.general.v1
  - **strength-lower**: ryx.fitness.general.v1
  - **conditioning**: ryx.fitness.crossfit.v1
  - **core**: ryx.fitness.general.v1
  - **kettlebell**: ryx.fitness.crossfit.v1
  - **olympic**: ryx.fitness.powerlifting.v1
  - **mobility-fitness**: ryx.fitness.calisthenics.v1
  - **racquet-padel**: ryx.sports.padel.v1
  - **racquet-tennis**: ryx.sports.tennis.v1
  - **court-basketball**: ryx.sports.basketball.v1
  - **field-golf**: ryx.sports.golf.v1
  - **field-football**: ryx.sports.football.v1
  - **field-soccer**: ryx.sports.football.v1
  - **track**: ryx.sports.football.v1
  - **combat**: ryx.sports.combat.v1
  - **swim**: ryx.sports.swimming.v1
  - **volleyball**: ryx.fitness.general.v1
  - **run**: ryx.fitness.general.v1
  - **cycle**: ryx.fitness.general.v1
  - **core-rehab**: ryx.wellness.rehab.v1
  - **hip-rehab**: ryx.wellness.rehab.v1
  - **shoulder-rehab**: ryx.wellness.rehab.v1
  - **knee-rehab**: ryx.wellness.rehab.v1
  - **ankle-rehab**: ryx.wellness.rehab.v1
  - **spine-mobility**: ryx.wellness.rehab.v1
  - **spine-rehab**: ryx.wellness.rehab.v1
  - **soft-tissue**: ryx.wellness.rehab.v1
  - **glute-activation**: ryx.wellness.rehab.v1
  - **posture**: ryx.wellness.rehab.v1
  - **neck**: ryx.wellness.rehab.v1
  - **yoga**: ryx.wellness.yoga.v1
  - **pilates**: ryx.wellness.yoga.v1
  - **mobility-wellness**: ryx.wellness.yoga.v1
  - **breathwork**: ryx.wellness.yoga.v1
  - **stretching**: ryx.wellness.yoga.v1
- **EXERCISE_WEDGE_OVERRIDES**:
  - **bench-press**:
    - ryx.fitness.bodybuilding.v1
    - ryx.fitness.powerlifting.v1
  - **dumbbell-bench-press**:
    - ryx.fitness.bodybuilding.v1
  - **squat**:
    - ryx.fitness.powerlifting.v1
    - ryx.fitness.bodybuilding.v1
  - **front-squat**:
    - ryx.fitness.powerlifting.v1
  - **deadlift**:
    - ryx.fitness.powerlifting.v1
  - **rdl**:
    - ryx.fitness.bodybuilding.v1
    - ryx.fitness.powerlifting.v1
  - **push-up**:
    - ryx.fitness.calisthenics.v1
    - ryx.fitness.bodybuilding.v1
  - **pull-up**:
    - ryx.fitness.calisthenics.v1
  - **chin-up**:
    - ryx.fitness.calisthenics.v1
  - **burpee**:
    - ryx.fitness.crossfit.v1
  - **kettlebell-swing**:
    - ryx.fitness.crossfit.v1
  - **battle-ropes**:
    - ryx.fitness.crossfit.v1
  - **power-clean**:
    - ryx.fitness.crossfit.v1
    - ryx.fitness.powerlifting.v1
  - **barbell-snatch**:
    - ryx.fitness.crossfit.v1
    - ryx.fitness.powerlifting.v1
  - **rainbow-flick**:
    - ryx.sports.football.v1
  - **soccer-shoot**:
    - ryx.sports.football.v1
  - **soccer-kick**:
    - ryx.sports.football.v1

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
{
  "route_table": [
    {
      "slug": "fitness.bodybuilding",
      "kb_id": "ryx.fitness.bodybuilding.v1",
      "niche": "Bodybuilding",
      "terms": [
        "bodybuilding",
        "bodybuilder",
        "hypertrophy",
        "physique",
        "muscle gain",
        "bulk",
        "bulking",
        "cutting",
        "contest prep",
        "posing",
        "pump",
        "aesthetic"
      ]
    },
    {
      "slug": "fitness.calisthenics",
      "kb_id": "ryx.fitness.calisthenics.v1",
      "niche": "Calisthenics",
      "terms": [
        "calisthenics",
        "bodyweight",
        "pull-up",
        "pullup",
        "chin-up",
        "muscle-up",
        "handstand",
        "planche",
        "front lever",
        "street workout",
        "rings"
      ]
    },
    {
      "slug": "fitness.crossfit",
      "kb_id": "ryx.fitness.crossfit.v1",
      "niche": "CrossFit",
      "terms": [
        "crossfit",
        "cross fit",
        "wod",
        "metcon",
        "amrap",
        "emom",
        "functional fitness",
        "box jump",
        "kipping"
      ]
    },
    {
      "slug": "fitness.powerlifting",
      "kb_id": "ryx.fitness.powerlifting.v1",
      "niche": "Powerlifting",
      "terms": [
        "powerlifting",
        "powerlift",
        "squat bench deadlift",
        "1rm",
        "one rep max",
        "ipf",
        "usapl",
        "strength meet",
        "competition squat"
      ]
    },
    {
      "slug": "sports.football",
      "kb_id": "ryx.sports.football.v1",
      "niche": "Football",
      "terms": [
        "football",
        "soccer",
        "winger",
        "striker",
        "midfielder",
        "pitch",
        "match fitness",
        "sprint",
        "hamstring"
      ]
    },
    {
      "slug": "sports.basketball",
      "kb_id": "ryx.sports.basketball.v1",
      "niche": "Basketball",
      "terms": [
        "basketball",
        "hoops",
        "court",
        "vertical jump",
        "dunk",
        "nba"
      ]
    },
    {
      "slug": "sports.swimming",
      "kb_id": "ryx.sports.swimming.v1",
      "niche": "Swimming",
      "terms": [
        "swimming",
        "swim",
        "pool",
        "freestyle",
        "backstroke",
        "breaststroke",
        "butterfly",
        "lap",
        "triathlon swim"
      ]
    },
    {
      "slug": "sports.padel",
      "kb_id": "ryx.sports.padel.v1",
      "niche": "Padel",
      "terms": [
        "padel",
        "bandeja",
        "vibora",
        "chiquita",
        "fip",
        "padel court",
        "volley",
        "overhead smash"
      ]
    },
    {
      "slug": "sports.tennis",
      "kb_id": "ryx.sports.tennis.v1",
      "niche": "Tennis",
      "terms": [
        "tennis",
        "forehand",
        "backhand",
        "serve",
        "volley",
        "racquet",
        "racket",
        "wta",
        "atp"
      ]
    },
    {
      "slug": "sports.golf",
      "kb_id": "ryx.sports.golf.v1",
      "niche": "Golf",
      "terms": [
        "golf",
        "swing",
        "driver",
        "putt",
        "fairway",
        "iron shot",
        "club head"
      ]
    },
    {
      "slug": "sports.combat",
      "kb_id": "ryx.sports.combat.v1",
      "niche": "Combat sports",
      "terms": [
        "boxing",
        "mma",
        "bjj",
        "jiu jitsu",
        "jiujitsu",
        "grappling",
        "submission",
        "triangle choke",
        "jab",
        "hook punch",
        "martial arts"
      ]
    },
    {
      "slug": "wellness.rehab",
      "kb_id": "ryx.wellness.rehab.v1",
      "niche": "Rehab & therapy",
      "terms": [
        "rehab",
        "physio",
        "physical therapy",
        "injury",
        "pain",
        "recovery",
        "foam roll",
        "stretch",
        "mobility drill",
        "activation",
        "mcgill",
        "posture correction"
      ]
    },
    {
      "slug": "wellness.yoga",
      "kb_id": "ryx.wellness.yoga.v1",
      "niche": "Yoga & mind-body",
      "terms": [
        "yoga",
        "pilates",
        "downward dog",
        "sun salutation",
        "warrior pose",
        "breathwork",
        "meditation breath",
        "flexibility",
        "mind-body"
      ]
    },
    {
      "slug": "fitness.general",
      "kb_id": "ryx.fitness.general.v1",
      "niche": "General fitness",
      "terms": [
        "general fitness",
        "workout",
        "gym routine",
        "full body",
        "get fit",
        "exercise",
        "training session"
      ]
    }
  ],
  "niche_map": {
    "NICHE_TO_WEDGE": {
      "strength-upper": "ryx.fitness.general.v1",
      "strength-lower": "ryx.fitness.general.v1",
      "conditioning": "ryx.fitness.crossfit.v1",
      "core": "ryx.fitness.general.v1",
      "kettlebell": "ryx.fitness.crossfit.v1",
      "olympic": "ryx.fitness.powerlifting.v1",
      "mobility-fitness": "ryx.fitness.calisthenics.v1",
      "racquet-padel": "ryx.sports.padel.v1",
      "racquet-tennis": "ryx.sports.tennis.v1",
      "court-basketball": "ryx.sports.basketball.v1",
      "field-golf": "ryx.sports.golf.v1",
      "field-football": "ryx.sports.football.v1",
      "field-soccer": "ryx.sports.football.v1",
      "track": "ryx.sports.football.v1",
      "combat": "ryx.sports.combat.v1",
      "swim": "ryx.sports.swimming.v1",
      "volleyball": "ryx.fitness.general.v1",
      "run": "ryx.fitness.general.v1",
      "cycle": "ryx.fitness.general.v1",
      "core-rehab": "ryx.wellness.rehab.v1",
      "hip-rehab": "ryx.wellness.rehab.v1",
      "shoulder-rehab": "ryx.wellness.rehab.v1",
      "knee-rehab": "ryx.wellness.rehab.v1",
      "ankle-rehab": "ryx.wellness.rehab.v1",
      "spine-mobility": "ryx.wellness.rehab.v1",
      "spine-rehab": "ryx.wellness.rehab.v1",
      "soft-tissue": "ryx.wellness.rehab.v1",
      "glute-activation": "ryx.wellness.rehab.v1",
      "posture": "ryx.wellness.rehab.v1",
      "neck": "ryx.wellness.rehab.v1",
      "yoga": "ryx.wellness.yoga.v1",
      "pilates": "ryx.wellness.yoga.v1",
      "mobility-wellness": "ryx.wellness.yoga.v1",
      "breathwork": "ryx.wellness.yoga.v1",
      "stretching": "ryx.wellness.yoga.v1"
    },
    "EXERCISE_WEDGE_OVERRIDES": {
      "bench-press": [
        "ryx.fitness.bodybuilding.v1",
        "ryx.fitness.powerlifting.v1"
      ],
      "dumbbell-bench-press": [
        "ryx.fitness.bodybuilding.v1"
      ],
      "squat": [
        "ryx.fitness.powerlifting.v1",
        "ryx.fitness.bodybuilding.v1"
      ],
      "front-squat": [
        "ryx.fitness.powerlifting.v1"
      ],
      "deadlift": [
        "ryx.fitness.powerlifting.v1"
      ],
      "rdl": [
        "ryx.fitness.bodybuilding.v1",
        "ryx.fitness.powerlifting.v1"
      ],
      "push-up": [
        "ryx.fitness.calisthenics.v1",
        "ryx.fitness.bodybuilding.v1"
      ],
      "pull-up": [
        "ryx.fitness.calisthenics.v1"
      ],
      "chin-up": [
        "ryx.fitness.calisthenics.v1"
      ],
      "burpee": [
        "ryx.fitness.crossfit.v1"
      ],
      "kettlebell-swing": [
        "ryx.fitness.crossfit.v1"
      ],
      "battle-ropes": [
        "ryx.fitness.crossfit.v1"
      ],
      "power-clean": [
        "ryx.fitness.crossfit.v1",
        "ryx.fitness.powerlifting.v1"
      ],
      "barbell-snatch": [
        "ryx.fitness.crossfit.v1",
        "ryx.fitness.powerlifting.v1"
      ],
      "rainbow-flick": [
        "ryx.sports.football.v1"
      ],
      "soccer-shoot": [
        "ryx.sports.football.v1"
      ],
      "soccer-kick": [
        "ryx.sports.football.v1"
      ]
    }
  }
}
```

## Source reference

- `ryx-brain/src/knowledge/wedgeRouter.js` — WEDGE_ROUTE_TABLE (line 4)
- `ryx-brain/src/knowledge/nicheMap.js` — Complete file (70 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
