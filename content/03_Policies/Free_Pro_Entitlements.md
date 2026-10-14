---
id: "ryx.policy.free_pro_entitlements"
title: "Free Pro Entitlements"
type: "policy"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/envelope.js"
  - "ryx-brain/src/buildSystemPrompt.js"
  - "ryx-brain/src/accounts.js"
  - "ryx-brain/src/credits.js"
  - "ryx-brain/src/cardLayout.js"
  - "ryx-landing/src/lib/cardLayout.js"
  - "ryx-landing/src/components/cards/RyxContentCard.jsx"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: true
decision_ids:
  - "H01"
  - "H03"
  - "H06"
  - "H07"
  - "H10"
---

# Free Pro Entitlements

## Authority and scope

This is the single authoritative entitlement matrix for RYX-generated coaching output. It uses existing Athlete/Trainer Free/Pro instructions and implemented feature contracts; it creates no new product feature or pricing.

Safety, access, core, role and mode rules take precedence over tier. Entitlements do not grant data access, professional clearance, autonomous delivery, new memory storage or a capability absent from the backend.

## Useful basic value

Free must provide useful basic value. When a Pro-only depth/feature is requested, deliver the useful permitted starter/summary/draft first, then at most one natural value-based Pro line. Incomplete unrelated profile fields do not remove that value.

Pro supports deeper analysis, richer outputs and existing expanded generation, with deliver-first under [[Response_Principles#Request-specific sufficiency and deliver-first]]. It receives no upgrade nudges.

## Generation and visibility interpretation

Available means within existing safety/context/capability limits. “Depth” means a richer output for an existing feature; “availability” means an existing generation feature restricted to Pro. “Not generated” means no Pro-only detailed payload is generated for a Free request.

Generated but locked: NONE is required by this candidate's canonical strategy for RYX-generated coaching. Free receives the useful basic output visibly; Pro-only depth is not generated for Free and hidden. Historical advanced-section/card-note locking is C08/C09/C10 and remains archived for future runtime/UI alignment.

Mandatory safety/research wording, required referrals, usable basic safety cues and Free basic protein/hydration guidance stay visible. A UI preview cannot substitute for generating a usable basic answer.

## Entitlement matrix

| Existing feature | Free generation and visibility | Pro generation and visibility | Generated but locked | Not generated / capability limit | Difference |
|---|---|---|---|---|---|
| Goal clarification, general fitness questions, expert matching | Useful basic answer and named category, visible | Contextual answer with the same scope/referral obligations | None | No invented user data or expert credentials | Depth |
| Beginner workout ideas and basic weekly structure | Usable starter structure/example days/exercises, visible | Personalized schedule and richer prescriptions from confirmed context | None | Free does not generate the full personalized multi-week program | Depth and availability |
| Exercise explanation, basic form cues, regression and available demo | Simple usable explanation and known available demo, visible | Contextual richer explanation/progression as requested | None | No unavailable tutorial or equipment assumed | Depth; media capability unchanged |
| Full personalized multi-week program/periodized blocks | Basic starter structure only | Complete program draft with exercises, sets/reps/rest/progression and assumptions | None | Detailed personalized multi-week generation not generated on Free | Availability |
| Workout/program adjustment | Basic practical next step within mode ownership | Specific progression/adjustment from current data; trainer review when applicable | None | Deep adjustment/restructure not generated on Free; no overriding assigned trainer plan | Depth and availability |
| General meal framework, protein/hydration and basic food guidance | Useful basic structure/tips, visible | Richer contextual meal guidance | None | No unsafe restriction or expanded clinical nutrition scope | Depth |
| Detailed meal plans, grocery support and schedule/travel/Ramadan adaptation | General meal framework only | Existing personalized meal drafts, examples, swaps and grocery support | None | Full detailed meal plan/grocery list not generated on Free | Availability |
| Basic weekly reflection and progress/plateau explanation | Basic wins, struggle, adherence/recovery observations and simple next focus | Deeper pattern/plateau interpretation and concrete next steps from available data | None | Deep multi-week trend/adherence/plateau analysis not generated on Free | Depth |
| Daily motivation and accountability | Simple motivation, basic daily focus and practical restart | Existing ongoing daily coaching output and integrated training/nutrition/habit focus | None | No autonomous scheduled outreach or unsupported background coaching claimed | Depth |
| Todo/list saving, completion and logged progress records | Existing app actions; basic coaching references to confirmed records | Same existing app actions; richer contextual coaching | None | No automatic task completion or absent persistent streak/score engine claimed | Depth; app availability unchanged |
| Advanced adherence/streak interpretation | Basic consistency reflection | Analysis only from supplied confirmed data | None | No claim that an unimplemented persistent analytics engine exists | Depth; backend capability unchanged |
| Photo/form/image analysis | Not currently available through the inspected text-only production chat path | Not currently available through that path | None | Future/planned until actual media context/analysis capability exists; the source-defined action price is not proof of availability | Capability limit, not a new commercial feature |
| Trainer client survey brief/basic snapshot | Basic scannable brief/summary with missing facts identified | Richer contextual interpretation/coaching approach | None | No fabricated client fields or roster | Depth |
| Trainer weekly check-in summary/client reply draft | Basic summary, key progress/struggle, simple next step and specific supportive draft | Full existing analysis sections and deeper trend/proposal output | None | Detailed multi-week/deep analysis not generated on Free | Depth |
| Trainer full workout/meal program drafts | Useful basic weekly/meal structure first | Full complete reviewable replacement/draft under Trainer_Approval_Model | None | Full generation not generated on Free | Availability |
| Trainer multiple program strategies and deep adjustments | Basic direction or one useful starter only | Existing materially different conservative/moderate/aggressive options where appropriate, with pros/cons and why | None | Multiple detailed program options/deep adjustments not generated on Free | Availability |
| Trainer basic communication/re-engagement wording | Simple supportive client-message draft | Richer specific drafts and existing retention/re-engagement strategy on request | None | Advanced retention strategy not generated on Free; no auto-send | Depth and availability |
| Trainer-development explanation | Simple trainer questions and basic feedback when asked | Existing detailed review/improvement reasoning when asked | None | No unsolicited critique or claimed automatic program repair | Depth |
| Conversation context and memory | Current/recent supplied context and existing saved CORYX data | Current/recent supplied context and existing saved CORYX data; use actual supplied history for deeper output | None | No promise of an unlimited/durable trainer-style or client-note memory store | Capability truth; see Memory_Policy |
| Backend context display depth | Existing Free formatter caps are documented in Athlete_Snapshot | Existing Pro formatter caps are documented there | None required canonically | Formatting depth is not authorization; raw current-runtime additions do not invent entitlements | Depth |
| Assigned program reading and explicit trainer approval | Existing authenticated relationship/ownership checks apply | Same checks apply | None required canonically | Tier never grants ownership, authorization or autonomous writes | App availability unchanged |
| DM, Body Map, check-in, event and todo app records | Existing authenticated app capabilities remain | Same existing app capabilities remain | None required canonically | No newly promised storage, delivery, staff escalation or service | App availability unchanged |
| Marketplace catalog/library/purchase stub/adapt hook | Existing authenticated backend contracts; RYX guidance stays basic | Same contracts; RYX generation may be richer | No new marketplace visibility policy defined | Stub purchase is not verified payment; owned-program commercial display policy needs separate product confirmation | App availability unchanged; no pricing change |
| Manual conversation report/support recommendation | Existing manual record submission or recommendation | Same | None | No guaranteed staff review, email/webhook escalation or automatic support delivery | Capability truth |
| Credit allowance | Existing 30 credits per fixed 30-day cycle; no rollover | Existing 600 credits per fixed 30-day cycle; up to 100 rollover | Not a content lock | Generation is metered under Credit_and_Tier_Rules | Existing allowance, no new pricing |

## Tier references and runtime alignment

[[Athlete_Free]], [[Athlete_Pro]], [[Trainer_Free]] and [[Trainer_Pro]] reference this matrix instead of defining separate entitlement lists. Existing implementation discrepancies remain in C08/C09/C10/C11/C17.

Commercial treatment of owned marketplace content outside RYX-generated coaching is not newly decided here. The matrix preserves existing backend availability, and [[CANONICALIZATION_REVIEW#Decisions requiring boss/product confirmation]] records the remaining commercial ambiguity.

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `ryx-brain/src/prompts/core.js`
- `ryx-brain/src/prompts/athlete.js`
- `ryx-brain/src/prompts/trainer.js`
- `ryx-brain/src/envelope.js`
- `ryx-brain/src/buildSystemPrompt.js`
- `ryx-brain/src/accounts.js`
- `ryx-brain/src/credits.js`
- `ryx-brain/src/cardLayout.js`
- `ryx-landing/src/lib/cardLayout.js`
- `ryx-landing/src/components/cards/RyxContentCard.jsx`

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
