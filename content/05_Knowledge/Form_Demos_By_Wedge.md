---
id: "ryx.knowledge.form_demos_by_wedge"
title: "Form Demos by Wedge"
type: "knowledge"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/knowledge/data/formDemosByWedge.json"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H04"
  - "H11"
  - "H12"
---

# Form Demos by Wedge

## Canonical interpretation and retained source

Canonical rule: [[Knowledge_System#Provenance and evidence]]; [[Knowledge_System#Future retrieval contract]]. Apply [[Brain_Architecture#Global instruction precedence]], [[Data_Boundary#Data truth precedence]], [[Pain_and_Injury#Active pain and clearance]] and [[Athlete_Profile#Confirmed equipment]] before using this lower-priority knowledge. Complete source payloads below remain unchanged; they do not create user facts or override safety/access/tier constraints.

# Form Demos by Wedge

The exact wedge → movement ID membership manifest used for demo retrieval. Read alongside [[Exercise_Media_Catalog]] and [[Knowledge_System]].

## Generated At

2026-08-01T09:12:23.324Z

## ByWedge

- **ryx.fitness.general.v1**:
  - ab-wheel
  - band-pull-apart
  - barbell-snatch
  - bench-press
  - bicep-curl
  - bird-dog
  - box-step-up
  - bulgarian-split-squat
  - cable-fly
  - calf-raise
  - chin-tuck
  - chin-up
  - dead-bug
  - deadlift
  - dip
  - dumbbell-bench-press
  - face-pull
  - football-throw
  - front-squat
  - glute-bridge
  - goblet-squat
  - good-morning
  - hip-cars
  - hip-hinge-drill
  - hip-thrust
  - hollow-body-hold
  - incline-push-up
  - indoor-cycling
  - inverted-row
  - lat-pulldown
  - lateral-raise
  - leg-curl
  - leg-press
  - lunge
  - pallof-press
  - plank
  - power-clean
  - pull-up
  - push-up
  - rdl
  - row
  - rowing-machine
  - running-form
  - shoulder-press
  - side-plank
  - spanish-squat
  - squat
  - step-up
  - thoracic-rotation
  - tricep-pushdown
  - volley-smash
  - volleyball-serve
  - volleyball-set
- **ryx.fitness.bodybuilding.v1**:
  - bench-press
  - dumbbell-bench-press
  - push-up
  - rdl
  - squat
- **ryx.fitness.powerlifting.v1**:
  - barbell-snatch
  - bench-press
  - deadlift
  - front-squat
  - power-clean
  - rdl
  - squat
- **ryx.wellness.rehab.v1**:
  - 90-90-hip-stretch
  - band-pull-apart
  - banded-lateral-walk
  - bird-dog
  - calf-stretch-achilles
  - cat-cow
  - chin-tuck
  - clamshell
  - dead-bug
  - foam-roll-it-band
  - foam-roll-quads
  - foam-roll-upper-back
  - glute-bridge
  - hip-flexor-stretch
  - mcgill-big-3
  - monster-walk
  - pallof-press
  - pigeon-stretch
  - plank
  - scapular-push-up
  - sleeper-stretch
  - spanish-squat
  - terminal-knee-extension
  - wall-angel
  - wall-slide
  - ytwl-shoulder
- **ryx.fitness.calisthenics.v1**:
  - chin-up
  - pull-up
  - push-up
  - worlds-greatest-stretch
- **ryx.fitness.crossfit.v1**:
  - barbell-snatch
  - battle-ropes
  - box-jump
  - burpee
  - farmer-carry
  - indoor-cycling
  - jump-rope
  - kettlebell-swing
  - mountain-climbers
  - power-clean
  - rowing-machine
  - running-form
  - sled-push
  - sprint-blocks
  - turkish-get-up
- **ryx.wellness.yoga.v1**:
  - 90-90-hip-stretch
  - box-breathing
  - calf-stretch-achilles
  - cat-cow
  - childs-pose
  - diaphragmatic-breathing
  - downward-dog
  - figure-four-stretch
  - hamstring-stretch
  - hip-cars
  - hip-flexor-stretch
  - pigeon-stretch
  - pilates-hundred
  - pilates-roll-up
  - sleeper-stretch
  - sun-salutation
  - thoracic-rotation
  - warrior-2
  - worlds-greatest-stretch
- **ryx.sports.padel.v1**:
  - padel-bandeja
  - padel-basics
  - padel-serve
  - padel-swing
  - padel-volley
  - volley-smash
- **ryx.sports.tennis.v1**:
  - tennis-backhand
  - tennis-forehand
  - tennis-serve
  - tennis-volley
- **ryx.sports.basketball.v1**:
  - basketball-dribble
  - basketball-layup
  - basketball-shot
  - rainbow-flick
- **ryx.sports.football.v1**:
  - football-tackle
  - football-throw
  - rainbow-flick
  - soccer-kick
  - soccer-shoot
  - sprint-blocks
- **ryx.sports.golf.v1**:
  - golf-swing
- **ryx.sports.combat.v1**:
  - boxing-hook
  - boxing-jab
  - triangle-choke
- **ryx.sports.swimming.v1**:
  - freestyle-swim

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
{
  "generated_at": "2026-08-01T09:12:23.324Z",
  "byWedge": {
    "ryx.fitness.general.v1": [
      "ab-wheel",
      "band-pull-apart",
      "barbell-snatch",
      "bench-press",
      "bicep-curl",
      "bird-dog",
      "box-step-up",
      "bulgarian-split-squat",
      "cable-fly",
      "calf-raise",
      "chin-tuck",
      "chin-up",
      "dead-bug",
      "deadlift",
      "dip",
      "dumbbell-bench-press",
      "face-pull",
      "football-throw",
      "front-squat",
      "glute-bridge",
      "goblet-squat",
      "good-morning",
      "hip-cars",
      "hip-hinge-drill",
      "hip-thrust",
      "hollow-body-hold",
      "incline-push-up",
      "indoor-cycling",
      "inverted-row",
      "lat-pulldown",
      "lateral-raise",
      "leg-curl",
      "leg-press",
      "lunge",
      "pallof-press",
      "plank",
      "power-clean",
      "pull-up",
      "push-up",
      "rdl",
      "row",
      "rowing-machine",
      "running-form",
      "shoulder-press",
      "side-plank",
      "spanish-squat",
      "squat",
      "step-up",
      "thoracic-rotation",
      "tricep-pushdown",
      "volley-smash",
      "volleyball-serve",
      "volleyball-set"
    ],
    "ryx.fitness.bodybuilding.v1": [
      "bench-press",
      "dumbbell-bench-press",
      "push-up",
      "rdl",
      "squat"
    ],
    "ryx.fitness.powerlifting.v1": [
      "barbell-snatch",
      "bench-press",
      "deadlift",
      "front-squat",
      "power-clean",
      "rdl",
      "squat"
    ],
    "ryx.wellness.rehab.v1": [
      "90-90-hip-stretch",
      "band-pull-apart",
      "banded-lateral-walk",
      "bird-dog",
      "calf-stretch-achilles",
      "cat-cow",
      "chin-tuck",
      "clamshell",
      "dead-bug",
      "foam-roll-it-band",
      "foam-roll-quads",
      "foam-roll-upper-back",
      "glute-bridge",
      "hip-flexor-stretch",
      "mcgill-big-3",
      "monster-walk",
      "pallof-press",
      "pigeon-stretch",
      "plank",
      "scapular-push-up",
      "sleeper-stretch",
      "spanish-squat",
      "terminal-knee-extension",
      "wall-angel",
      "wall-slide",
      "ytwl-shoulder"
    ],
    "ryx.fitness.calisthenics.v1": [
      "chin-up",
      "pull-up",
      "push-up",
      "worlds-greatest-stretch"
    ],
    "ryx.fitness.crossfit.v1": [
      "barbell-snatch",
      "battle-ropes",
      "box-jump",
      "burpee",
      "farmer-carry",
      "indoor-cycling",
      "jump-rope",
      "kettlebell-swing",
      "mountain-climbers",
      "power-clean",
      "rowing-machine",
      "running-form",
      "sled-push",
      "sprint-blocks",
      "turkish-get-up"
    ],
    "ryx.wellness.yoga.v1": [
      "90-90-hip-stretch",
      "box-breathing",
      "calf-stretch-achilles",
      "cat-cow",
      "childs-pose",
      "diaphragmatic-breathing",
      "downward-dog",
      "figure-four-stretch",
      "hamstring-stretch",
      "hip-cars",
      "hip-flexor-stretch",
      "pigeon-stretch",
      "pilates-hundred",
      "pilates-roll-up",
      "sleeper-stretch",
      "sun-salutation",
      "thoracic-rotation",
      "warrior-2",
      "worlds-greatest-stretch"
    ],
    "ryx.sports.padel.v1": [
      "padel-bandeja",
      "padel-basics",
      "padel-serve",
      "padel-swing",
      "padel-volley",
      "volley-smash"
    ],
    "ryx.sports.tennis.v1": [
      "tennis-backhand",
      "tennis-forehand",
      "tennis-serve",
      "tennis-volley"
    ],
    "ryx.sports.basketball.v1": [
      "basketball-dribble",
      "basketball-layup",
      "basketball-shot",
      "rainbow-flick"
    ],
    "ryx.sports.football.v1": [
      "football-tackle",
      "football-throw",
      "rainbow-flick",
      "soccer-kick",
      "soccer-shoot",
      "sprint-blocks"
    ],
    "ryx.sports.golf.v1": [
      "golf-swing"
    ],
    "ryx.sports.combat.v1": [
      "boxing-hook",
      "boxing-jab",
      "triangle-choke"
    ],
    "ryx.sports.swimming.v1": [
      "freestyle-swim"
    ]
  }
}
```

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/knowledge/data/formDemosByWedge.json` — Complete file (188 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
