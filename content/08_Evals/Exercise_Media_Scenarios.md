---
id: "ryx.eval.exercise_media_scenarios"
title: "Exercise Media Scenarios"
type: "eval"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/evalExerciseMedia.js"
  - "ryx-brain/src/evalExerciseMediaNiches.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
decision_ids:
  - "H08"
  - "H12"
---

# Exercise Media Scenarios

## Reference status

Retained historical/source evidence, excluded from the candidate manifest. It is not an independent canonical instruction or claim of a new passing run. See [[RYX_BRAIN_DECISIONS]] for intended rules and [[Knowledge_System#Future retrieval contract]] / [[Eval_System#Production-quality evaluation contract]] for future integration.

# Exercise Media Scenarios

Original deterministic media query/expected-movement cases, including niche and prior-context variants. Matched ID must equal expectMatch; expected catalog matches require an exercise card, media and a reachable embed in the original harness. Null expectations detect wrong matches and distinguish gaps. No historical result or online availability claim is migrated.

## Item 1

- **source**: ryx-brain/src/evalExerciseMedia.js
- **scenarios**:
  - Item 1:
    - **id**: F01
    - **category**: fitness
    - **query**: How do I bench press
    - **expectMatch**: bench-press
  - Item 2:
    - **id**: F02
    - **category**: fitness
    - **query**: How do I bench
    - **expectMatch**: bench-press
  - Item 3:
    - **id**: F03
    - **category**: fitness
    - **query**: how to do a push up
    - **expectMatch**: push-up
  - Item 4:
    - **id**: F04
    - **category**: fitness
    - **query**: explain incline push-ups
    - **expectMatch**: incline-push-up
  - Item 5:
    - **id**: F05
    - **category**: fitness
    - **query**: how do I goblet squat
    - **expectMatch**: goblet-squat
  - Item 6:
    - **id**: F06
    - **category**: fitness
    - **query**: how to squat properly
    - **expectMatch**: squat
  - Item 7:
    - **id**: F07
    - **category**: fitness
    - **query**: Romanian deadlift form
    - **expectMatch**: rdl
  - Item 8:
    - **id**: F08
    - **category**: fitness
    - **query**: how do I RDL
    - **expectMatch**: rdl
  - Item 9:
    - **id**: F09
    - **category**: fitness
    - **query**: walking lunge technique
    - **expectMatch**: lunge
  - Item 10:
    - **id**: F10
    - **category**: fitness
    - **query**: how to plank
    - **expectMatch**: plank
  - Item 11:
    - **id**: F11
    - **category**: fitness
    - **query**: pull-up form cues
    - **expectMatch**: pull-up
  - Item 12:
    - **id**: F12
    - **category**: fitness
    - **query**: shoulder press technique
    - **expectMatch**: shoulder-press
  - Item 13:
    - **id**: F13
    - **category**: fitness
    - **query**: military press form
    - **expectMatch**: shoulder-press
  - Item 14:
    - **id**: F14
    - **category**: fitness
    - **query**: dumbbell row how to
    - **expectMatch**: row
  - Item 15:
    - **id**: F15
    - **category**: fitness
    - **query**: how to do tricep dips
    - **expectMatch**: dip
  - Item 16:
    - **id**: F16
    - **category**: fitness
    - **query**: how do I hip thrust
    - **expectMatch**: hip-thrust
  - Item 17:
    - **id**: F17
    - **category**: fitness
    - **query**: lat pulldown form
    - **expectMatch**: lat-pulldown
  - Item 18:
    - **id**: F18
    - **category**: fitness
    - **query**: how to leg press
    - **expectMatch**: leg-press
  - Item 19:
    - **id**: F19
    - **category**: fitness
    - **query**: inverted row technique
    - **expectMatch**: inverted-row
  - Item 20:
    - **id**: F20
    - **category**: fitness
    - **query**: farmer carry form
    - **expectMatch**: farmer-carry
  - Item 21:
    - **id**: F21
    - **category**: fitness
    - **query**: how to deadlift
    - **expectMatch**: deadlift
  - Item 22:
    - **id**: F22
    - **category**: fitness
    - **query**: barbell deadlift form
    - **expectMatch**: deadlift
  - Item 23:
    - **id**: S01
    - **category**: sports
    - **query**: how do I serve in padel
    - **expectMatch**: padel-serve
  - Item 24:
    - **id**: S02
    - **category**: sports
    - **query**: tennis forehand technique
    - **expectMatch**: tennis-forehand
  - Item 25:
    - **id**: S03
    - **category**: sports
    - **query**: how to shoot a basketball
    - **expectMatch**: basketball-shot
  - Item 26:
    - **id**: S04
    - **category**: sports
    - **query**: sprint starting blocks form
    - **expectMatch**: sprint-blocks
  - Item 27:
    - **id**: S05
    - **category**: sports
    - **query**: how to swing a golf club
    - **expectMatch**: golf-swing
  - Item 28:
    - **id**: S06
    - **category**: sports
    - **query**: football tackling form
    - **expectMatch**: football-tackle
  - Item 29:
    - **id**: S07
    - **category**: sports
    - **query**: box jump technique
    - **expectMatch**: box-jump
  - Item 30:
    - **id**: S08
    - **category**: sports
    - **query**: sled push form
    - **expectMatch**: sled-push
  - Item 31:
    - **id**: S09
    - **category**: sports
    - **query**: box step up for padel
    - **expectMatch**: box-step-up
  - Item 32:
    - **id**: S10
    - **category**: sports
    - **query**: how to do a burpee
    - **expectMatch**: burpee
  - Item 33:
    - **id**: T01
    - **category**: therapy
    - **query**: dead bug exercise how to
    - **expectMatch**: dead-bug
  - Item 34:
    - **id**: T02
    - **category**: therapy
    - **query**: band pull apart form
    - **expectMatch**: band-pull-apart
  - Item 35:
    - **id**: T03
    - **category**: therapy
    - **query**: clamshell exercise for hip
    - **expectMatch**: clamshell
  - Item 36:
    - **id**: T04
    - **category**: therapy
    - **query**: how to do bird dog
    - **expectMatch**: bird-dog
  - Item 37:
    - **id**: T05
    - **category**: therapy
    - **query**: cat cow stretch technique
    - **expectMatch**: cat-cow
  - Item 38:
    - **id**: T06
    - **category**: therapy
    - **query**: how to foam roll quads
    - **expectMatch**: foam-roll-quads
  - Item 39:
    - **id**: T07
    - **category**: therapy
    - **query**: pallof press anti rotation
    - **expectMatch**: pallof-press
  - Item 40:
    - **id**: T08
    - **category**: therapy
    - **query**: wall slide shoulder rehab
    - **expectMatch**: wall-slide
  - Item 41:
    - **id**: T09
    - **category**: therapy
    - **query**: how to perform a plank for core rehab
    - **expectMatch**: plank
  - Item 42:
    - **id**: T10
    - **category**: therapy
    - **query**: glute bridge for back pain
    - **expectMatch**: glute-bridge
  - Item 43:
    - **id**: E01
    - **category**: edge
    - **query**: push-up
    - **expectMatch**: push-up
    - **needsCard**: true
  - Item 44:
    - **id**: E02
    - **category**: edge
    - **query**: show me squat form
    - **expectMatch**: squat
  - Item 45:
    - **id**: E03
    - **category**: edge
    - **query**: teach me the lunge
    - **expectMatch**: lunge
  - Item 46:
    - **id**: E04
    - **category**: edge
    - **query**: what is proper dip form
    - **expectMatch**: dip
  - Item 47:
    - **id**: E05
    - **category**: edge
    - **query**: how do I row properly
    - **expectMatch**: row
  - Item 48:
    - **id**: E06
    - **category**: edge
    - **query**: give me a workout
    - **expectMatch**: null

## Item 2

- **source**: ryx-brain/src/evalExerciseMediaNiches.js
- **scenarios**:
  - Item 1:
    - **id**: FIT-01
    - **niche**: strength-upper
    - **query**: how do I bench press
    - **expectMatch**: bench-press
  - Item 2:
    - **id**: FIT-02
    - **niche**: strength-upper
    - **query**: push up form
    - **expectMatch**: push-up
  - Item 3:
    - **id**: FIT-03
    - **niche**: strength-upper
    - **query**: incline push-up technique
    - **expectMatch**: incline-push-up
  - Item 4:
    - **id**: FIT-04
    - **niche**: strength-upper
    - **query**: dumbbell row how to
    - **expectMatch**: row
  - Item 5:
    - **id**: FIT-05
    - **niche**: strength-upper
    - **query**: shoulder press form
    - **expectMatch**: shoulder-press
  - Item 6:
    - **id**: FIT-06
    - **niche**: strength-upper
    - **query**: pull-up technique
    - **expectMatch**: pull-up
  - Item 7:
    - **id**: FIT-07
    - **niche**: strength-upper
    - **query**: lat pulldown form
    - **expectMatch**: lat-pulldown
  - Item 8:
    - **id**: FIT-08
    - **niche**: strength-upper
    - **query**: tricep dips form
    - **expectMatch**: dip
  - Item 9:
    - **id**: FIT-09
    - **niche**: strength-lower
    - **query**: how to squat
    - **expectMatch**: squat
  - Item 10:
    - **id**: FIT-10
    - **niche**: strength-lower
    - **query**: goblet squat form
    - **expectMatch**: goblet-squat
  - Item 11:
    - **id**: FIT-11
    - **niche**: strength-lower
    - **query**: hip thrust technique
    - **expectMatch**: hip-thrust
  - Item 12:
    - **id**: FIT-12
    - **niche**: strength-lower
    - **query**: leg press form
    - **expectMatch**: leg-press
  - Item 13:
    - **id**: FIT-13
    - **niche**: strength-lower
    - **query**: Romanian deadlift form
    - **expectMatch**: rdl
  - Item 14:
    - **id**: FIT-14
    - **niche**: strength-lower
    - **query**: barbell deadlift form
    - **expectMatch**: deadlift
  - Item 15:
    - **id**: FIT-15
    - **niche**: strength-lower
    - **query**: walking lunge technique
    - **expectMatch**: lunge
  - Item 16:
    - **id**: FIT-16
    - **niche**: strength-lower
    - **query**: inverted row form
    - **expectMatch**: inverted-row
  - Item 17:
    - **id**: FIT-17
    - **niche**: conditioning
    - **query**: how to do a burpee
    - **expectMatch**: burpee
  - Item 18:
    - **id**: FIT-18
    - **niche**: conditioning
    - **query**: farmer carry form
    - **expectMatch**: farmer-carry
  - Item 19:
    - **id**: FIT-19
    - **niche**: conditioning
    - **query**: box jump technique
    - **expectMatch**: box-jump
  - Item 20:
    - **id**: FIT-20
    - **niche**: conditioning
    - **query**: sled push form
    - **expectMatch**: sled-push
  - Item 21:
    - **id**: FIT-21
    - **niche**: core
    - **query**: how to plank
    - **expectMatch**: plank
  - Item 22:
    - **id**: GAP-F01
    - **niche**: strength-upper
    - **query**: how to bicep curl
    - **expectMatch**: bicep-curl
  - Item 23:
    - **id**: GAP-F02
    - **niche**: strength-upper
    - **query**: tricep pushdown form
    - **expectMatch**: tricep-pushdown
  - Item 24:
    - **id**: GAP-F03
    - **niche**: strength-upper
    - **query**: lateral raise technique
    - **expectMatch**: lateral-raise
  - Item 25:
    - **id**: GAP-F04
    - **niche**: strength-upper
    - **query**: face pull form
    - **expectMatch**: face-pull
  - Item 26:
    - **id**: GAP-F05
    - **niche**: strength-upper
    - **query**: dumbbell bench press form
    - **expectMatch**: dumbbell-bench-press
  - Item 27:
    - **id**: GAP-F06
    - **niche**: strength-upper
    - **query**: cable fly technique
    - **expectMatch**: cable-fly
  - Item 28:
    - **id**: GAP-F07
    - **niche**: strength-upper
    - **query**: chin up form
    - **expectMatch**: chin-up
  - Item 29:
    - **id**: GAP-F08
    - **niche**: strength-lower
    - **query**: front squat form
    - **expectMatch**: front-squat
  - Item 30:
    - **id**: GAP-F09
    - **niche**: strength-lower
    - **query**: Bulgarian split squat technique
    - **expectMatch**: bulgarian-split-squat
  - Item 31:
    - **id**: GAP-F10
    - **niche**: strength-lower
    - **query**: leg curl form
    - **expectMatch**: leg-curl
  - Item 32:
    - **id**: GAP-F11
    - **niche**: strength-lower
    - **query**: calf raise technique
    - **expectMatch**: calf-raise
  - Item 33:
    - **id**: GAP-F12
    - **niche**: strength-lower
    - **query**: hip hinge drill form
    - **expectMatch**: hip-hinge-drill
  - Item 34:
    - **id**: GAP-F13
    - **niche**: strength-lower
    - **query**: good morning exercise form
    - **expectMatch**: good-morning
  - Item 35:
    - **id**: GAP-F14
    - **niche**: kettlebell
    - **query**: kettlebell swing form
    - **expectMatch**: kettlebell-swing
  - Item 36:
    - **id**: GAP-F15
    - **niche**: kettlebell
    - **query**: Turkish get up technique
    - **expectMatch**: turkish-get-up
  - Item 37:
    - **id**: GAP-F16
    - **niche**: olympic
    - **query**: how to power clean
    - **expectMatch**: power-clean
  - Item 38:
    - **id**: GAP-F17
    - **niche**: olympic
    - **query**: barbell snatch form
    - **expectMatch**: barbell-snatch
  - Item 39:
    - **id**: GAP-F18
    - **niche**: conditioning
    - **query**: battle ropes form
    - **expectMatch**: battle-ropes
  - Item 40:
    - **id**: GAP-F19
    - **niche**: conditioning
    - **query**: rowing machine technique
    - **expectMatch**: rowing-machine
  - Item 41:
    - **id**: GAP-F20
    - **niche**: conditioning
    - **query**: jump rope form
    - **expectMatch**: jump-rope
  - Item 42:
    - **id**: GAP-F21
    - **niche**: conditioning
    - **query**: mountain climbers exercise
    - **expectMatch**: mountain-climbers
  - Item 43:
    - **id**: GAP-F22
    - **niche**: core
    - **query**: side plank form
    - **expectMatch**: side-plank
  - Item 44:
    - **id**: GAP-F23
    - **niche**: core
    - **query**: hollow body hold technique
    - **expectMatch**: hollow-body-hold
  - Item 45:
    - **id**: GAP-F24
    - **niche**: core
    - **query**: ab wheel rollout form
    - **expectMatch**: ab-wheel
  - Item 46:
    - **id**: GAP-F25
    - **niche**: mobility-fitness
    - **query**: worlds greatest stretch
    - **expectMatch**: worlds-greatest-stretch
  - Item 47:
    - **id**: SPT-01
    - **niche**: racquet-padel
    - **query**: how do I serve in padel
    - **expectMatch**: padel-serve
  - Item 48:
    - **id**: SPT-02
    - **niche**: racquet-padel
    - **query**: how do i swing the padel racket
    - **expectMatch**: padel-swing
  - Item 49:
    - **id**: SPT-03
    - **niche**: racquet-padel
    - **query**: how to play padel basics
    - **expectMatch**: padel-basics
  - Item 50:
    - **id**: SPT-04
    - **niche**: racquet-tennis
    - **query**: tennis forehand technique
    - **expectMatch**: tennis-forehand
  - Item 51:
    - **id**: SPT-05
    - **niche**: court-basketball
    - **query**: how to shoot a basketball
    - **expectMatch**: basketball-shot
  - Item 52:
    - **id**: SPT-06
    - **niche**: field-golf
    - **query**: how to swing a golf club
    - **expectMatch**: golf-swing
  - Item 53:
    - **id**: SPT-07
    - **niche**: track
    - **query**: sprint starting blocks form
    - **expectMatch**: sprint-blocks
  - Item 54:
    - **id**: SPT-08
    - **niche**: field-football
    - **query**: football tackling form
    - **expectMatch**: football-tackle
  - Item 55:
    - **id**: GAP-S01
    - **niche**: racquet-tennis
    - **query**: tennis backhand technique
    - **expectMatch**: tennis-backhand
  - Item 56:
    - **id**: GAP-S02
    - **niche**: racquet-tennis
    - **query**: tennis serve form
    - **expectMatch**: tennis-serve
  - Item 57:
    - **id**: GAP-S03
    - **niche**: racquet-tennis
    - **query**: tennis volley technique
    - **expectMatch**: tennis-volley
  - Item 58:
    - **id**: GAP-S04
    - **niche**: racquet-padel
    - **query**: padel bandeja shot
    - **expectMatch**: padel-bandeja
  - Item 59:
    - **id**: GAP-S05
    - **niche**: racquet-padel
    - **query**: padel volley form
    - **expectMatch**: padel-volley
  - Item 60:
    - **id**: GAP-S06
    - **niche**: court-basketball
    - **query**: basketball layup form
    - **expectMatch**: basketball-layup
  - Item 61:
    - **id**: GAP-S07
    - **niche**: court-basketball
    - **query**: how to dribble a basketball
    - **expectMatch**: basketball-dribble
  - Item 62:
    - **id**: GAP-S08
    - **niche**: field-soccer
    - **query**: soccer shooting technique
    - **expectMatch**: soccer-shoot
  - Item 63:
    - **id**: GAP-S09
    - **niche**: field-soccer
    - **query**: how to kick a soccer ball
    - **expectMatch**: soccer-kick
  - Item 64:
    - **id**: GAP-S10
    - **niche**: combat
    - **query**: how to throw a jab
    - **expectMatch**: boxing-jab
  - Item 65:
    - **id**: GAP-S11
    - **niche**: combat
    - **query**: boxing hook technique
    - **expectMatch**: boxing-hook
  - Item 66:
    - **id**: GAP-S12
    - **niche**: combat
    - **query**: triangle choke technique
    - **expectMatch**: triangle-choke
  - Item 67:
    - **id**: GAP-S12
    - **niche**: swim
    - **query**: freestyle swimming form
    - **expectMatch**: freestyle-swim
  - Item 68:
    - **id**: GAP-S13
    - **niche**: volleyball
    - **query**: volleyball set technique
    - **expectMatch**: volleyball-set
  - Item 69:
    - **id**: GAP-S14
    - **niche**: racquet-padel
    - **query**: volley smash technique
    - **expectMatch**: volley-smash
  - Item 70:
    - **id**: GAP-S15
    - **niche**: volleyball
    - **query**: volleyball serve technique
    - **expectMatch**: volleyball-serve
  - Item 71:
    - **id**: GAP-S16
    - **niche**: run
    - **query**: proper running form
    - **expectMatch**: running-form
  - Item 72:
    - **id**: GAP-S17
    - **niche**: cycle
    - **query**: indoor cycling form
    - **expectMatch**: indoor-cycling
  - Item 73:
    - **id**: GAP-S18
    - **niche**: field-football
    - **query**: how to throw a football
    - **expectMatch**: football-throw
  - Item 74:
    - **id**: REH-01
    - **niche**: core-rehab
    - **query**: dead bug exercise how to
    - **expectMatch**: dead-bug
  - Item 75:
    - **id**: REH-02
    - **niche**: core-rehab
    - **query**: bird dog form
    - **expectMatch**: bird-dog
  - Item 76:
    - **id**: REH-03
    - **niche**: hip-rehab
    - **query**: clamshell exercise form
    - **expectMatch**: clamshell
  - Item 77:
    - **id**: REH-04
    - **niche**: hip-rehab
    - **query**: glute bridge for back pain
    - **expectMatch**: glute-bridge
  - Item 78:
    - **id**: REH-05
    - **niche**: spine-mobility
    - **query**: cat cow stretch technique
    - **expectMatch**: cat-cow
  - Item 79:
    - **id**: REH-06
    - **niche**: shoulder-rehab
    - **query**: band pull apart form
    - **expectMatch**: band-pull-apart
  - Item 80:
    - **id**: REH-07
    - **niche**: core-rehab
    - **query**: pallof press form
    - **expectMatch**: pallof-press
  - Item 81:
    - **id**: REH-08
    - **niche**: shoulder-rehab
    - **query**: wall slide shoulder rehab
    - **expectMatch**: wall-slide
  - Item 82:
    - **id**: REH-09
    - **niche**: soft-tissue
    - **query**: how to foam roll quads
    - **expectMatch**: foam-roll-quads
  - Item 83:
    - **id**: REH-10
    - **niche**: core-rehab
    - **query**: plank for core rehab
    - **expectMatch**: plank
  - Item 84:
    - **id**: GAP-R01
    - **niche**: soft-tissue
    - **query**: foam roll IT band
    - **expectMatch**: foam-roll-it-band
  - Item 85:
    - **id**: GAP-R02
    - **niche**: soft-tissue
    - **query**: foam roll upper back
    - **expectMatch**: foam-roll-upper-back
  - Item 86:
    - **id**: GAP-R03
    - **niche**: hip-rehab
    - **query**: 90 90 hip stretch
    - **expectMatch**: 90-90-hip-stretch
  - Item 87:
    - **id**: GAP-R04
    - **niche**: hip-rehab
    - **query**: pigeon stretch form
    - **expectMatch**: pigeon-stretch
  - Item 88:
    - **id**: GAP-R05
    - **niche**: hip-rehab
    - **query**: hip flexor stretch technique
    - **expectMatch**: hip-flexor-stretch
  - Item 89:
    - **id**: GAP-R06
    - **niche**: shoulder-rehab
    - **query**: scapular push up form
    - **expectMatch**: scapular-push-up
  - Item 90:
    - **id**: GAP-R07
    - **niche**: shoulder-rehab
    - **query**: YTWL shoulder exercise
    - **expectMatch**: ytwl-shoulder
  - Item 91:
    - **id**: GAP-R08
    - **niche**: shoulder-rehab
    - **query**: sleeper stretch shoulder
    - **expectMatch**: sleeper-stretch
  - Item 92:
    - **id**: GAP-R09
    - **niche**: spine-rehab
    - **query**: McGill big 3 exercises
    - **expectMatch**: mcgill-big-3
  - Item 93:
    - **id**: GAP-R10
    - **niche**: knee-rehab
    - **query**: terminal knee extension exercise
    - **expectMatch**: terminal-knee-extension
  - Item 94:
    - **id**: GAP-R11
    - **niche**: knee-rehab
    - **query**: Spanish squat form
    - **expectMatch**: spanish-squat
  - Item 95:
    - **id**: GAP-R12
    - **niche**: ankle-rehab
    - **query**: calf stretch for Achilles
    - **expectMatch**: calf-stretch-achilles
  - Item 96:
    - **id**: GAP-R13
    - **niche**: glute-activation
    - **query**: banded lateral walk form
    - **expectMatch**: banded-lateral-walk
  - Item 97:
    - **id**: GAP-R14
    - **niche**: glute-activation
    - **query**: monster walk exercise
    - **expectMatch**: monster-walk
  - Item 98:
    - **id**: GAP-R15
    - **niche**: posture
    - **query**: wall angel exercise form
    - **expectMatch**: wall-angel
  - Item 99:
    - **id**: GAP-R16
    - **niche**: neck
    - **query**: chin tuck exercise for neck pain
    - **expectMatch**: chin-tuck
  - Item 100:
    - **id**: GAP-W01
    - **niche**: yoga
    - **query**: downward dog form
    - **expectMatch**: downward-dog
  - Item 101:
    - **id**: GAP-W02
    - **niche**: yoga
    - **query**: sun salutation tutorial
    - **expectMatch**: sun-salutation
  - Item 102:
    - **id**: GAP-W03
    - **niche**: yoga
    - **query**: warrior 2 pose alignment
    - **expectMatch**: warrior-2
  - Item 103:
    - **id**: GAP-W04
    - **niche**: yoga
    - **query**: childs pose stretch
    - **expectMatch**: childs-pose
  - Item 104:
    - **id**: GAP-W05
    - **niche**: pilates
    - **query**: pilates hundred exercise
    - **expectMatch**: pilates-hundred
  - Item 105:
    - **id**: GAP-W06
    - **niche**: pilates
    - **query**: pilates roll up form
    - **expectMatch**: pilates-roll-up
  - Item 106:
    - **id**: GAP-W07
    - **niche**: mobility-wellness
    - **query**: thoracic rotation stretch
    - **expectMatch**: thoracic-rotation
  - Item 107:
    - **id**: GAP-W08
    - **niche**: mobility-wellness
    - **query**: hip CARs mobility
    - **expectMatch**: hip-cars
  - Item 108:
    - **id**: GAP-W09
    - **niche**: breathwork
    - **query**: diaphragmatic breathing exercise
    - **expectMatch**: diaphragmatic-breathing
  - Item 109:
    - **id**: GAP-W10
    - **niche**: breathwork
    - **query**: box breathing technique
    - **expectMatch**: box-breathing
  - Item 110:
    - **id**: GAP-W11
    - **niche**: stretching
    - **query**: hamstring stretch form
    - **expectMatch**: hamstring-stretch
  - Item 111:
    - **id**: GAP-W12
    - **niche**: stretching
    - **query**: figure four stretch glute
    - **expectMatch**: figure-four-stretch
  - Item 112:
    - **id**: CTX-01
    - **niche**: racquet-padel
    - **query**: I want to know the basics
    - **expectMatch**: padel-basics
    - **context**: how do i swing the padel racket
  - Item 113:
    - **id**: CTX-02
    - **niche**: racquet-padel
    - **query**: can you show me how to play
    - **expectMatch**: padel-basics
    - **context**: how do i swing the padel racket
  - Item 114:
    - **id**: CTX-03
    - **niche**: court-basketball
    - **query**: what about how to do a rainbow flick
    - **expectMatch**: rainbow-flick
    - **context**: show me how to shoot a basketball
  - Item 115:
    - **id**: CTX-04
    - **niche**: combat
    - **query**: what about a triangle choke
    - **expectMatch**: triangle-choke
    - **context**: Show me how to do the downward dog how do i do a lay up
  - Item 116:
    - **id**: CTX-05
    - **niche**: volleyball
    - **query**: show me a video
    - **expectMatch**: volleyball-set
    - **context**: what about a set in volleyball
  - Item 117:
    - **id**: EDGE-01
    - **niche**: meta
    - **query**: give me a workout
    - **expectMatch**: null

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
[
  {
    "source": "ryx-brain/src/evalExerciseMedia.js",
    "scenarios": [
      {
        "id": "F01",
        "category": "fitness",
        "query": "How do I bench press",
        "expectMatch": "bench-press"
      },
      {
        "id": "F02",
        "category": "fitness",
        "query": "How do I bench",
        "expectMatch": "bench-press"
      },
      {
        "id": "F03",
        "category": "fitness",
        "query": "how to do a push up",
        "expectMatch": "push-up"
      },
      {
        "id": "F04",
        "category": "fitness",
        "query": "explain incline push-ups",
        "expectMatch": "incline-push-up"
      },
      {
        "id": "F05",
        "category": "fitness",
        "query": "how do I goblet squat",
        "expectMatch": "goblet-squat"
      },
      {
        "id": "F06",
        "category": "fitness",
        "query": "how to squat properly",
        "expectMatch": "squat"
      },
      {
        "id": "F07",
        "category": "fitness",
        "query": "Romanian deadlift form",
        "expectMatch": "rdl"
      },
      {
        "id": "F08",
        "category": "fitness",
        "query": "how do I RDL",
        "expectMatch": "rdl"
      },
      {
        "id": "F09",
        "category": "fitness",
        "query": "walking lunge technique",
        "expectMatch": "lunge"
      },
      {
        "id": "F10",
        "category": "fitness",
        "query": "how to plank",
        "expectMatch": "plank"
      },
      {
        "id": "F11",
        "category": "fitness",
        "query": "pull-up form cues",
        "expectMatch": "pull-up"
      },
      {
        "id": "F12",
        "category": "fitness",
        "query": "shoulder press technique",
        "expectMatch": "shoulder-press"
      },
      {
        "id": "F13",
        "category": "fitness",
        "query": "military press form",
        "expectMatch": "shoulder-press"
      },
      {
        "id": "F14",
        "category": "fitness",
        "query": "dumbbell row how to",
        "expectMatch": "row"
      },
      {
        "id": "F15",
        "category": "fitness",
        "query": "how to do tricep dips",
        "expectMatch": "dip"
      },
      {
        "id": "F16",
        "category": "fitness",
        "query": "how do I hip thrust",
        "expectMatch": "hip-thrust"
      },
      {
        "id": "F17",
        "category": "fitness",
        "query": "lat pulldown form",
        "expectMatch": "lat-pulldown"
      },
      {
        "id": "F18",
        "category": "fitness",
        "query": "how to leg press",
        "expectMatch": "leg-press"
      },
      {
        "id": "F19",
        "category": "fitness",
        "query": "inverted row technique",
        "expectMatch": "inverted-row"
      },
      {
        "id": "F20",
        "category": "fitness",
        "query": "farmer carry form",
        "expectMatch": "farmer-carry"
      },
      {
        "id": "F21",
        "category": "fitness",
        "query": "how to deadlift",
        "expectMatch": "deadlift"
      },
      {
        "id": "F22",
        "category": "fitness",
        "query": "barbell deadlift form",
        "expectMatch": "deadlift"
      },
      {
        "id": "S01",
        "category": "sports",
        "query": "how do I serve in padel",
        "expectMatch": "padel-serve"
      },
      {
        "id": "S02",
        "category": "sports",
        "query": "tennis forehand technique",
        "expectMatch": "tennis-forehand"
      },
      {
        "id": "S03",
        "category": "sports",
        "query": "how to shoot a basketball",
        "expectMatch": "basketball-shot"
      },
      {
        "id": "S04",
        "category": "sports",
        "query": "sprint starting blocks form",
        "expectMatch": "sprint-blocks"
      },
      {
        "id": "S05",
        "category": "sports",
        "query": "how to swing a golf club",
        "expectMatch": "golf-swing"
      },
      {
        "id": "S06",
        "category": "sports",
        "query": "football tackling form",
        "expectMatch": "football-tackle"
      },
      {
        "id": "S07",
        "category": "sports",
        "query": "box jump technique",
        "expectMatch": "box-jump"
      },
      {
        "id": "S08",
        "category": "sports",
        "query": "sled push form",
        "expectMatch": "sled-push"
      },
      {
        "id": "S09",
        "category": "sports",
        "query": "box step up for padel",
        "expectMatch": "box-step-up"
      },
      {
        "id": "S10",
        "category": "sports",
        "query": "how to do a burpee",
        "expectMatch": "burpee"
      },
      {
        "id": "T01",
        "category": "therapy",
        "query": "dead bug exercise how to",
        "expectMatch": "dead-bug"
      },
      {
        "id": "T02",
        "category": "therapy",
        "query": "band pull apart form",
        "expectMatch": "band-pull-apart"
      },
      {
        "id": "T03",
        "category": "therapy",
        "query": "clamshell exercise for hip",
        "expectMatch": "clamshell"
      },
      {
        "id": "T04",
        "category": "therapy",
        "query": "how to do bird dog",
        "expectMatch": "bird-dog"
      },
      {
        "id": "T05",
        "category": "therapy",
        "query": "cat cow stretch technique",
        "expectMatch": "cat-cow"
      },
      {
        "id": "T06",
        "category": "therapy",
        "query": "how to foam roll quads",
        "expectMatch": "foam-roll-quads"
      },
      {
        "id": "T07",
        "category": "therapy",
        "query": "pallof press anti rotation",
        "expectMatch": "pallof-press"
      },
      {
        "id": "T08",
        "category": "therapy",
        "query": "wall slide shoulder rehab",
        "expectMatch": "wall-slide"
      },
      {
        "id": "T09",
        "category": "therapy",
        "query": "how to perform a plank for core rehab",
        "expectMatch": "plank"
      },
      {
        "id": "T10",
        "category": "therapy",
        "query": "glute bridge for back pain",
        "expectMatch": "glute-bridge"
      },
      {
        "id": "E01",
        "category": "edge",
        "query": "push-up",
        "expectMatch": "push-up",
        "needsCard": true
      },
      {
        "id": "E02",
        "category": "edge",
        "query": "show me squat form",
        "expectMatch": "squat"
      },
      {
        "id": "E03",
        "category": "edge",
        "query": "teach me the lunge",
        "expectMatch": "lunge"
      },
      {
        "id": "E04",
        "category": "edge",
        "query": "what is proper dip form",
        "expectMatch": "dip"
      },
      {
        "id": "E05",
        "category": "edge",
        "query": "how do I row properly",
        "expectMatch": "row"
      },
      {
        "id": "E06",
        "category": "edge",
        "query": "give me a workout",
        "expectMatch": null
      }
    ]
  },
  {
    "source": "ryx-brain/src/evalExerciseMediaNiches.js",
    "scenarios": [
      {
        "id": "FIT-01",
        "niche": "strength-upper",
        "query": "how do I bench press",
        "expectMatch": "bench-press"
      },
      {
        "id": "FIT-02",
        "niche": "strength-upper",
        "query": "push up form",
        "expectMatch": "push-up"
      },
      {
        "id": "FIT-03",
        "niche": "strength-upper",
        "query": "incline push-up technique",
        "expectMatch": "incline-push-up"
      },
      {
        "id": "FIT-04",
        "niche": "strength-upper",
        "query": "dumbbell row how to",
        "expectMatch": "row"
      },
      {
        "id": "FIT-05",
        "niche": "strength-upper",
        "query": "shoulder press form",
        "expectMatch": "shoulder-press"
      },
      {
        "id": "FIT-06",
        "niche": "strength-upper",
        "query": "pull-up technique",
        "expectMatch": "pull-up"
      },
      {
        "id": "FIT-07",
        "niche": "strength-upper",
        "query": "lat pulldown form",
        "expectMatch": "lat-pulldown"
      },
      {
        "id": "FIT-08",
        "niche": "strength-upper",
        "query": "tricep dips form",
        "expectMatch": "dip"
      },
      {
        "id": "FIT-09",
        "niche": "strength-lower",
        "query": "how to squat",
        "expectMatch": "squat"
      },
      {
        "id": "FIT-10",
        "niche": "strength-lower",
        "query": "goblet squat form",
        "expectMatch": "goblet-squat"
      },
      {
        "id": "FIT-11",
        "niche": "strength-lower",
        "query": "hip thrust technique",
        "expectMatch": "hip-thrust"
      },
      {
        "id": "FIT-12",
        "niche": "strength-lower",
        "query": "leg press form",
        "expectMatch": "leg-press"
      },
      {
        "id": "FIT-13",
        "niche": "strength-lower",
        "query": "Romanian deadlift form",
        "expectMatch": "rdl"
      },
      {
        "id": "FIT-14",
        "niche": "strength-lower",
        "query": "barbell deadlift form",
        "expectMatch": "deadlift"
      },
      {
        "id": "FIT-15",
        "niche": "strength-lower",
        "query": "walking lunge technique",
        "expectMatch": "lunge"
      },
      {
        "id": "FIT-16",
        "niche": "strength-lower",
        "query": "inverted row form",
        "expectMatch": "inverted-row"
      },
      {
        "id": "FIT-17",
        "niche": "conditioning",
        "query": "how to do a burpee",
        "expectMatch": "burpee"
      },
      {
        "id": "FIT-18",
        "niche": "conditioning",
        "query": "farmer carry form",
        "expectMatch": "farmer-carry"
      },
      {
        "id": "FIT-19",
        "niche": "conditioning",
        "query": "box jump technique",
        "expectMatch": "box-jump"
      },
      {
        "id": "FIT-20",
        "niche": "conditioning",
        "query": "sled push form",
        "expectMatch": "sled-push"
      },
      {
        "id": "FIT-21",
        "niche": "core",
        "query": "how to plank",
        "expectMatch": "plank"
      },
      {
        "id": "GAP-F01",
        "niche": "strength-upper",
        "query": "how to bicep curl",
        "expectMatch": "bicep-curl"
      },
      {
        "id": "GAP-F02",
        "niche": "strength-upper",
        "query": "tricep pushdown form",
        "expectMatch": "tricep-pushdown"
      },
      {
        "id": "GAP-F03",
        "niche": "strength-upper",
        "query": "lateral raise technique",
        "expectMatch": "lateral-raise"
      },
      {
        "id": "GAP-F04",
        "niche": "strength-upper",
        "query": "face pull form",
        "expectMatch": "face-pull"
      },
      {
        "id": "GAP-F05",
        "niche": "strength-upper",
        "query": "dumbbell bench press form",
        "expectMatch": "dumbbell-bench-press"
      },
      {
        "id": "GAP-F06",
        "niche": "strength-upper",
        "query": "cable fly technique",
        "expectMatch": "cable-fly"
      },
      {
        "id": "GAP-F07",
        "niche": "strength-upper",
        "query": "chin up form",
        "expectMatch": "chin-up"
      },
      {
        "id": "GAP-F08",
        "niche": "strength-lower",
        "query": "front squat form",
        "expectMatch": "front-squat"
      },
      {
        "id": "GAP-F09",
        "niche": "strength-lower",
        "query": "Bulgarian split squat technique",
        "expectMatch": "bulgarian-split-squat"
      },
      {
        "id": "GAP-F10",
        "niche": "strength-lower",
        "query": "leg curl form",
        "expectMatch": "leg-curl"
      },
      {
        "id": "GAP-F11",
        "niche": "strength-lower",
        "query": "calf raise technique",
        "expectMatch": "calf-raise"
      },
      {
        "id": "GAP-F12",
        "niche": "strength-lower",
        "query": "hip hinge drill form",
        "expectMatch": "hip-hinge-drill"
      },
      {
        "id": "GAP-F13",
        "niche": "strength-lower",
        "query": "good morning exercise form",
        "expectMatch": "good-morning"
      },
      {
        "id": "GAP-F14",
        "niche": "kettlebell",
        "query": "kettlebell swing form",
        "expectMatch": "kettlebell-swing"
      },
      {
        "id": "GAP-F15",
        "niche": "kettlebell",
        "query": "Turkish get up technique",
        "expectMatch": "turkish-get-up"
      },
      {
        "id": "GAP-F16",
        "niche": "olympic",
        "query": "how to power clean",
        "expectMatch": "power-clean"
      },
      {
        "id": "GAP-F17",
        "niche": "olympic",
        "query": "barbell snatch form",
        "expectMatch": "barbell-snatch"
      },
      {
        "id": "GAP-F18",
        "niche": "conditioning",
        "query": "battle ropes form",
        "expectMatch": "battle-ropes"
      },
      {
        "id": "GAP-F19",
        "niche": "conditioning",
        "query": "rowing machine technique",
        "expectMatch": "rowing-machine"
      },
      {
        "id": "GAP-F20",
        "niche": "conditioning",
        "query": "jump rope form",
        "expectMatch": "jump-rope"
      },
      {
        "id": "GAP-F21",
        "niche": "conditioning",
        "query": "mountain climbers exercise",
        "expectMatch": "mountain-climbers"
      },
      {
        "id": "GAP-F22",
        "niche": "core",
        "query": "side plank form",
        "expectMatch": "side-plank"
      },
      {
        "id": "GAP-F23",
        "niche": "core",
        "query": "hollow body hold technique",
        "expectMatch": "hollow-body-hold"
      },
      {
        "id": "GAP-F24",
        "niche": "core",
        "query": "ab wheel rollout form",
        "expectMatch": "ab-wheel"
      },
      {
        "id": "GAP-F25",
        "niche": "mobility-fitness",
        "query": "worlds greatest stretch",
        "expectMatch": "worlds-greatest-stretch"
      },
      {
        "id": "SPT-01",
        "niche": "racquet-padel",
        "query": "how do I serve in padel",
        "expectMatch": "padel-serve"
      },
      {
        "id": "SPT-02",
        "niche": "racquet-padel",
        "query": "how do i swing the padel racket",
        "expectMatch": "padel-swing"
      },
      {
        "id": "SPT-03",
        "niche": "racquet-padel",
        "query": "how to play padel basics",
        "expectMatch": "padel-basics"
      },
      {
        "id": "SPT-04",
        "niche": "racquet-tennis",
        "query": "tennis forehand technique",
        "expectMatch": "tennis-forehand"
      },
      {
        "id": "SPT-05",
        "niche": "court-basketball",
        "query": "how to shoot a basketball",
        "expectMatch": "basketball-shot"
      },
      {
        "id": "SPT-06",
        "niche": "field-golf",
        "query": "how to swing a golf club",
        "expectMatch": "golf-swing"
      },
      {
        "id": "SPT-07",
        "niche": "track",
        "query": "sprint starting blocks form",
        "expectMatch": "sprint-blocks"
      },
      {
        "id": "SPT-08",
        "niche": "field-football",
        "query": "football tackling form",
        "expectMatch": "football-tackle"
      },
      {
        "id": "GAP-S01",
        "niche": "racquet-tennis",
        "query": "tennis backhand technique",
        "expectMatch": "tennis-backhand"
      },
      {
        "id": "GAP-S02",
        "niche": "racquet-tennis",
        "query": "tennis serve form",
        "expectMatch": "tennis-serve"
      },
      {
        "id": "GAP-S03",
        "niche": "racquet-tennis",
        "query": "tennis volley technique",
        "expectMatch": "tennis-volley"
      },
      {
        "id": "GAP-S04",
        "niche": "racquet-padel",
        "query": "padel bandeja shot",
        "expectMatch": "padel-bandeja"
      },
      {
        "id": "GAP-S05",
        "niche": "racquet-padel",
        "query": "padel volley form",
        "expectMatch": "padel-volley"
      },
      {
        "id": "GAP-S06",
        "niche": "court-basketball",
        "query": "basketball layup form",
        "expectMatch": "basketball-layup"
      },
      {
        "id": "GAP-S07",
        "niche": "court-basketball",
        "query": "how to dribble a basketball",
        "expectMatch": "basketball-dribble"
      },
      {
        "id": "GAP-S08",
        "niche": "field-soccer",
        "query": "soccer shooting technique",
        "expectMatch": "soccer-shoot"
      },
      {
        "id": "GAP-S09",
        "niche": "field-soccer",
        "query": "how to kick a soccer ball",
        "expectMatch": "soccer-kick"
      },
      {
        "id": "GAP-S10",
        "niche": "combat",
        "query": "how to throw a jab",
        "expectMatch": "boxing-jab"
      },
      {
        "id": "GAP-S11",
        "niche": "combat",
        "query": "boxing hook technique",
        "expectMatch": "boxing-hook"
      },
      {
        "id": "GAP-S12",
        "niche": "combat",
        "query": "triangle choke technique",
        "expectMatch": "triangle-choke"
      },
      {
        "id": "GAP-S12",
        "niche": "swim",
        "query": "freestyle swimming form",
        "expectMatch": "freestyle-swim"
      },
      {
        "id": "GAP-S13",
        "niche": "volleyball",
        "query": "volleyball set technique",
        "expectMatch": "volleyball-set"
      },
      {
        "id": "GAP-S14",
        "niche": "racquet-padel",
        "query": "volley smash technique",
        "expectMatch": "volley-smash"
      },
      {
        "id": "GAP-S15",
        "niche": "volleyball",
        "query": "volleyball serve technique",
        "expectMatch": "volleyball-serve"
      },
      {
        "id": "GAP-S16",
        "niche": "run",
        "query": "proper running form",
        "expectMatch": "running-form"
      },
      {
        "id": "GAP-S17",
        "niche": "cycle",
        "query": "indoor cycling form",
        "expectMatch": "indoor-cycling"
      },
      {
        "id": "GAP-S18",
        "niche": "field-football",
        "query": "how to throw a football",
        "expectMatch": "football-throw"
      },
      {
        "id": "REH-01",
        "niche": "core-rehab",
        "query": "dead bug exercise how to",
        "expectMatch": "dead-bug"
      },
      {
        "id": "REH-02",
        "niche": "core-rehab",
        "query": "bird dog form",
        "expectMatch": "bird-dog"
      },
      {
        "id": "REH-03",
        "niche": "hip-rehab",
        "query": "clamshell exercise form",
        "expectMatch": "clamshell"
      },
      {
        "id": "REH-04",
        "niche": "hip-rehab",
        "query": "glute bridge for back pain",
        "expectMatch": "glute-bridge"
      },
      {
        "id": "REH-05",
        "niche": "spine-mobility",
        "query": "cat cow stretch technique",
        "expectMatch": "cat-cow"
      },
      {
        "id": "REH-06",
        "niche": "shoulder-rehab",
        "query": "band pull apart form",
        "expectMatch": "band-pull-apart"
      },
      {
        "id": "REH-07",
        "niche": "core-rehab",
        "query": "pallof press form",
        "expectMatch": "pallof-press"
      },
      {
        "id": "REH-08",
        "niche": "shoulder-rehab",
        "query": "wall slide shoulder rehab",
        "expectMatch": "wall-slide"
      },
      {
        "id": "REH-09",
        "niche": "soft-tissue",
        "query": "how to foam roll quads",
        "expectMatch": "foam-roll-quads"
      },
      {
        "id": "REH-10",
        "niche": "core-rehab",
        "query": "plank for core rehab",
        "expectMatch": "plank"
      },
      {
        "id": "GAP-R01",
        "niche": "soft-tissue",
        "query": "foam roll IT band",
        "expectMatch": "foam-roll-it-band"
      },
      {
        "id": "GAP-R02",
        "niche": "soft-tissue",
        "query": "foam roll upper back",
        "expectMatch": "foam-roll-upper-back"
      },
      {
        "id": "GAP-R03",
        "niche": "hip-rehab",
        "query": "90 90 hip stretch",
        "expectMatch": "90-90-hip-stretch"
      },
      {
        "id": "GAP-R04",
        "niche": "hip-rehab",
        "query": "pigeon stretch form",
        "expectMatch": "pigeon-stretch"
      },
      {
        "id": "GAP-R05",
        "niche": "hip-rehab",
        "query": "hip flexor stretch technique",
        "expectMatch": "hip-flexor-stretch"
      },
      {
        "id": "GAP-R06",
        "niche": "shoulder-rehab",
        "query": "scapular push up form",
        "expectMatch": "scapular-push-up"
      },
      {
        "id": "GAP-R07",
        "niche": "shoulder-rehab",
        "query": "YTWL shoulder exercise",
        "expectMatch": "ytwl-shoulder"
      },
      {
        "id": "GAP-R08",
        "niche": "shoulder-rehab",
        "query": "sleeper stretch shoulder",
        "expectMatch": "sleeper-stretch"
      },
      {
        "id": "GAP-R09",
        "niche": "spine-rehab",
        "query": "McGill big 3 exercises",
        "expectMatch": "mcgill-big-3"
      },
      {
        "id": "GAP-R10",
        "niche": "knee-rehab",
        "query": "terminal knee extension exercise",
        "expectMatch": "terminal-knee-extension"
      },
      {
        "id": "GAP-R11",
        "niche": "knee-rehab",
        "query": "Spanish squat form",
        "expectMatch": "spanish-squat"
      },
      {
        "id": "GAP-R12",
        "niche": "ankle-rehab",
        "query": "calf stretch for Achilles",
        "expectMatch": "calf-stretch-achilles"
      },
      {
        "id": "GAP-R13",
        "niche": "glute-activation",
        "query": "banded lateral walk form",
        "expectMatch": "banded-lateral-walk"
      },
      {
        "id": "GAP-R14",
        "niche": "glute-activation",
        "query": "monster walk exercise",
        "expectMatch": "monster-walk"
      },
      {
        "id": "GAP-R15",
        "niche": "posture",
        "query": "wall angel exercise form",
        "expectMatch": "wall-angel"
      },
      {
        "id": "GAP-R16",
        "niche": "neck",
        "query": "chin tuck exercise for neck pain",
        "expectMatch": "chin-tuck"
      },
      {
        "id": "GAP-W01",
        "niche": "yoga",
        "query": "downward dog form",
        "expectMatch": "downward-dog"
      },
      {
        "id": "GAP-W02",
        "niche": "yoga",
        "query": "sun salutation tutorial",
        "expectMatch": "sun-salutation"
      },
      {
        "id": "GAP-W03",
        "niche": "yoga",
        "query": "warrior 2 pose alignment",
        "expectMatch": "warrior-2"
      },
      {
        "id": "GAP-W04",
        "niche": "yoga",
        "query": "childs pose stretch",
        "expectMatch": "childs-pose"
      },
      {
        "id": "GAP-W05",
        "niche": "pilates",
        "query": "pilates hundred exercise",
        "expectMatch": "pilates-hundred"
      },
      {
        "id": "GAP-W06",
        "niche": "pilates",
        "query": "pilates roll up form",
        "expectMatch": "pilates-roll-up"
      },
      {
        "id": "GAP-W07",
        "niche": "mobility-wellness",
        "query": "thoracic rotation stretch",
        "expectMatch": "thoracic-rotation"
      },
      {
        "id": "GAP-W08",
        "niche": "mobility-wellness",
        "query": "hip CARs mobility",
        "expectMatch": "hip-cars"
      },
      {
        "id": "GAP-W09",
        "niche": "breathwork",
        "query": "diaphragmatic breathing exercise",
        "expectMatch": "diaphragmatic-breathing"
      },
      {
        "id": "GAP-W10",
        "niche": "breathwork",
        "query": "box breathing technique",
        "expectMatch": "box-breathing"
      },
      {
        "id": "GAP-W11",
        "niche": "stretching",
        "query": "hamstring stretch form",
        "expectMatch": "hamstring-stretch"
      },
      {
        "id": "GAP-W12",
        "niche": "stretching",
        "query": "figure four stretch glute",
        "expectMatch": "figure-four-stretch"
      },
      {
        "id": "CTX-01",
        "niche": "racquet-padel",
        "query": "I want to know the basics",
        "expectMatch": "padel-basics",
        "context": "how do i swing the padel racket"
      },
      {
        "id": "CTX-02",
        "niche": "racquet-padel",
        "query": "can you show me how to play",
        "expectMatch": "padel-basics",
        "context": "how do i swing the padel racket"
      },
      {
        "id": "CTX-03",
        "niche": "court-basketball",
        "query": "what about how to do a rainbow flick",
        "expectMatch": "rainbow-flick",
        "context": "show me how to shoot a basketball"
      },
      {
        "id": "CTX-04",
        "niche": "combat",
        "query": "what about a triangle choke",
        "expectMatch": "triangle-choke",
        "context": "Show me how to do the downward dog how do i do a lay up"
      },
      {
        "id": "CTX-05",
        "niche": "volleyball",
        "query": "show me a video",
        "expectMatch": "volleyball-set",
        "context": "what about a set in volleyball"
      },
      {
        "id": "EDGE-01",
        "niche": "meta",
        "query": "give me a workout",
        "expectMatch": null
      }
    ]
  }
]
```

## Source reference

- `ryx-brain/src/evalExerciseMedia.js` — Complete file (176 lines)
- `ryx-brain/src/evalExerciseMediaNiches.js` — Complete file (324 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
