---
id: "ryx.knowledge.legacy_playbooks"
title: "Legacy Playbooks"
type: "knowledge"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/knowledge/data/playbooks.json"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
decision_ids:
  - "H08"
  - "H12"
---

# Legacy Playbooks

## Reference status

Retained historical/source evidence, excluded from the candidate manifest. It is not an independent canonical instruction or claim of a new passing run. See [[RYX_BRAIN_DECISIONS]] for intended rules and [[Knowledge_System#Future retrieval contract]] / [[Eval_System#Production-quality evaluation contract]] for future integration.

# Legacy Playbooks

All six existing playbooks are retained as reference knowledge. Current retrieveRyxKnowledge returns playbooks: [] for both roles; these are not part of the active v0.1.0 production manifest. Do not treat retained unused material as executed instruction.

## Fat loss fundamentals (RYX)

- **id**: fat-loss-fundamentals
- **title**: Fat loss fundamentals (RYX)
- **niche**:
  - fat-loss
  - weight-loss
  - lean
  - cut
  - general-fitness
- **level**:
  - beginner
  - intermediate
- **points**:
  - Prioritize a sustainable calorie deficit — not crash dieting; protein ~1.6–2.2 g/kg bodyweight when possible.
  - Train 3–4 days/week: mix full-body or upper/lower with steps/NEAT daily (8–10k steps is a common anchor).
  - Keep most sets in 6–15 reps for muscle retention while dieting; maintain at least 2 hard lower and 2 hard upper sessions per week.
  - Sleep and stress matter as much as workouts — flag low sleep before adding training volume.
  - Scale food and training together: if energy crashes, reduce deficit or deload training — never both crash at once.

## Hypertrophy — 4-day upper/lower (full gym)

- **id**: hypertrophy-gym-4d
- **title**: Hypertrophy — 4-day upper/lower (full gym)
- **niche**:
  - muscle
  - hypertrophy
  - muscle-gain
  - bodybuilding
  - strength
- **level**:
  - intermediate
  - advanced
- **points**:
  - Split: Upper / Lower / Upper / Lower with one rest day between hard lower days when possible.
  - Each session: 1 main compound (4 sets), 2 secondary compounds or machines (3 sets), 2–3 isolations (2–3 sets).
  - Most working sets RPE 7–9, 6–15 reps; double progression (add reps then load).
  - Deload every 4–6 weeks or when performance drops 2 sessions in a row.
  - Protein and sleep drive growth — program volume is second to recovery.

## Home dumbbell — 3-day full body

- **id**: home-dumbbell-3d
- **title**: Home dumbbell — 3-day full body
- **niche**:
  - home
  - dumbbell
  - beginner
  - general-fitness
  - muscle
- **level**:
  - beginner
  - intermediate
- **points**:
  - Day A: Goblet squat, DB bench, RDL, plank. Day B: Lunge, row, shoulder press, dead bug. Day C: Repeat A pattern with +1 set or +2 reps.
  - 3 sets of 8–12 for main lifts; 2–3 sets for core. Rest 60–90 sec.
  - If only one DB pair, prioritize single-arm work and goblet variations.
  - Add walks or farmer carries on off days for easy conditioning.
  - Progress by reps first, then load, then an extra set — not all three at once.

## Return after break or injury (non-clinical)

- **id**: return-to-training
- **title**: Return after break or injury (non-clinical)
- **niche**:
  - return
  - restart
  - injury
  - recovery
  - rehab
  - accident
  - crash
- **level**:
  - beginner
  - intermediate
- **points**:
  - Week 1–2: movement quality, pain-free range, 2–3 sessions, RPE 5–6 only unless medically cleared for more.
  - Use bilateral and stable patterns first (goblet squat, dead bug, band pull-apart, incline push-up).
  - No max effort or failure sets until clearance and 2 weeks pain-free training.
  - If pain spikes during a movement, swap regression same session — do not push through.
  - Always recommend professional clearance after accident, surgery, or persistent pain.

## Padel / court sport conditioning

- **id**: padel-conditioning
- **title**: Padel / court sport conditioning
- **niche**:
  - padel
  - sport
  - football
  - tennis
  - conditioning
  - sport-performance
- **level**:
  - intermediate
  - advanced
- **points**:
  - Train repeated accelerations and decelerations: lateral steps, box step-ups, Pallof press, short sled or bike intervals.
  - 2 strength days (lower + upper) + 1–2 conditioning days; avoid heavy legs same day as match if performance matters.
  - Eccentric calf and hamstring work for injury resilience; warm up hips and thoracic rotation before court.
  - Conditioning: work/rest 1:2 or 1:3, 6–10 rounds, leave 1–2 reps in tank for repeatability.
  - Refer sport-specific skill work to a sport coach; RYX handles physical prep.

## Wellness nutrition basics (non-clinical)

- **id**: nutrition-wellness-basics
- **title**: Wellness nutrition basics (non-clinical)
- **niche**:
  - nutrition
  - wellness
  - eat
  - meal
  - protein
  - health
- **level**:
  - beginner
  - intermediate
- **points**:
  - Anchor each meal with protein + produce + water before supplements.
  - Eating out: protein-forward choice, half plate vegetables when possible, avoid doubling fried sides every meal.
  - Hydration 30–35 ml/kg/day as a starting estimate; adjust for heat and training sweat.
  - No extreme restriction; if user shows ED risk signals, stop diet coaching and refer to qualified help.
  - Align calories with goal: modest deficit for fat loss, slight surplus for muscle gain, maintenance for performance.

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
[
  {
    "id": "fat-loss-fundamentals",
    "title": "Fat loss fundamentals (RYX)",
    "niche": [
      "fat-loss",
      "weight-loss",
      "lean",
      "cut",
      "general-fitness"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "points": [
      "Prioritize a sustainable calorie deficit — not crash dieting; protein ~1.6–2.2 g/kg bodyweight when possible.",
      "Train 3–4 days/week: mix full-body or upper/lower with steps/NEAT daily (8–10k steps is a common anchor).",
      "Keep most sets in 6–15 reps for muscle retention while dieting; maintain at least 2 hard lower and 2 hard upper sessions per week.",
      "Sleep and stress matter as much as workouts — flag low sleep before adding training volume.",
      "Scale food and training together: if energy crashes, reduce deficit or deload training — never both crash at once."
    ]
  },
  {
    "id": "hypertrophy-gym-4d",
    "title": "Hypertrophy — 4-day upper/lower (full gym)",
    "niche": [
      "muscle",
      "hypertrophy",
      "muscle-gain",
      "bodybuilding",
      "strength"
    ],
    "level": [
      "intermediate",
      "advanced"
    ],
    "points": [
      "Split: Upper / Lower / Upper / Lower with one rest day between hard lower days when possible.",
      "Each session: 1 main compound (4 sets), 2 secondary compounds or machines (3 sets), 2–3 isolations (2–3 sets).",
      "Most working sets RPE 7–9, 6–15 reps; double progression (add reps then load).",
      "Deload every 4–6 weeks or when performance drops 2 sessions in a row.",
      "Protein and sleep drive growth — program volume is second to recovery."
    ]
  },
  {
    "id": "home-dumbbell-3d",
    "title": "Home dumbbell — 3-day full body",
    "niche": [
      "home",
      "dumbbell",
      "beginner",
      "general-fitness",
      "muscle"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "points": [
      "Day A: Goblet squat, DB bench, RDL, plank. Day B: Lunge, row, shoulder press, dead bug. Day C: Repeat A pattern with +1 set or +2 reps.",
      "3 sets of 8–12 for main lifts; 2–3 sets for core. Rest 60–90 sec.",
      "If only one DB pair, prioritize single-arm work and goblet variations.",
      "Add walks or farmer carries on off days for easy conditioning.",
      "Progress by reps first, then load, then an extra set — not all three at once."
    ]
  },
  {
    "id": "return-to-training",
    "title": "Return after break or injury (non-clinical)",
    "niche": [
      "return",
      "restart",
      "injury",
      "recovery",
      "rehab",
      "accident",
      "crash"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "points": [
      "Week 1–2: movement quality, pain-free range, 2–3 sessions, RPE 5–6 only unless medically cleared for more.",
      "Use bilateral and stable patterns first (goblet squat, dead bug, band pull-apart, incline push-up).",
      "No max effort or failure sets until clearance and 2 weeks pain-free training.",
      "If pain spikes during a movement, swap regression same session — do not push through.",
      "Always recommend professional clearance after accident, surgery, or persistent pain."
    ]
  },
  {
    "id": "padel-conditioning",
    "title": "Padel / court sport conditioning",
    "niche": [
      "padel",
      "sport",
      "football",
      "tennis",
      "conditioning",
      "sport-performance"
    ],
    "level": [
      "intermediate",
      "advanced"
    ],
    "points": [
      "Train repeated accelerations and decelerations: lateral steps, box step-ups, Pallof press, short sled or bike intervals.",
      "2 strength days (lower + upper) + 1–2 conditioning days; avoid heavy legs same day as match if performance matters.",
      "Eccentric calf and hamstring work for injury resilience; warm up hips and thoracic rotation before court.",
      "Conditioning: work/rest 1:2 or 1:3, 6–10 rounds, leave 1–2 reps in tank for repeatability.",
      "Refer sport-specific skill work to a sport coach; RYX handles physical prep."
    ]
  },
  {
    "id": "nutrition-wellness-basics",
    "title": "Wellness nutrition basics (non-clinical)",
    "niche": [
      "nutrition",
      "wellness",
      "eat",
      "meal",
      "protein",
      "health"
    ],
    "level": [
      "beginner",
      "intermediate"
    ],
    "points": [
      "Anchor each meal with protein + produce + water before supplements.",
      "Eating out: protein-forward choice, half plate vegetables when possible, avoid doubling fried sides every meal.",
      "Hydration 30–35 ml/kg/day as a starting estimate; adjust for heat and training sweat.",
      "No extreme restriction; if user shows ED risk signals, stop diet coaching and refer to qualified help.",
      "Align calories with goal: modest deficit for fat loss, slight surplus for muscle gain, maintenance for performance."
    ]
  }
]
```

## Source reference

- `ryx-brain/src/knowledge/data/playbooks.json` — Complete file (81 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
