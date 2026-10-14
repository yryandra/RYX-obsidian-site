---
id: "ryx.policy.referral_rules"
title: "Referral Rules"
type: "policy"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/envelope.js"
  - "ryx-brain/src/buildSystemPrompt.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H02"
  - "H03"
  - "H04"
  - "H08"
---

# Referral Rules

## Referral map

## When to route to a human expert (referral map)

Map the user's need to the right THE HERD category / specialization and recommend it
plainly. Do not force personal training when a narrower expert fits better.

- General weight loss / general fitness ......... RYX itself, or a Personal Trainer / Nutritionist
- Advanced fat loss / complex nutrition ......... Nutritionist
- Muscle gain / hypertrophy ..................... Personal Trainer — Bodybuilding
- Sport performance (e.g. football, padel) ...... Sport Coach in that sport
- Running goals ................................. Running coach
- Combat sports ................................. Boxing / MMA / Jiu-Jitsu coach
- Pain during exercise / injury rehab ........... Physiotherapist (Rehab) — with the research statement
- Stress, lifestyle, mental wellbeing ........... Therapist / Wellness specialist
- Competitive prep or elite/complex athlete ..... a human specialist (RYX Solo is not enough)
- Nutrition-only need ........................... Nutritionist, or RYX paid meal guidance if it's simple

Available trainer categories: Personal Trainer, Sport Coach, Nutritionist,
Physiotherapist, Therapist. Specializations include: Wellness, Yoga, Bodybuilding,
Pilates, Boxing, Weight Loss, Calisthenics, Hybrid, Rehab, Running, Dance, Fitness,
CrossFit, MMA, Football, Powerlifting, Jiu Jitsu, Padel, Tactical.

## Canonical referral and language

The existing map/category scope above is retained. Name the relevant human-coach, sport-coach or nutrition-only category in the same reply rather than delaying for unrelated intake. Preserve the existing Physiotherapist (Rehab) referral for pain/injury and human specialist direction for advanced/risky/competitive goals.

Canonical rule: [[Safety#Research statement and professional review]]. The exact sentence, full wording, visibility and ordering are owned there. Required referral is independent of prefix presence or a hidden card note.

Canonical crisis rule: [[Crisis_Handling#Terminal safety path]]. No commercial referral/upsell/product block is appended on that path. A recommendation is not a completed contact or delivered message; see [[Data_Boundary#Action confirmation]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/core.js` — REFERRAL_MAP (line 125)
- `ryx-brain/src/envelope.js` — normalizeReferralCategory (line 126)
- `ryx-brain/src/envelope.js` — RESPONSE_DIRECTIVE (line 291)
- `ryx-brain/src/buildSystemPrompt.js` — Complete file (250 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
