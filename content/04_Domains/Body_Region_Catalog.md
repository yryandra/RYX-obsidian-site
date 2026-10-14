---
id: "ryx.domain.body_region_catalog"
title: "Body Region Catalog"
type: "domain"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/bodymapRegions.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H04"
  - "H09"
---

# Body Region Catalog

## Authoritative implemented schema

# Body Region Catalog

The exact 34 current zones and legacy alias map. Region identifiers, labels, views and sides are interpretation schema, not user reports. Legacy rollups may select one side for older broad entries (for example core → abs-l); do not infer a more precise original anatomical report.

## Regions

- Item 1:
  - **id**: neck
  - **label**: Neck
  - **view**: both
  - **side**: both
- Item 2:
  - **id**: trapezius
  - **label**: Trapezius
  - **view**: front
  - **side**: both
- Item 3:
  - **id**: deltoids-l
  - **label**: Left Deltoid
  - **view**: both
  - **side**: left
- Item 4:
  - **id**: deltoids-r
  - **label**: Right Deltoid
  - **view**: both
  - **side**: right
- Item 5:
  - **id**: chest-l
  - **label**: Left Chest
  - **view**: front
  - **side**: left
- Item 6:
  - **id**: chest-r
  - **label**: Right Chest
  - **view**: front
  - **side**: right
- Item 7:
  - **id**: abs-l
  - **label**: Left Abs
  - **view**: front
  - **side**: left
- Item 8:
  - **id**: abs-r
  - **label**: Right Abs
  - **view**: front
  - **side**: right
- Item 9:
  - **id**: obliques-l
  - **label**: Left Obliques
  - **view**: front
  - **side**: left
- Item 10:
  - **id**: obliques-r
  - **label**: Right Obliques
  - **view**: front
  - **side**: right
- Item 11:
  - **id**: biceps-l
  - **label**: Left Biceps
  - **view**: front
  - **side**: left
- Item 12:
  - **id**: biceps-r
  - **label**: Right Biceps
  - **view**: front
  - **side**: right
- Item 13:
  - **id**: triceps-l
  - **label**: Left Triceps
  - **view**: both
  - **side**: left
- Item 14:
  - **id**: triceps-r
  - **label**: Right Triceps
  - **view**: both
  - **side**: right
- Item 15:
  - **id**: forearm-l
  - **label**: Left Forearm
  - **view**: both
  - **side**: left
- Item 16:
  - **id**: forearm-r
  - **label**: Right Forearm
  - **view**: both
  - **side**: right
- Item 17:
  - **id**: adductors-l
  - **label**: Left Adductors
  - **view**: both
  - **side**: left
- Item 18:
  - **id**: adductors-r
  - **label**: Right Adductors
  - **view**: both
  - **side**: right
- Item 19:
  - **id**: quadriceps-l
  - **label**: Left Quadriceps
  - **view**: front
  - **side**: left
- Item 20:
  - **id**: quadriceps-r
  - **label**: Right Quadriceps
  - **view**: front
  - **side**: right
- Item 21:
  - **id**: tibialis-l
  - **label**: Left Tibialis
  - **view**: front
  - **side**: left
- Item 22:
  - **id**: tibialis-r
  - **label**: Right Tibialis
  - **view**: front
  - **side**: right
- Item 23:
  - **id**: calves-l
  - **label**: Left Calves
  - **view**: both
  - **side**: left
- Item 24:
  - **id**: calves-r
  - **label**: Right Calves
  - **view**: both
  - **side**: right
- Item 25:
  - **id**: trapezius-l
  - **label**: Left Trapezius
  - **view**: back
  - **side**: left
- Item 26:
  - **id**: trapezius-r
  - **label**: Right Trapezius
  - **view**: back
  - **side**: right
- Item 27:
  - **id**: upper-back-l
  - **label**: Left Upper back
  - **view**: back
  - **side**: left
- Item 28:
  - **id**: upper-back-r
  - **label**: Right Upper back
  - **view**: back
  - **side**: right
- Item 29:
  - **id**: lower-back-l
  - **label**: Left Lower back
  - **view**: back
  - **side**: left
- Item 30:
  - **id**: lower-back-r
  - **label**: Right Lower back
  - **view**: back
  - **side**: right
- Item 31:
  - **id**: gluteal-l
  - **label**: Left Glutes
  - **view**: back
  - **side**: left
- Item 32:
  - **id**: gluteal-r
  - **label**: Right Glutes
  - **view**: back
  - **side**: right
- Item 33:
  - **id**: hamstring-l
  - **label**: Left Hamstrings
  - **view**: back
  - **side**: left
- Item 34:
  - **id**: hamstring-r
  - **label**: Right Hamstrings
  - **view**: back
  - **side**: right

## Legacy Aliases

- **neck-l**: neck
- **neck-r**: neck
- **shoulder-l**: deltoids-l
- **shoulder-r**: deltoids-r
- **deltoid-l**: deltoids-l
- **deltoid-r**: deltoids-r
- **deltoid-post-l**: deltoids-l
- **deltoid-post-r**: deltoids-r
- **pec-l**: chest-l
- **pec-r**: chest-r
- **arm-l**: biceps-l
- **arm-r**: biceps-r
- **arm-back-l**: triceps-l
- **arm-back-r**: triceps-r
- **forearm-flex-l**: forearm-l
- **forearm-flex-r**: forearm-r
- **forearm-ext-l**: forearm-l
- **forearm-ext-r**: forearm-r
- **core**: abs-l
- **abs-upper**: abs-l
- **abs-lower**: abs-r
- **oblique-l**: obliques-l
- **oblique-r**: obliques-r
- **hip**: adductors-l
- **hip-flexor**: adductors-l
- **tfl-l**: adductors-l
- **tfl-r**: adductors-r
- **quad-l**: quadriceps-l
- **quad-r**: quadriceps-r
- **vastus-med-l**: quadriceps-l
- **vastus-lat-l**: quadriceps-l
- **vastus-med-r**: quadriceps-r
- **vastus-lat-r**: quadriceps-r
- **lower-leg-l**: calves-l
- **lower-leg-r**: calves-r
- **shin-l**: tibialis-l
- **shin-r**: tibialis-r
- **calf-front-l**: calves-l
- **calf-front-r**: calves-r
- **traps**: trapezius
- **infraspinatus-l**: upper-back-l
- **lat-l**: upper-back-l
- **infraspinatus-r**: upper-back-r
- **lat-r**: upper-back-r
- **upper-back**: upper-back-l
- **lower-back**: lower-back-l
- **glute-l**: gluteal-l
- **glute-r**: gluteal-r
- **hamstring-l-lat**: hamstring-l
- **hamstring-l-med**: hamstring-l
- **hamstring-r-lat**: hamstring-r
- **hamstring-r-med**: hamstring-r
- **calf-back-l**: calves-l
- **calf-back-r**: calves-r
- **calf-lat-l**: calves-l
- **calf-med-l**: calves-l
- **calf-lat-r**: calves-r
- **calf-med-r**: calves-r
- **chest**: chest-l
- **abs**: abs-l
- **glutes**: gluteal-l
- **knee-l**: quadriceps-l
- **knee-r**: quadriceps-r
- **calf-l**: calves-l
- **calf-r**: calves-r

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
{
  "regions": [
    {
      "id": "neck",
      "label": "Neck",
      "view": "both",
      "side": "both"
    },
    {
      "id": "trapezius",
      "label": "Trapezius",
      "view": "front",
      "side": "both"
    },
    {
      "id": "deltoids-l",
      "label": "Left Deltoid",
      "view": "both",
      "side": "left"
    },
    {
      "id": "deltoids-r",
      "label": "Right Deltoid",
      "view": "both",
      "side": "right"
    },
    {
      "id": "chest-l",
      "label": "Left Chest",
      "view": "front",
      "side": "left"
    },
    {
      "id": "chest-r",
      "label": "Right Chest",
      "view": "front",
      "side": "right"
    },
    {
      "id": "abs-l",
      "label": "Left Abs",
      "view": "front",
      "side": "left"
    },
    {
      "id": "abs-r",
      "label": "Right Abs",
      "view": "front",
      "side": "right"
    },
    {
      "id": "obliques-l",
      "label": "Left Obliques",
      "view": "front",
      "side": "left"
    },
    {
      "id": "obliques-r",
      "label": "Right Obliques",
      "view": "front",
      "side": "right"
    },
    {
      "id": "biceps-l",
      "label": "Left Biceps",
      "view": "front",
      "side": "left"
    },
    {
      "id": "biceps-r",
      "label": "Right Biceps",
      "view": "front",
      "side": "right"
    },
    {
      "id": "triceps-l",
      "label": "Left Triceps",
      "view": "both",
      "side": "left"
    },
    {
      "id": "triceps-r",
      "label": "Right Triceps",
      "view": "both",
      "side": "right"
    },
    {
      "id": "forearm-l",
      "label": "Left Forearm",
      "view": "both",
      "side": "left"
    },
    {
      "id": "forearm-r",
      "label": "Right Forearm",
      "view": "both",
      "side": "right"
    },
    {
      "id": "adductors-l",
      "label": "Left Adductors",
      "view": "both",
      "side": "left"
    },
    {
      "id": "adductors-r",
      "label": "Right Adductors",
      "view": "both",
      "side": "right"
    },
    {
      "id": "quadriceps-l",
      "label": "Left Quadriceps",
      "view": "front",
      "side": "left"
    },
    {
      "id": "quadriceps-r",
      "label": "Right Quadriceps",
      "view": "front",
      "side": "right"
    },
    {
      "id": "tibialis-l",
      "label": "Left Tibialis",
      "view": "front",
      "side": "left"
    },
    {
      "id": "tibialis-r",
      "label": "Right Tibialis",
      "view": "front",
      "side": "right"
    },
    {
      "id": "calves-l",
      "label": "Left Calves",
      "view": "both",
      "side": "left"
    },
    {
      "id": "calves-r",
      "label": "Right Calves",
      "view": "both",
      "side": "right"
    },
    {
      "id": "trapezius-l",
      "label": "Left Trapezius",
      "view": "back",
      "side": "left"
    },
    {
      "id": "trapezius-r",
      "label": "Right Trapezius",
      "view": "back",
      "side": "right"
    },
    {
      "id": "upper-back-l",
      "label": "Left Upper back",
      "view": "back",
      "side": "left"
    },
    {
      "id": "upper-back-r",
      "label": "Right Upper back",
      "view": "back",
      "side": "right"
    },
    {
      "id": "lower-back-l",
      "label": "Left Lower back",
      "view": "back",
      "side": "left"
    },
    {
      "id": "lower-back-r",
      "label": "Right Lower back",
      "view": "back",
      "side": "right"
    },
    {
      "id": "gluteal-l",
      "label": "Left Glutes",
      "view": "back",
      "side": "left"
    },
    {
      "id": "gluteal-r",
      "label": "Right Glutes",
      "view": "back",
      "side": "right"
    },
    {
      "id": "hamstring-l",
      "label": "Left Hamstrings",
      "view": "back",
      "side": "left"
    },
    {
      "id": "hamstring-r",
      "label": "Right Hamstrings",
      "view": "back",
      "side": "right"
    }
  ],
  "legacy_aliases": {
    "neck-l": "neck",
    "neck-r": "neck",
    "shoulder-l": "deltoids-l",
    "shoulder-r": "deltoids-r",
    "deltoid-l": "deltoids-l",
    "deltoid-r": "deltoids-r",
    "deltoid-post-l": "deltoids-l",
    "deltoid-post-r": "deltoids-r",
    "pec-l": "chest-l",
    "pec-r": "chest-r",
    "arm-l": "biceps-l",
    "arm-r": "biceps-r",
    "arm-back-l": "triceps-l",
    "arm-back-r": "triceps-r",
    "forearm-flex-l": "forearm-l",
    "forearm-flex-r": "forearm-r",
    "forearm-ext-l": "forearm-l",
    "forearm-ext-r": "forearm-r",
    "core": "abs-l",
    "abs-upper": "abs-l",
    "abs-lower": "abs-r",
    "oblique-l": "obliques-l",
    "oblique-r": "obliques-r",
    "hip": "adductors-l",
    "hip-flexor": "adductors-l",
    "tfl-l": "adductors-l",
    "tfl-r": "adductors-r",
    "quad-l": "quadriceps-l",
    "quad-r": "quadriceps-r",
    "vastus-med-l": "quadriceps-l",
    "vastus-lat-l": "quadriceps-l",
    "vastus-med-r": "quadriceps-r",
    "vastus-lat-r": "quadriceps-r",
    "lower-leg-l": "calves-l",
    "lower-leg-r": "calves-r",
    "shin-l": "tibialis-l",
    "shin-r": "tibialis-r",
    "calf-front-l": "calves-l",
    "calf-front-r": "calves-r",
    "traps": "trapezius",
    "infraspinatus-l": "upper-back-l",
    "lat-l": "upper-back-l",
    "infraspinatus-r": "upper-back-r",
    "lat-r": "upper-back-r",
    "upper-back": "upper-back-l",
    "lower-back": "lower-back-l",
    "glute-l": "gluteal-l",
    "glute-r": "gluteal-r",
    "hamstring-l-lat": "hamstring-l",
    "hamstring-l-med": "hamstring-l",
    "hamstring-r-lat": "hamstring-r",
    "hamstring-r-med": "hamstring-r",
    "calf-back-l": "calves-l",
    "calf-back-r": "calves-r",
    "calf-lat-l": "calves-l",
    "calf-med-l": "calves-l",
    "calf-lat-r": "calves-r",
    "calf-med-r": "calves-r",
    "chest": "chest-l",
    "abs": "abs-l",
    "glutes": "gluteal-l",
    "knee-l": "quadriceps-l",
    "knee-r": "quadriceps-r",
    "calf-l": "calves-l",
    "calf-r": "calves-r"
  }
}
```

Canonical interpretation: [[Body_Map#Current authoritative domain model]]. Canonical safety: [[Pain_and_Injury#Active pain and clearance]]. Region metadata and aliases are schema, not user body reports.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/bodymapRegions.js` — Complete file (106 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
