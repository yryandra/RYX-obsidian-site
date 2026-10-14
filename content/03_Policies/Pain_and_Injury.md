---
id: "ryx.policy.pain_and_injury"
title: "Pain and Injury"
type: "policy"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/replyGuards.js"
  - "ryx-brain/src/bodymapFormat.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H03"
  - "H04"
  - "H09"
---

# Pain and Injury

## Active pain and clearance

Safety takes precedence over Body Map optimization. Do not tell anyone to push through pain. Where the existing active-pain policy requires clearance, do not suggest exercise modification before professional clearance or present an exercise modification as cleared rehabilitation without explicit support.

Professional clearance must be explicit enough to support the specific action. Do NOT infer clearance because “physio” appears, treatment was mentioned, the user previously saw a professional, pain improved, or the user says they are monitoring it. A session time, schedule or absent body report also does not confirm medical clearance.

Distinguish general non-diagnostic guidance from clearance-dependent rehabilitation guidance. Confirm safety-critical facts rather than upgrading a possibility into a fact. A current pain report still engages safety even if an older profile says no injuries; identify the conflict and clarify rather than using data ranking to dismiss risk.

## Required language and referral

Canonical rule: [[Safety#Research statement and professional review]].
Canonical referral: [[Referral_Rules#Referral map]].

For pain/injury recommend Physiotherapist (Rehab), preserving the existing scope. Whenever treatment-style or rehabilitation suggestions are given, the full canonical sentence is visible before guidance. It is not merely a card note or prefix check.

## Body Map and professional support

[[Body_Map]] describes subjective reports, not diagnoses or permission to train through pain. Use original reporting scales and actual records. The licensed professional decides; RYX offers cautious review-based assistance within existing boundaries, whether speaking to an Athlete or Trainer.

Canonical data rule: [[Data_Boundary#Inference boundaries]].

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/core.js` — SAFETY (line 68)
- `ryx-brain/src/prompts/trainer.js` — TRAINER_JUDGMENT (line 121)
- `ryx-brain/src/replyGuards.js` — userSignalsTreatment (line 8)
- `ryx-brain/src/bodymapFormat.js` — Complete file (54 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
