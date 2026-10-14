---
id: "ryx.knowledge.exercise_library"
title: "Exercise Library"
type: "knowledge"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/knowledge/data/exercises.json"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H04"
  - "H11"
  - "H12"
---

# Exercise Library

## Canonical interpretation and retained source

Canonical rule: [[Knowledge_System#Provenance and evidence]]; [[Knowledge_System#Future retrieval contract]]. Apply [[Brain_Architecture#Global instruction precedence]], [[Data_Boundary#Data truth precedence]], [[Pain_and_Injury#Active pain and clearance]] and [[Athlete_Profile#Confirmed equipment]] before using this lower-priority knowledge. Complete source payloads below remain unchanged; they do not create user facts or override safety/access/tier constraints.

# Exercise Library

Curated supporting movement names, identifiers, equipment/level tags, cues, regressions and avoidIf caveats. All 18 entries are retained. These names support exact prescription wording; the retriever scores suitability but does not enforce a strict equipment filter. Core pain/clearance policy still applies. See [[Knowledge_System]] and [[Exercise_Media_Catalog]].

## Goblet squat

- **id**: goblet-squat
- **name**: Goblet squat
- **equipment**:
  - dumbbell
  - kettlebell
  - home
- **muscles**:
  - quads
  - glutes
  - core
- **level**:
  - beginner
  - intermediate
- **tags**:
  - squat
  - legs
  - lower
  - home
  - muscle
  - fat-loss
  - general
- **cues**: Hold weight at chest, elbows inside knees, sit between hips, full foot pressure.
- **regressions**: Box squat or sit-to-stand from a chair.
- **progressions**: Front squat or split squat.
- **avoidIf**: Acute knee pain without clearance; scale depth.

## Romanian deadlift (dumbbells)

- **id**: rdl-dumbbell
- **name**: Romanian deadlift (dumbbells)
- **equipment**:
  - dumbbell
  - home
- **muscles**:
  - hamstrings
  - glutes
  - back
- **level**:
  - beginner
  - intermediate
  - advanced
- **tags**:
  - hinge
  - legs
  - posterior
  - home
  - muscle
  - hypertrophy
- **cues**: Soft knees, hips back, bar/DBs close to legs, stop when hamstrings stretch.
- **regressions**: Hip hinge drill with dowel on back.
- **progressions**: Barbell RDL.
- **avoidIf**: Sharp low-back pain; reduce range and load.

## Dumbbell bench press

- **id**: db-bench-press
- **name**: Dumbbell bench press
- **equipment**:
  - dumbbell
  - home
  - gym
- **muscles**:
  - chest
  - shoulders
  - triceps
- **level**:
  - beginner
  - intermediate
  - advanced
- **tags**:
  - push
  - upper
  - chest
  - muscle
  - hypertrophy
  - home
- **cues**: Shoulder blades pinched, feet planted, control descent, neutral wrists.
- **regressions**: Floor press or incline push-up.
- **progressions**: Barbell bench with spotter setup.
- **avoidIf**: Shoulder impingement symptoms — use neutral-grip floor press.

## Push-up

- **id**: push-up
- **name**: Push-up
- **equipment**:
  - bodyweight
  - home
  - none
- **muscles**:
  - chest
  - shoulders
  - triceps
  - core
- **level**:
  - beginner
  - intermediate
- **tags**:
  - push
  - upper
  - bodyweight
  - home
  - beginner
  - general
- **cues**: Ribs down, glutes on, hands under shoulders, full body line.
- **regressions**: Incline push-up on bench or wall.
- **progressions**: Deficit or weighted push-up.
- **avoidIf**: Wrist pain — use handles or fists neutral.

## Inverted row (bar or rings)

- **id**: inverted-row
- **name**: Inverted row (bar or rings)
- **equipment**:
  - gym
  - home
  - bar
- **muscles**:
  - back
  - biceps
  - rear-delts
- **level**:
  - beginner
  - intermediate
- **tags**:
  - pull
  - upper
  - back
  - home
  - muscle
- **cues**: Chest to bar, squeeze shoulder blades, avoid shrugging.
- **regressions**: Bent-over dumbbell row.
- **progressions**: Weighted row or pull-up progression.
- **avoidIf**: Shoulder instability — reduce range.

## Dumbbell shoulder press

- **id**: db-shoulder-press
- **name**: Dumbbell shoulder press
- **equipment**:
  - dumbbell
  - home
  - gym
- **muscles**:
  - shoulders
  - triceps
- **level**:
  - intermediate
  - advanced
- **tags**:
  - push
  - upper
  - shoulders
  - muscle
- **cues**: Ribs down, press up and slightly back, no lower-back arch.
- **regressions**: Half-kneeling single-arm press.
- **progressions**: Standing barbell OHP when mobility allows.
- **avoidIf**: Overhead pain — stay below painful arc.

## Walking lunge

- **id**: walking-lunge
- **name**: Walking lunge
- **equipment**:
  - bodyweight
  - dumbbell
  - home
  - gym
- **muscles**:
  - quads
  - glutes
- **level**:
  - beginner
  - intermediate
- **tags**:
  - legs
  - lower
  - single-leg
  - fat-loss
  - general
- **cues**: Long step, front knee tracks over foot, torso tall.
- **regressions**: Static split squat holding support.
- **progressions**: Weighted walking lunge.
- **avoidIf**: Knee pain — shorten step and depth.

## Front plank

- **id**: plank
- **name**: Front plank
- **equipment**:
  - bodyweight
  - none
  - home
- **muscles**:
  - core
- **level**:
  - beginner
  - intermediate
  - advanced
- **tags**:
  - core
  - stability
  - beginner
  - general
  - rehab
- **cues**: Elbows under shoulders, squeeze glutes, breathe, no sagging hips.
- **regressions**: Incline plank on bench.
- **progressions**: RKC plank or weighted plank.
- **avoidIf**: Diastasis or acute lumbar pain — use dead bug instead.

## Dead bug

- **id**: dead-bug
- **name**: Dead bug
- **equipment**:
  - bodyweight
  - none
  - home
- **muscles**:
  - core
- **level**:
  - beginner
  - intermediate
- **tags**:
  - core
  - stability
  - beginner
  - rehab
  - return
- **cues**: Low back gently pressed to floor, slow opposite arm/leg.
- **regressions**: Heel taps only.
- **progressions**: Band anti-rotation hold.
- **avoidIf**: None for most; stop if back pain increases.

## Hip thrust (barbell or dumbbell)

- **id**: hip-thrust
- **name**: Hip thrust (barbell or dumbbell)
- **equipment**:
  - gym
  - dumbbell
  - home
- **muscles**:
  - glutes
  - hamstrings
- **level**:
  - intermediate
  - advanced
- **tags**:
  - glutes
  - hinge
  - muscle
  - hypertrophy
  - lower
- **cues**: Shoulders on bench, chin tucked, full hip extension, pause at top.
- **regressions**: Glute bridge on floor.
- **progressions**: Barbell hip thrust.
- **avoidIf**: Acute hip flexor strain — reduce range.

## Lat pulldown

- **id**: lat-pulldown
- **name**: Lat pulldown
- **equipment**:
  - gym
- **muscles**:
  - back
  - biceps
- **level**:
  - beginner
  - intermediate
- **tags**:
  - pull
  - upper
  - back
  - gym
  - muscle
- **cues**: Drive elbows to pockets, slight lean, avoid behind-neck.
- **regressions**: Band pulldown or assisted pull-up.
- **progressions**: Pull-up.
- **avoidIf**: Shoulder pain on wide grip — use neutral close grip.

## Leg press

- **id**: leg-press
- **name**: Leg press
- **equipment**:
  - gym
- **muscles**:
  - quads
  - glutes
- **level**:
  - beginner
  - intermediate
- **tags**:
  - legs
  - lower
  - gym
  - muscle
  - hypertrophy
- **cues**: Feet shoulder-width, lower with control, knees track toes, no butt lift.
- **regressions**: Goblet squat.
- **progressions**: Higher load with tempo control.
- **avoidIf**: Knee pain at deep flexion — limit depth.

## Pallof press (anti-rotation)

- **id**: cable-pallof
- **name**: Pallof press (anti-rotation)
- **equipment**:
  - gym
  - band
  - home
- **muscles**:
  - core
  - obliques
- **level**:
  - beginner
  - intermediate
  - advanced
- **tags**:
  - core
  - stability
  - sport
  - padel
  - football
  - rotation
- **cues**: Press straight out, resist rotation, ribs down.
- **regressions**: Band anti-rotation hold.
- **progressions**: Split-stance Pallof walkout.
- **avoidIf**: Acute oblique strain.

## Sled push

- **id**: sled-push
- **name**: Sled push
- **equipment**:
  - gym
- **muscles**:
  - legs
  - conditioning
- **level**:
  - intermediate
  - advanced
- **tags**:
  - conditioning
  - sport
  - football
  - padel
  - fat-loss
  - cardio
- **cues**: Low torso angle, drive through balls of feet, steady breathing.
- **regressions**: Brisk incline walk.
- **progressions**: Heavier sled or shorter rest intervals.
- **avoidIf**: High blood pressure uncontrolled — consult professional first.

## Box step-up

- **id**: box-step-up
- **name**: Box step-up
- **equipment**:
  - gym
  - home
  - box
- **muscles**:
  - quads
  - glutes
- **level**:
  - beginner
  - intermediate
- **tags**:
  - single-leg
  - legs
  - sport
  - padel
  - general
- **cues**: Drive through whole foot on box, minimal push from back leg.
- **regressions**: Lower box height.
- **progressions**: Weighted step-up.
- **avoidIf**: Knee pain on step-down — step down to lower surface.

## Farmer carry

- **id**: farmer-carry
- **name**: Farmer carry
- **equipment**:
  - dumbbell
  - gym
  - home
- **muscles**:
  - grip
  - core
  - traps
- **level**:
  - beginner
  - intermediate
  - advanced
- **tags**:
  - carry
  - conditioning
  - general
  - fat-loss
  - core
- **cues**: Tall posture, shoulders packed, walk smooth and controlled.
- **regressions**: Suitcase carry one side.
- **progressions**: Heavier load or longer distance.
- **avoidIf**: Grip or elbow pain — reduce load.

## Band pull-apart

- **id**: band-pull-apart
- **name**: Band pull-apart
- **equipment**:
  - band
  - home
  - gym
- **muscles**:
  - rear-delts
  - upper-back
- **level**:
  - beginner
  - intermediate
- **tags**:
  - pull
  - shoulder health
  - warmup
  - rehab
  - posture
- **cues**: Arms straight, pull band to chest, squeeze shoulder blades.
- **regressions**: Lighter band or shorter range.
- **progressions**: Face pull with cable.
- **avoidIf**: Acute shoulder pain — pain-free range only.

## Bike intervals (moderate)

- **id**: bike-intervals
- **name**: Bike intervals (moderate)
- **equipment**:
  - gym
  - cardio
- **muscles**:
  - conditioning
- **level**:
  - beginner
  - intermediate
  - advanced
- **tags**:
  - cardio
  - fat-loss
  - conditioning
  - sport
  - football
  - padel
- **cues**: Warm up 5 min; work intervals hard but repeatable; cool down.
- **regressions**: Brisk walk intervals.
- **progressions**: Shorter rest or longer work bouts.
- **avoidIf**: Chest pain or dizziness — stop and seek medical help.

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
[
  {
    "id": "goblet-squat",
    "name": "Goblet squat",
    "equipment": [
      "dumbbell",
      "kettlebell",
      "home"
    ],
    "muscles": [
      "quads",
      "glutes",
      "core"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "tags": [
      "squat",
      "legs",
      "lower",
      "home",
      "muscle",
      "fat-loss",
      "general"
    ],
    "cues": "Hold weight at chest, elbows inside knees, sit between hips, full foot pressure.",
    "regressions": "Box squat or sit-to-stand from a chair.",
    "progressions": "Front squat or split squat.",
    "avoidIf": "Acute knee pain without clearance; scale depth."
  },
  {
    "id": "rdl-dumbbell",
    "name": "Romanian deadlift (dumbbells)",
    "equipment": [
      "dumbbell",
      "home"
    ],
    "muscles": [
      "hamstrings",
      "glutes",
      "back"
    ],
    "level": [
      "beginner",
      "intermediate",
      "advanced"
    ],
    "tags": [
      "hinge",
      "legs",
      "posterior",
      "home",
      "muscle",
      "hypertrophy"
    ],
    "cues": "Soft knees, hips back, bar/DBs close to legs, stop when hamstrings stretch.",
    "regressions": "Hip hinge drill with dowel on back.",
    "progressions": "Barbell RDL.",
    "avoidIf": "Sharp low-back pain; reduce range and load."
  },
  {
    "id": "db-bench-press",
    "name": "Dumbbell bench press",
    "equipment": [
      "dumbbell",
      "home",
      "gym"
    ],
    "muscles": [
      "chest",
      "shoulders",
      "triceps"
    ],
    "level": [
      "beginner",
      "intermediate",
      "advanced"
    ],
    "tags": [
      "push",
      "upper",
      "chest",
      "muscle",
      "hypertrophy",
      "home"
    ],
    "cues": "Shoulder blades pinched, feet planted, control descent, neutral wrists.",
    "regressions": "Floor press or incline push-up.",
    "progressions": "Barbell bench with spotter setup.",
    "avoidIf": "Shoulder impingement symptoms — use neutral-grip floor press."
  },
  {
    "id": "push-up",
    "name": "Push-up",
    "equipment": [
      "bodyweight",
      "home",
      "none"
    ],
    "muscles": [
      "chest",
      "shoulders",
      "triceps",
      "core"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "tags": [
      "push",
      "upper",
      "bodyweight",
      "home",
      "beginner",
      "general"
    ],
    "cues": "Ribs down, glutes on, hands under shoulders, full body line.",
    "regressions": "Incline push-up on bench or wall.",
    "progressions": "Deficit or weighted push-up.",
    "avoidIf": "Wrist pain — use handles or fists neutral."
  },
  {
    "id": "inverted-row",
    "name": "Inverted row (bar or rings)",
    "equipment": [
      "gym",
      "home",
      "bar"
    ],
    "muscles": [
      "back",
      "biceps",
      "rear-delts"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "tags": [
      "pull",
      "upper",
      "back",
      "home",
      "muscle"
    ],
    "cues": "Chest to bar, squeeze shoulder blades, avoid shrugging.",
    "regressions": "Bent-over dumbbell row.",
    "progressions": "Weighted row or pull-up progression.",
    "avoidIf": "Shoulder instability — reduce range."
  },
  {
    "id": "db-shoulder-press",
    "name": "Dumbbell shoulder press",
    "equipment": [
      "dumbbell",
      "home",
      "gym"
    ],
    "muscles": [
      "shoulders",
      "triceps"
    ],
    "level": [
      "intermediate",
      "advanced"
    ],
    "tags": [
      "push",
      "upper",
      "shoulders",
      "muscle"
    ],
    "cues": "Ribs down, press up and slightly back, no lower-back arch.",
    "regressions": "Half-kneeling single-arm press.",
    "progressions": "Standing barbell OHP when mobility allows.",
    "avoidIf": "Overhead pain — stay below painful arc."
  },
  {
    "id": "walking-lunge",
    "name": "Walking lunge",
    "equipment": [
      "bodyweight",
      "dumbbell",
      "home",
      "gym"
    ],
    "muscles": [
      "quads",
      "glutes"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "tags": [
      "legs",
      "lower",
      "single-leg",
      "fat-loss",
      "general"
    ],
    "cues": "Long step, front knee tracks over foot, torso tall.",
    "regressions": "Static split squat holding support.",
    "progressions": "Weighted walking lunge.",
    "avoidIf": "Knee pain — shorten step and depth."
  },
  {
    "id": "plank",
    "name": "Front plank",
    "equipment": [
      "bodyweight",
      "none",
      "home"
    ],
    "muscles": [
      "core"
    ],
    "level": [
      "beginner",
      "intermediate",
      "advanced"
    ],
    "tags": [
      "core",
      "stability",
      "beginner",
      "general",
      "rehab"
    ],
    "cues": "Elbows under shoulders, squeeze glutes, breathe, no sagging hips.",
    "regressions": "Incline plank on bench.",
    "progressions": "RKC plank or weighted plank.",
    "avoidIf": "Diastasis or acute lumbar pain — use dead bug instead."
  },
  {
    "id": "dead-bug",
    "name": "Dead bug",
    "equipment": [
      "bodyweight",
      "none",
      "home"
    ],
    "muscles": [
      "core"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "tags": [
      "core",
      "stability",
      "beginner",
      "rehab",
      "return"
    ],
    "cues": "Low back gently pressed to floor, slow opposite arm/leg.",
    "regressions": "Heel taps only.",
    "progressions": "Band anti-rotation hold.",
    "avoidIf": "None for most; stop if back pain increases."
  },
  {
    "id": "hip-thrust",
    "name": "Hip thrust (barbell or dumbbell)",
    "equipment": [
      "gym",
      "dumbbell",
      "home"
    ],
    "muscles": [
      "glutes",
      "hamstrings"
    ],
    "level": [
      "intermediate",
      "advanced"
    ],
    "tags": [
      "glutes",
      "hinge",
      "muscle",
      "hypertrophy",
      "lower"
    ],
    "cues": "Shoulders on bench, chin tucked, full hip extension, pause at top.",
    "regressions": "Glute bridge on floor.",
    "progressions": "Barbell hip thrust.",
    "avoidIf": "Acute hip flexor strain — reduce range."
  },
  {
    "id": "lat-pulldown",
    "name": "Lat pulldown",
    "equipment": [
      "gym"
    ],
    "muscles": [
      "back",
      "biceps"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "tags": [
      "pull",
      "upper",
      "back",
      "gym",
      "muscle"
    ],
    "cues": "Drive elbows to pockets, slight lean, avoid behind-neck.",
    "regressions": "Band pulldown or assisted pull-up.",
    "progressions": "Pull-up.",
    "avoidIf": "Shoulder pain on wide grip — use neutral close grip."
  },
  {
    "id": "leg-press",
    "name": "Leg press",
    "equipment": [
      "gym"
    ],
    "muscles": [
      "quads",
      "glutes"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "tags": [
      "legs",
      "lower",
      "gym",
      "muscle",
      "hypertrophy"
    ],
    "cues": "Feet shoulder-width, lower with control, knees track toes, no butt lift.",
    "regressions": "Goblet squat.",
    "progressions": "Higher load with tempo control.",
    "avoidIf": "Knee pain at deep flexion — limit depth."
  },
  {
    "id": "cable-pallof",
    "name": "Pallof press (anti-rotation)",
    "equipment": [
      "gym",
      "band",
      "home"
    ],
    "muscles": [
      "core",
      "obliques"
    ],
    "level": [
      "beginner",
      "intermediate",
      "advanced"
    ],
    "tags": [
      "core",
      "stability",
      "sport",
      "padel",
      "football",
      "rotation"
    ],
    "cues": "Press straight out, resist rotation, ribs down.",
    "regressions": "Band anti-rotation hold.",
    "progressions": "Split-stance Pallof walkout.",
    "avoidIf": "Acute oblique strain."
  },
  {
    "id": "sled-push",
    "name": "Sled push",
    "equipment": [
      "gym"
    ],
    "muscles": [
      "legs",
      "conditioning"
    ],
    "level": [
      "intermediate",
      "advanced"
    ],
    "tags": [
      "conditioning",
      "sport",
      "football",
      "padel",
      "fat-loss",
      "cardio"
    ],
    "cues": "Low torso angle, drive through balls of feet, steady breathing.",
    "regressions": "Brisk incline walk.",
    "progressions": "Heavier sled or shorter rest intervals.",
    "avoidIf": "High blood pressure uncontrolled — consult professional first."
  },
  {
    "id": "box-step-up",
    "name": "Box step-up",
    "equipment": [
      "gym",
      "home",
      "box"
    ],
    "muscles": [
      "quads",
      "glutes"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "tags": [
      "single-leg",
      "legs",
      "sport",
      "padel",
      "general"
    ],
    "cues": "Drive through whole foot on box, minimal push from back leg.",
    "regressions": "Lower box height.",
    "progressions": "Weighted step-up.",
    "avoidIf": "Knee pain on step-down — step down to lower surface."
  },
  {
    "id": "farmer-carry",
    "name": "Farmer carry",
    "equipment": [
      "dumbbell",
      "gym",
      "home"
    ],
    "muscles": [
      "grip",
      "core",
      "traps"
    ],
    "level": [
      "beginner",
      "intermediate",
      "advanced"
    ],
    "tags": [
      "carry",
      "conditioning",
      "general",
      "fat-loss",
      "core"
    ],
    "cues": "Tall posture, shoulders packed, walk smooth and controlled.",
    "regressions": "Suitcase carry one side.",
    "progressions": "Heavier load or longer distance.",
    "avoidIf": "Grip or elbow pain — reduce load."
  },
  {
    "id": "band-pull-apart",
    "name": "Band pull-apart",
    "equipment": [
      "band",
      "home",
      "gym"
    ],
    "muscles": [
      "rear-delts",
      "upper-back"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "tags": [
      "pull",
      "shoulder health",
      "warmup",
      "rehab",
      "posture"
    ],
    "cues": "Arms straight, pull band to chest, squeeze shoulder blades.",
    "regressions": "Lighter band or shorter range.",
    "progressions": "Face pull with cable.",
    "avoidIf": "Acute shoulder pain — pain-free range only."
  },
  {
    "id": "bike-intervals",
    "name": "Bike intervals (moderate)",
    "equipment": [
      "gym",
      "cardio"
    ],
    "muscles": [
      "conditioning"
    ],
    "level": [
      "beginner",
      "intermediate",
      "advanced"
    ],
    "tags": [
      "cardio",
      "fat-loss",
      "conditioning",
      "sport",
      "football",
      "padel"
    ],
    "cues": "Warm up 5 min; work intervals hard but repeatable; cool down.",
    "regressions": "Brisk walk intervals.",
    "progressions": "Shorter rest or longer work bouts.",
    "avoidIf": "Chest pain or dizziness — stop and seek medical help."
  }
]
```

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/knowledge/data/exercises.json` — Complete file (219 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
