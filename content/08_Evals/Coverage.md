---
id: "ryx.eval.coverage"
title: "Coverage"
type: "eval"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/COVERAGE.md"
  - "ryx-brain/src/scenarios/athlete.json"
  - "ryx-brain/src/scenarios/trainer.json"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
decision_ids:
  - "H08"
  - "H12"
---

# Coverage

## Candidate evaluation distinction

This is reference_only evidence. The original migration coverage matrix and its checkmarks remain historical mapping, not proof that the current runtime meets v0.2.0. Canonical intended full-pipeline evaluation is [[Eval_System#Production-quality evaluation contract]]; the H01–H12 acceptance overlay is [[Eval_System#Canonical candidate acceptance]]. No test runner or historical result has been changed.

# Coverage

## How to interpret this map

The original matrix below is retained verbatim. Checkmarks indicate a referenced scenario, not a fresh passing run. Dashes and app-side/emergent rows remain unchanged. Some rule attribution and app-side descriptions predate newer workflow blocks and shared API behavior; see [[MIGRATION_REVIEW]]. Actual suites currently contain 50 athlete and 47 trainer scenarios.

## Original coverage document

# RYX brain — scenario coverage

Maps every use-case group from the two spec docs (60 athlete + 69 trainer scenarios)
to the brain rule that covers it, and to the eval that checks it. Prompt sources live in
`src/prompts/` (`core.js`, `athlete.js`, `trainer.js`) and are assembled by
`src/buildSystemPrompt.js`. Scenarios sampled by the automated eval are marked ✔ (eval);
the rest are covered by the same rule but not individually graded.

Legend for "Covered by": file · exported block.

---

## Athlete Assistant (R.Y.X. - Athlete Assistant User Scenerios)

| Scenario(s) | Covered by | Eval |
|---|---|---|
| A1 New user, no trainer | athlete · `ATHLETE_ROLE` (Solo) + `ATHLETE_CAPABILITIES` (assessment) | ✔ A1 |
| A2 Vague goal → clearer | athlete · `ATHLETE_CAPABILITIES` (goal discovery) | ✔ A2 |
| A3 Multiple goals → primary/secondary | athlete · `ATHLETE_CAPABILITIES` ("name ONE primary") | ✔ A3 |
| A4 Beginner level | athlete · `ATHLETE_CAPABILITIES` + core `PERSONALITY` (patient, confidence-building) | ✔ A4 |
| A5 Equipment access (home only) | athlete · `ATHLETE_CAPABILITIES` ("never prescribe equipment they lack") | ✔ A5 |
| A6 Affordable coaching (Solo) | athlete · `ATHLETE_ROLE` + core `IDENTITY` (affordable coach) | ✔ A6 |
| A7 Paid beginner plan | athlete · `ATHLETE_PAID` (full program: days/exercises/sets/reps/rest/progression) | ✔ A7 |
| A8 Free user asks full plan | athlete · `ATHLETE_FREE` (basic structure + one upgrade line) | ✔ A8 |
| A9 Missed a workout | athlete · `ATHLETE_CAPABILITIES` (restart, momentum-over-guilt) | ✔ A9 |
| A10 Restart after falling off | athlete · `ATHLETE_CAPABILITIES` (restart plan) | ✔ A10 |
| A11 How to do an exercise | athlete · `ATHLETE_CAPABILITIES` (form + safety cues) | ✔ A11 |
| A12 Exercise alternative | athlete · `ATHLETE_CAPABILITIES` (regressions) | ✔ A12 |
| A13 Too hard | athlete · `ATHLETE_CAPABILITIES` (adjust down, no failure framing) | ✔ A13 |
| A14 Too easy | athlete · `ATHLETE_CAPABILITIES` (progression) | ✔ A14 |
| A15 What to do today | athlete · `ATHLETE_CAPABILITIES` (daily focus) | ✔ A15 |
| A16 Eat for weight loss (free) | athlete · `ATHLETE_FREE` (general nutrition) + core `SAFETY` (no extreme diet) | ✔ A16 |
| A17 Full meal plan (paid) | athlete · `ATHLETE_PAID` (meal plan draft) | ✔ A17 |
| A18 Full meal plan (free) | athlete · `ATHLETE_FREE` (structure + upgrade) | ✔ A18 |
| A19 Food swaps | athlete · `ATHLETE_CAPABILITIES` (swaps, same purpose) | ✔ A19 |
| A20 Eating out | athlete · `ATHLETE_CAPABILITIES` (eating-out tips) | ✔ A20 |
| A21 Daily focus | athlete · `ATHLETE_CAPABILITIES` (accountability) | ✔ A21 |
| A22 Habit completion tracking | athlete · `ATHLETE_PAID` (habit tracking, streaks) — app-side data | — |
| A23 Low motivation | athlete · `ATHLETE_CAPABILITIES` + core `PERSONALITY` (shrink the task) | ✔ A23 |
| A24 Feels guilty | athlete · `ATHLETE_CAPABILITIES` (reframe, reset not shame) | ✔ A24 |
| A25 Check-in reminder | athlete · `ATHLETE_CAPABILITIES` (check-ins) — app-side trigger | — |
| A26 Completes weekly check-in | athlete · `ATHLETE_CAPABILITIES` (summarize week) | ✔ A26 |
| A27 Poor adherence | athlete · `ATHLETE_CAPABILITIES` ("fix consistency FIRST") | ✔ A27 |
| A28 Strong adherence | athlete · `ATHLETE_PAID` (safe progression) | ✔ A28 |
| A29 Plateau | athlete · `ATHLETE_PAID` (plateau analysis: nutrition/training/sleep/stress) | ✔ A29 |
| A30 Recovery issue | athlete · `ATHLETE_PAID` ("prioritize recovery, do not push harder") | ✔ A30 |
| A31 Am I progressing? | athlete · `ATHLETE_CAPABILITIES` (progress beyond weight) | ✔ A31 |
| A32 Weight unchanged | athlete · `ATHLETE_CAPABILITIES` (other indicators) | ✔ A32 |
| A33 Progress photo | core `SAFETY` (no body-shaming) + `ATHLETE_CAPABILITIES` — app-side media | — |
| A34 Performance improves | athlete · `ATHLETE_CAPABILITIES` (strength progress) | ✔ A34 |
| A35 Has active trainer (Companion) | athlete · `ATHLETE_ROLE` (Companion mode) | — (mode default) |
| A36 Asks to change trainer's plan | athlete · `ATHLETE_ROLE` ("never override; draft a message") | ✔ A36 |
| A37 Doesn't understand plan | athlete · `ATHLETE_ROLE` (explain plan simply) | ✔ A37 |
| A38 Message the trainer | athlete · `ATHLETE_ROLE` (draft, never send) | ✔ A38 |
| A39 Prep for trainer check-in | athlete · `ATHLETE_ROLE` (summarize week) | ✔ A39 |
| A40 Needs a human trainer | core `REFERRAL_MAP` | ✔ A40 |
| A41 Injury concern | core `SAFETY` (rules 1–2, 6) + `REFERRAL_MAP` (physiotherapist) | ✔ A41 |
| A42 Sport-specific goal | core `REFERRAL_MAP` (Padel coach) | ✔ A42 |
| A43 Nutrition-only support | core `REFERRAL_MAP` (Nutritionist vs paid meal guidance) | ✔ A43 |
| A44 Too advanced for Solo | core `REFERRAL_MAP` (elite/complex → human) | — |
| A45 Reports pain | core `SAFETY` (rules 1–2: research statement, no diagnosis) | ✔ A45 |
| A46 Asks for a diagnosis | core `SAFETY` (rule 1, no diagnosis) | ✔ A46 |
| A47 Extreme weight loss | core `SAFETY` (rule 3, reject unsafe target) | ✔ A47 |
| A48 Eating-disorder risk | core `SAFETY` (rule 4) | ✔ A48 |
| A49 Mental-health crisis | core `SAFETY` (rule 5, crisis-safe) | ✔ A49 |
| A50 Free depth limit | athlete · `ATHLETE_FREE` (gate advanced programming) | ✔ A50 |
| A51 Free advanced analysis | athlete · `ATHLETE_FREE` (basic + Pro for analysis) | ✔ A51 |
| A52 Free daily accountability | athlete · `ATHLETE_FREE` (limited + paid daily coaching) | — |
| A53 Paid full experience | athlete · `ATHLETE_PAID` (integrated plan) | ✔ A53 |
| A54 Bad week | core `PERSONALITY` + athlete `ATHLETE_CAPABILITIES` (no shame) | ✔ A54 |
| A55 Direct guidance | core `PERSONALITY` (decisive, concise) | ✔ A55 |
| A56 Repeated beginner Qs | core `PERSONALITY` (patient, not judgmental) | ✔ A56 |
| A57–A60 Business outcomes | Emergent from the above (retention, upsell, capture, better check-ins) — not user-facing behaviours | — |

## Athlete Minimum Launch Acceptance — mapping

Trainer vs no-trainer & Solo/Companion switch → `ATHLETE_ROLE` + SESSION `mode`. Clarify goal /
assess level, schedule, equipment → `ATHLETE_CAPABILITIES`. Recommend categories/specializations →
`REFERRAL_MAP`. Basic-for-free / full-for-paid programs & meal guidance → `ATHLETE_FREE` / `ATHLETE_PAID`.
Daily accountability, weekly check-ins, analysis, adjustments, restart help, explain simply, progress
beyond weight, message trainer, never override in Companion, recommend experts, safe language,
maintain tone → the correspondingly-named rules above.

---

## Trainer Assistant (R.Y.X. - Trainer Assistant User Scenerios)

| Scenario(s) | Covered by | Eval |
|---|---|---|
| T1 Understand trainer profile | trainer · `TRAINER_ROLE` + SESSION profile | ✔ T1 |
| T2 Multiple categories | trainer · `TRAINER_ROLE` ("workout lens vs nutrition lens") | ✔ T2 |
| T3 Category ≠ specialization confusion | trainer · `TRAINER_ROLE` (adapt to category+specialization) | ✔ T3 |
| T4 Summarize new client survey | trainer · `TRAINER_OUTPUTS` (Client Brief) | ✔ T4 |
| T5 Identify primary goal | trainer · `TRAINER_OUTPUTS` (Brief: primary/secondary) | ✔ T5 |
| T6 Missing client info | trainer · `TRAINER_JUDGMENT` (flag gaps) + `TRAINER_OUTPUTS` | ✔ T6 |
| T7 Onboarding brief | trainer · `TRAINER_OUTPUTS` (Client Brief, six sections) | ✔ T7 |
| T8 Free summarizes check-in | trainer · `TRAINER_FREE` (check-in summary) | ✔ T8 |
| T9 Free drafts a reply | trainer · `TRAINER_FREE` (simple reply draft) | ✔ T9 |
| T10 Free next-step suggestion | trainer · `TRAINER_FREE` (basic next step) | ✔ T10 |
| T11 Free blocks full program | trainer · `TRAINER_FREE` (gate + basic structure) | ✔ T11 |
| T12 Paid full workout program | trainer · `TRAINER_PAID` + `TRAINER_OUTPUTS` (Program Draft) | ✔ T12 |
| T13 Paid full meal plan | trainer · `TRAINER_PAID` (meal draft) | ✔ T13 |
| T14 Multiple options | trainer · `TRAINER_OUTPUTS` (2–3 options, pros/cons) | ✔ T14 |
| T15 Explain a recommendation | trainer · `TRAINER_ROLE` (explain reasoning on request) | ✔ T15 |
| T16 Analyze weekly check-in | trainer · `TRAINER_OUTPUTS` (Check-in Analysis) | ✔ T16 |
| T17 Detect poor adherence | trainer · `TRAINER_JUDGMENT` ("issue is adherence, keep it simple") | ✔ T17 |
| T18 Detect plateau | trainer · `TRAINER_JUDGMENT` (plateau review points) | ✔ T18 |
| T19 Detect recovery issue | trainer · `TRAINER_JUDGMENT` (recovery before workload) | ✔ T19 |
| T20 Pain/injury mention | trainer · `TRAINER_JUDGMENT` (research statement) + core `SAFETY` | ✔ T20 |
| T21 Basic adjustment | trainer · `TRAINER_JUDGMENT` (reduce intensity, don't overcorrect) | — |
| T22 Advanced adjustment (paid) | trainer · `TRAINER_PAID` (keep/change/why/replacements/focus/draft) | ✔ T22 |
| T23 Provide alternatives | trainer · `TRAINER_ROLE` (offer alternatives) | ✔ T23 |
| T24 Save as client note | trainer · `TRAINER_PAID` (memory) — app-side persistence | — |
| T25 Trainer approves | trainer · `TRAINER_ROLE` (suggest, trainer approves) | ✔ T25 |
| T26 Trainer edits | trainer · `TRAINER_ROLE` (Approve/Edit/Reject) | — |
| T27 Trainer rejects | trainer · `TRAINER_ROLE` (nothing auto-applied) | ✔ T27 |
| T28 Regenerate in a tone | trainer · `TRAINER_ROLE` (regenerate shorter/motivational/professional) | ✔ T28 |
| T29 Explain the suggestion | trainer · `TRAINER_ROLE` (explain logic) | — |
| T30 Motivational feedback | trainer · `TRAINER_JUDGMENT` (specific, personal) | — |
| T31 Supportive after bad week | trainer · `TRAINER_JUDGMENT` (supportive, not aggressive) | ✔ T31 |
| T32 Re-engagement message | trainer · `TRAINER_JUDGMENT` (re-engagement, no guilt) | ✔ T32 |
| T33 Educational feedback | trainer · `TRAINER_JUDGMENT` (clear, goal-specific) | — |
| T34 PT bodybuilding | trainer · `TRAINER_ROLE` (adapt to specialization) | — |
| T35 PT weight loss | trainer · `TRAINER_ROLE` + `TRAINER_JUDGMENT` (adherence/lifestyle) | — |
| T36 Sport Coach football | trainer · `TRAINER_ROLE` (sport-specific) | ✔ T36 |
| T37 Nutritionist nutrition-only | trainer · `TRAINER_ROLE` (nutrition lens, no forced workout) | ✔ T37 |
| T38 Physio rehab | trainer · `TRAINER_JUDGMENT` (research statement) | ✔ T38 |
| T39 Therapist wellness | trainer · `TRAINER_JUDGMENT` + core `SAFETY` (no diagnosis) | ✔ T39 |
| T40 Required research statement | trainer · `TRAINER_JUDGMENT` (mandatory statement) | ✔ T40 |
| T41 Research-informed vs final | trainer · `TRAINER_JUDGMENT` (for professional review) | ✔ T41 |
| T42 Remembers client history | trainer · `TRAINER_PAID` (long-term memory) | ✔ T42 |
| T43 Remembers prior changes | trainer · `TRAINER_PAID` (prior approved changes) | — |
| T44 Remembers trainer prefs | trainer · `TRAINER_PAID` (style memory) | — |
| T45 Free limited memory | trainer · `TRAINER_FREE` (limited memory) | ✔ T45 |
| T46–T48 Upgrade triggers | trainer · `TRAINER_FREE` (gate program/analysis/meal with upgrade line) | ✔ T46 |
| T49 Never auto-send | trainer · `TRAINER_ROLE` (never send) | ✔ T49 |
| T50 Never auto-apply | trainer · `TRAINER_ROLE` (never apply) | ✔ T50 |
| T51 Flag uncertainty | trainer · `TRAINER_JUDGMENT` (thin data → say so) | ✔ T51 |
| T52 Avoid aggressive tone | trainer · `TRAINER_JUDGMENT` + core `PERSONALITY` | ✔ T52 |
| T53 Review my program | trainer · `TRAINER_JUDGMENT` (development on request) | ✔ T53 |
| T54 Improve client feedback | trainer · `TRAINER_JUDGMENT` (improve message) | — |
| T55 Ask for education | trainer · `TRAINER_JUDGMENT` (explain non-progress) | ✔ T55 |
| T56–T58 Dashboard / prioritize / daily briefing | trainer · `TRAINER_OUTPUTS` + `TRAINER_PAID` — app-side data feed | — |
| T59 Specific, not generic | trainer · `TRAINER_JUDGMENT` (reference actual check-in) | ✔ T59 |
| T60 Adapts to specialization | trainer · `TRAINER_ROLE` (category/specialization) | ✔ T60 |
| T61 Structured outputs | trainer · `TRAINER_OUTPUTS` (labelled sections) | ✔ T61 |
| T62 Missing client data | trainer · `TRAINER_JUDGMENT` (ask or limited draft) | — |
| T63 Conflicting data | trainer · `TRAINER_JUDGMENT` (flag conflict) | ✔ T63 |
| T64 Out of scope (escalation) | trainer · `TRAINER_JUDGMENT` (V1.0 no human escalation) | ✔ T64 |
| T65–T69 Business outcomes | Emergent (time saved, more clients, better client experience, consistency) | — |

## Trainer Minimum Launch Acceptance — mapping

Understand category/specialization & multi-category → `TRAINER_ROLE`. Pull trainer/client context →
SESSION + `TRAINER_ROLE`. Summarize onboarding & check-ins, read form + chat → `TRAINER_OUTPUTS`.
Draft feedback, suggest next steps / adjustments, full drafts for paid, gate for free →
`TRAINER_FREE` / `TRAINER_PAID` / `TRAINER_OUTPUTS`. Adapt by category/specialization, required
research statement, all actions under approval, never auto-send/apply, tone, structured outputs,
memory by tier → the correspondingly-named rules above.

---

## Notes

- Rows marked "app-side" depend on data the product feeds RYX (stored check-ins, media, dashboards);
  the brain's behaviour is specified but the eval can't exercise it without that data.
- Emergent business outcomes (A57–A60, T65–T69) are results of the behaviours above, not separate
  instructions, so they have no dedicated rule or eval row.

## Source reference

- `ryx-brain/COVERAGE.md` — Complete file (169 lines)
- `ryx-brain/src/scenarios/athlete.json` — Complete file (466 lines)
- `ryx-brain/src/scenarios/trainer.json` — Complete file (589 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
