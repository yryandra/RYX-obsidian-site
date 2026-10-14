---
id: "ryx.review.brain_decisions"
title: "RYX Brain Decisions"
type: "policy"
status: "review"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "CORYX-RYX-Brain/MIGRATION_REVIEW.md"
  - "ryx-brain/src/prompts/athlete.js"
  - "ryx-brain/src/prompts/trainer.js"
  - "ryx-brain/src/envelope.js"
  - "ryx-brain/src/profileFunnel.js"
  - "ryx-brain/src/server.js"
  - "ryx-brain/src/prompts/core.js"
  - "ryx-brain/src/replyGuards.js"
  - "ryx-brain/src/eval.js"
  - "ryx-brain/src/evalOpenai.js"
  - "ryx-brain/src/bodymapFormat.js"
  - "ryx-brain/src/buildSystemPrompt.js"
  - "ryx-landing/src/App.jsx"
  - "ryx-landing/src/lib/cardLayout.js"
  - "ryx-landing/src/components/cards/RyxContentCard.jsx"
  - "ryx-brain/src/accounts.js"
  - "ryx-brain/src/credits.js"
  - "ryx-brain/README.md"
  - "ryx-brain/docs/accounts.md"
  - "ryx-brain/docs/shared-athlete-data.md"
  - "ryx-brain/src/identityRoutes.js"
  - "ryx-brain/src/chatIntake.js"
  - "ryx-brain/docs/reports.md"
  - "ryx-brain/docs/event-countdown.md"
  - "ryx-brain/src/events.js"
  - "ryx-brain/src/labMemory.js"
  - "ryx-brain/src/identity.js"
  - "ryx-brain/src/programs.js"
  - "ryx-brain/src/athleteSnapshot.js"
  - "ryx-brain/src/runChat.js"
  - "ryx-brain/src/openaiRun.js"
  - "ryx-brain/src/labSessions.js"
  - "ryx-brain/docs/body-map.md"
  - "ryx-brain/src/bodymapRegions.js"
  - "ryx-brain/src/bodymap.js"
  - "RYX_Wedge_Knowledge_Bases_v1/index.json"
  - "ryx-brain/src/knowledge/wedgeRouter.js"
  - "ryx-brain/src/knowledge/wedgeFormat.js"
  - "ryx-brain/src/knowledge/README.md"
  - "ryx-brain/src/labInsights.js"
  - "ryx-brain/COVERAGE.md"
last_reviewed: "2026-10-14"
canonical: false
---

# RYX Brain Decisions

## Status

Canonicalization decisions for the reviewed Obsidian brain.
These decisions do not yet imply production runtime implementation.

The H01–H12 decisions below are approved by the Phase 2 request dated 2026-10-14. This record does not silently resolve additional product questions. [[MIGRATION_REVIEW]] and [[MIGRATION_MAP]] remain unchanged. Existing note wording is available in [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## H01 — Deliver-first versus unrelated intake

### Existing conflict

[[MIGRATION_REVIEW#C01 — Pro delivery versus incomplete-intake gate]]

Pro prompts say deliver concrete output first when context exists; the production athlete intake gate strips weekly_plan/major_adjustment/advanced_multistep cards on incomplete profiles without a tier exemption. The post-model executed gate can defeat the prompt contract.

### Decision

Useful output is delivered when the specific request has sufficient required context. Intake blocks only missing safety/correctness, permission/context or operation-critical information. Noncritical assumptions/limitations are explicit and optional refinement follows value; Pro remains deliver-first and Free uses the central depth matrix.

### Brain notes affected

- [[01_Core/Response_Principles]]
- [[02_Roles/Athlete/Athlete_Role]]
- [[02_Roles/Athlete/Athlete_Free]]
- [[02_Roles/Athlete/Athlete_Pro]]
- [[02_Roles/Trainer/Trainer_Role]]
- [[02_Roles/Trainer/Trainer_Free]]
- [[02_Roles/Trainer/Trainer_Pro]]
- [[07_Workflows/Intake_and_Journey_Rules]]
- [[07_Workflows/Athlete_Onboarding]]
- [[09_Runtime_Context/SESSION]]

### Runtime code requiring future alignment

- `ryx-brain/src/prompts/athlete.js`
- `ryx-brain/src/prompts/trainer.js`
- `ryx-brain/src/envelope.js`
- `ryx-brain/src/profileFunnel.js`
- `ryx-brain/src/server.js`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## H02 — Terminal crisis and final safety

### Existing conflict

[[MIGRATION_REVIEW#C02 — Crisis safety versus later intake processing]]

The crisis guard removes questions/cards and returns quick_question. Production still runs intake enforcement and question coercion afterward without a crisis exemption; an incomplete profile can receive an intake question again. The inspected pipeline does not rerun guards at the end.

[[MIGRATION_REVIEW#C03 — Crisis prompt versus keyword guard acceptance]]

Prompt requires no fitness/questions, care/urgency and 2–4 sentences, with broad crisis/hopelessness recognition. Guard triggers on a narrower phrase set and accepts any existing lead containing emergency/999/911/crisis/helpline/suicide, without checking fitness framing, sentence count or coaching questions.

### Decision

Crisis is terminal within the response. No intake, card/task, upsell, unrelated question or normal coaching may resume or be appended. Preserve existing concise/calm urgent-support scope. Future runtime final safety enforcement occurs AFTER all normal response coercion; source is not yet aligned.

### Brain notes affected

- [[03_Policies/Crisis_Handling]]
- [[03_Policies/Safety]]
- [[03_Policies/Deterministic_Reply_Guards]]
- [[01_Core/Brain_Architecture]]
- [[01_Core/Response_Principles]]
- [[07_Workflows/Intake_and_Journey_Rules]]
- [[07_Workflows/Daily_Training]]
- [[07_Workflows/Body_Map_Response]]
- [[08_Evals/Eval_System]]

### Runtime code requiring future alignment

- `ryx-brain/src/prompts/core.js`
- `ryx-brain/src/replyGuards.js`
- `ryx-brain/src/profileFunnel.js`
- `ryx-brain/src/server.js`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## H03 — Full visible research sentence and referral

### Existing conflict

[[MIGRATION_REVIEW#C04 — Exact research sentence/order/referral versus prefix guard]]

Prompt requires the full verbatim sentence before any treatment-style suggestion. Guard checks only a prefix across lead/card note, appends the sentence after existing content, and adds a physiotherapist referral only if that prefix is absent. A partial prefix or existing card-note prefix may bypass lead/referral/order requirements. Eval hard gates also check the prefix.

[[MIGRATION_REVIEW#C10 — Mandatory safety card note versus Free note locking]]

The output directive uses card.note for the mandatory research statement. Free workout/program/meal/analysis note footers are locked in the app. Guards may add it to lead, but an existing prefix in card.note suppresses that addition. The required statement can remain in a locked note.

### Decision

Safety owns the unchanged full exact research sentence. When triggered, it is user-visible before treatment-style/rehabilitation guidance, never a prefix-only check or exclusively hidden card.note. Preserve the existing required professional referral independently; do not expand medical scope.

### Brain notes affected

- [[03_Policies/Safety]]
- [[03_Policies/Pain_and_Injury]]
- [[03_Policies/Referral_Rules]]
- [[03_Policies/Deterministic_Reply_Guards]]
- [[01_Core/Output_and_Card_Behaviour]]
- [[08_Evals/Eval_System]]

### Runtime code requiring future alignment

- `ryx-brain/src/prompts/core.js`
- `ryx-brain/src/prompts/trainer.js`
- `ryx-brain/src/replyGuards.js`
- `ryx-brain/src/eval.js`
- `ryx-brain/src/evalOpenai.js`
- `ryx-brain/src/envelope.js`
- `ryx-landing/src/lib/cardLayout.js`
- `ryx-landing/src/components/cards/RyxContentCard.jsx`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## H04 — Active pain and confirmed safety context

### Existing conflict

[[MIGRATION_REVIEW#C05 — Active-pain clearance versus body-map modification advice]]

Core prohibits exercise modifications before professional clearance when pain is active. Body-map SESSION instructs modifications/avoidance for flagged regions and swaps/mobility for severe regions without a separate clearance condition. Keep both sources visible; safety is explicitly highest priority in the prompt but the lower block still exists.

[[MIGRATION_REVIEW#C15 — No invented context/clearance versus intake heuristics]]

Executed extraction can infer equipment from sport, schedule from the whole thread including assistant suggestions, noInjuries from sessionStart+schedule, and cleared/monitoring return from the word physio. Scored labels can overwrite specific extracted values. Some inferred fields are not persisted by saveProfile. These may be rendered as established facts despite the prompt prohibition on inventing data; no inference fix applied.

### Decision

Safety overrides Body Map optimization. Clearance sufficient for the specific action must be explicit; physio/treatment mentions, a prior professional visit, improved pain or monitoring do not establish it. Inference cannot silently create clearance, equipment, permission or other protected facts. General non-diagnostic guidance remains distinct from clearance-dependent guidance within existing scope.

### Brain notes affected

- [[03_Policies/Safety]]
- [[03_Policies/Pain_and_Injury]]
- [[04_Domains/Body_Map]]
- [[04_Domains/Athlete_Profile]]
- [[09_Runtime_Context/Known_Context]]
- [[09_Runtime_Context/Data_Boundary]]
- [[06_Tools/Update_Athlete_Profile]]

### Runtime code requiring future alignment

- `ryx-brain/src/prompts/core.js`
- `ryx-brain/src/bodymapFormat.js`
- `ryx-brain/src/labMemory.js`
- `ryx-brain/src/identity.js`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## H05 — Authoritative mode and trainer ownership

### Existing conflict

[[MIGRATION_REVIEW#C06 — Unknown-mode Companion prompt versus renderer/guard parameter]]

Athlete prompt treats a mentioned existing coach with unknown mode as Companion. Renderer uses Solo for any mode other than companion, guards depend on explicit mode, and production forces Companion only for an assigned program. The live frontend also sends mode solo. A relationship or trainer mention alone is not the same executed mode signal.

[[MIGRATION_REVIEW#C07 — Companion drafting format and conditional override protection]]

Role requests quoted draft text starting Draft message:. Guard wraps tell/message-my-trainer replies under another label and has a fixed leg-day draft for recognized change requests. If lead already contains draft message to your trainer, the change branch leaves any existing card/question intact. Trigger vocabulary is narrower than the role rule.

### Decision

Mode comes from authoritative CORYX backend/app state, not casual trainer/coach mentions. In Companion, RYX supports human program ownership and may suggest/draft for review without overriding it. Trainer-directed drafts use the visible prefix Draft message:. Claims of sending/applying require confirmed backend execution; chat approval wording alone is insufficient.

### Brain notes affected

- [[02_Roles/Athlete/Companion_Mode]]
- [[02_Roles/Athlete/Solo_Mode]]
- [[03_Policies/Trainer_Athlete_Access]]
- [[02_Roles/Trainer/Trainer_Approval_Model]]
- [[01_Core/Response_Principles]]
- [[06_Tools/Draft_Message]]
- [[07_Workflows/Program_Adjustment]]
- [[07_Workflows/Trainer_Client_Message_Draft]]

### Runtime code requiring future alignment

- `ryx-brain/src/prompts/athlete.js`
- `ryx-brain/src/buildSystemPrompt.js`
- `ryx-brain/src/server.js`
- `ryx-brain/src/replyGuards.js`
- `ryx-landing/src/App.jsx`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## H06 — One entitlement matrix and visible Free value

### Existing conflict

[[MIGRATION_REVIEW#C08 — Free useful reflection versus feature/depth restrictions]]

Athlete workflows allow a basic plateau explanation while ATHLETE_FREE gates plateau analysis; trainer Free summary/message contracts coexist with the output directive requiring full matching formats. UI locks later analysis/meal sections, including hydration, observations and suggested actions. These overlapping depth distinctions remain unresolved, not expanded by migration.

[[MIGRATION_REVIEW#C09 — Free advanced-section previews versus basic-only cards]]

SESSION tells Free athlete cards to include Warm-up/Main and advanced Finisher/Cool-down/Form cues/Progression/Recovery sections for UI locks. RESPONSE_DIRECTIVE says Free cards should remain basic. Actual app gating changes visibility, not the received payload.

### Decision

Free_Pro_Entitlements is the sole feature/depth authority. Canonical interpretation: generate useful basic Free content visibly; do not generate Pro-only detailed content for Free and then hide it. No generated-but-locked Pro-only coaching payload is required by this candidate. Keep safety/research wording and useful basic safety/protein/hydration information visible. Pro receives existing richer generation/depth within actual capabilities; no new commercial features or pricing.

### Brain notes affected

- [[03_Policies/Free_Pro_Entitlements]]
- [[02_Roles/Athlete/Athlete_Free]]
- [[02_Roles/Athlete/Athlete_Pro]]
- [[02_Roles/Trainer/Trainer_Free]]
- [[02_Roles/Trainer/Trainer_Pro]]
- [[02_Roles/Trainer/Trainer_Outputs]]
- [[01_Core/Output_and_Card_Behaviour]]

### Runtime code requiring future alignment

- `ryx-brain/src/prompts/athlete.js`
- `ryx-brain/src/prompts/trainer.js`
- `ryx-brain/src/envelope.js`
- `ryx-landing/src/lib/cardLayout.js`
- `ryx-brain/src/buildSystemPrompt.js`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## H07 — Metered wording and final-action billing

### Existing conflict

[[MIGRATION_REVIEW#C11 — Unlimited-credit upsell example versus actual metering]]

Directive upsell examples include unlimited credits. Actual Pro account grants 600 per fixed 30-day cycle plus capped 100 rollover and remains action-metered. No entitlement/credit logic was changed.

[[MIGRATION_REVIEW#C18 — Returned action versus final billed cost]]

Model action sets creditCost after a pre-estimate gate. Crisis guard changes action without recalculating cost; production funnel stripping also changes action without explicit cost update (Lab recalculates). Later card coercion recalculates only on its own action change. Final cost can exceed available prechecked credits; deduction floors at zero. No charging change applied.

### Decision

Remove the unsupported unbounded-credit promise. Preserve Free 30 credits per fixed 30-day cycle, Pro 600 with up to 100 rollover, and all source action weights. Future final executed/billed action sets cost after model/guards/coercion, then balance is verified, charged once and a ledger entry persisted. The ledger/sequence is future alignment, not implemented capability or new pricing.

### Brain notes affected

- [[03_Policies/Credit_and_Tier_Rules]]
- [[03_Policies/Free_Pro_Entitlements]]
- [[01_Core/Brain_Architecture]]
- [[01_Core/Output_and_Card_Behaviour]]
- [[06_Tools/Get_Account]]
- [[06_Tools/Change_Plan_and_Credits]]

### Runtime code requiring future alignment

- `ryx-brain/src/envelope.js`
- `ryx-brain/src/accounts.js`
- `ryx-brain/src/credits.js`
- `ryx-brain/src/runChat.js`
- `ryx-brain/src/openaiRun.js`
- `ryx-brain/src/replyGuards.js`
- `ryx-brain/src/profileFunnel.js`
- `ryx-brain/src/server.js`
- `ryx-brain/src/labSessions.js`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## H08 — Authenticated access and truthful reporting

### Existing conflict

[[MIGRATION_REVIEW#C12 — Older fixture/userId documentation versus authenticated production]]

Older README/account sections describe fixture-backed HERD context/localStorage user IDs and request userId. Current production uses authenticated role/identity, relationship-checked fresh snapshots and saved profiles, and ignores HERD fixtures. Shared-athlete-data documentation describes the newer implementation; preserve the distinction.

[[MIGRATION_REVIEW#C13 — Report listing/auth and auto-escalation documentation]]

reports.md labels GET report listing no-auth admin/Lab MVP; current ordinary user sessions are blocked from that diagnostic listing. A user-submitted persisted report exists; trainer prompt/guard still says automatic human escalation is unavailable. No email/webhook or guaranteed human response is implemented.

### Decision

Authenticated CORYX identity and active relationship checks are canonical. Fixture/localStorage/no-auth access guidance is legacy/reference_only. Distinguish recommending support contact from executed contact. No auto staff escalation, guaranteed human review, email/webhook escalation or message delivery is promised without actual backend performance and confirmation; a manual persisted report is not proof of those services.

### Brain notes affected

- [[03_Policies/Data_Access]]
- [[03_Policies/Trainer_Athlete_Access]]
- [[03_Policies/RYX_Boundaries]]
- [[09_Runtime_Context/Data_Boundary]]
- [[06_Tools/Report_Conversation]]
- [[04_Domains/Direct_Messaging]]

### Runtime code requiring future alignment

- `ryx-brain/README.md`
- `ryx-brain/docs/accounts.md`
- `ryx-brain/docs/shared-athlete-data.md`
- `ryx-brain/src/server.js`
- `ryx-brain/src/identityRoutes.js`
- `ryx-brain/src/chatIntake.js`
- `ryx-brain/docs/reports.md`
- `ryx-brain/src/prompts/trainer.js`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## H09 — Current Body Map and most recent past event

### Existing conflict

[[MIGRATION_REVIEW#C14 — Past active-event selector]]

Documentation says nearest future or most recent past active event. getActiveEvent sorts ascending and chooses the earliest when all active candidates are past. Current write paths tend to enforce a single active event; the fallback still differs.

[[MIGRATION_REVIEW#C20 — Body-map documentation versus current catalog/schema]]

Older document lists23 coarse regions and only1–10 input. Code has34 zones, more aliases, feelType and original5/10 reporting scales. The vault domain/catalog follows executed schema and records the stale document explicitly.

### Decision

Body Map documents the implemented 34 zones, aliases, feelType, original 5/10 rating scales and normalized representation, without records. The old 23-region document is stale/legacy. Most recent past active event means the most recent past date, not earliest historical date; this semantic intent does not modify events.js.

### Brain notes affected

- [[04_Domains/Body_Map]]
- [[04_Domains/Body_Region_Catalog]]
- [[04_Domains/Events]]
- [[06_Tools/Get_Events]]
- [[09_Runtime_Context/Athlete_Snapshot]]

### Runtime code requiring future alignment

- `ryx-brain/docs/event-countdown.md`
- `ryx-brain/src/events.js`
- `ryx-brain/docs/body-map.md`
- `ryx-brain/src/bodymapRegions.js`
- `ryx-brain/src/bodymap.js`
- `ryx-brain/src/athleteSnapshot.js`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## H10 — Truthful memory and independent trainer greeting

### Existing conflict

[[MIGRATION_REVIEW#C17 — Free/Pro memory promise versus current loading/persistence]]

Pro promises long-term client/style memory and Free recent context only. The same trainer-history query loads at most 24 turns for either tier; no dedicated durable client-note/style preference store is present. Raw snapshot additions also bypass several formatted Free history caps. Actual persistence is documented separately from prompt promises.

[[MIGRATION_REVIEW#C19 — Trainer first-contact prompt versus mandatory client selection]]

Prompt says greet a first-time trainer by name/category/specialization and list capabilities. Production resolveAthlete can return which-client/no-athletes clarification before invoking the model, even for hey/first-contact requests. The general prompt introduction is therefore not always reached.

### Decision

Separate current conversation, recent history, implemented persisted records, CORYX profile/data and future preference memory. Promise only implemented memory; a durable trainer-style/client-note store is not currently available. A generic trainer greeting/capability explanation needs no athlete selection; athlete-specific data/action does require authorized selection.

### Brain notes affected

- [[03_Policies/Memory_Policy]]
- [[02_Roles/Trainer/Trainer_Role]]
- [[02_Roles/Trainer/Trainer_Free]]
- [[02_Roles/Trainer/Trainer_Pro]]
- [[09_Runtime_Context/SESSION]]
- [[02_Roles/Trainer/Trainer_Outputs]]

### Runtime code requiring future alignment

- `ryx-brain/src/prompts/trainer.js`
- `ryx-brain/src/identity.js`
- `ryx-brain/src/athleteSnapshot.js`
- `ryx-brain/src/server.js`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## H11 — Confirmed equipment and explicit program gaps

### Existing conflict

[[MIGRATION_REVIEW#C16 — Equipment-only prescriptions versus marketplace bodyweight swaps]]

Athlete rules use only available equipment. Adapt hook groups home and bodyweight together and replaces gym movements with DB/band alternatives, so a bodyweight-only profile can receive equipment it lacks. This fixed hook remains separate from LLM behavior.

Also see the existing missing-template-week/day limitation in [[Programs]] and the archived program note.

### Decision

Use confirmed available equipment; bodyweight-only never implies dumbbells, bands, barbells, machines or other equipment. Ask when required or offer clearly labelled alternatives when equipment is unknown. Do not silently invent/reuse missing weeks/days as source content. Any RYX gap fill is labelled a suggestion/draft and follows Solo/Companion/Trainer ownership and review.

### Brain notes affected

- [[04_Domains/Programs]]
- [[04_Domains/Athlete_Profile]]
- [[04_Domains/Training_Sessions]]
- [[06_Tools/Adapt_Purchased_Program]]
- [[07_Workflows/Program_Generation]]
- [[07_Workflows/Program_Adjustment]]
- [[07_Workflows/Trainer_Program_Draft]]

### Runtime code requiring future alignment

- `ryx-brain/src/prompts/athlete.js`
- `ryx-brain/src/programs.js`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## H12 — Provenance-preserving retrieval and full-pipeline evaluation

### Existing conflict

[[MIGRATION_REVIEW#C21 — Intended retrieval contract versus actual projection]]

Index describes taxonomy filtering, meaningful chunks, claim/source preservation and validation/refresh checks. Current router is substring scoring; formatter drops IDs, omits fields, slices arrays/objects and capscharacters. Knowledge README also shows an older collection path; loader uses repository root. Full KB storage is preserved without assuming the current model receives it all.

[[MIGRATION_REVIEW#C22 — Evaluation-path descriptions versus executed coverage]]

Anthropic evaluator bypasses retrieval/envelope/guards/server processing. OpenAI evaluator comments imply Lab+funnel equivalence but it omits actual server/Lab postprocessing; provider selection can follow configuration. Coverage is a documentary matrix, not an up-to-date passing report, and Lab safety metrics permit weaker generic review wording.

### Decision

Preserve complete structured knowledge, stable note/knowledge/claim IDs where present, source references, taxonomy, caveats and safety boundaries. Future retrieved units retain provenance and content together; no retriever is implemented. Production-quality evaluation must exercise the complete user-visible prompt/context/retrieval/model/guards/intake/coercion/formatting/final-safety pipeline, not raw provider output alone.

### Brain notes affected

- [[05_Knowledge/Knowledge_System]]
- [[06_Tools/Retrieve_Knowledge]]
- [[08_Evals/Eval_System]]
- [[08_Evals/Coverage]]

### Runtime code requiring future alignment

- `RYX_Wedge_Knowledge_Bases_v1/index.json`
- `ryx-brain/src/knowledge/wedgeRouter.js`
- `ryx-brain/src/knowledge/wedgeFormat.js`
- `ryx-brain/src/knowledge/README.md`
- `ryx-brain/src/eval.js`
- `ryx-brain/src/evalOpenai.js`
- `ryx-brain/src/labInsights.js`
- `ryx-brain/COVERAGE.md`
- `ryx-brain/src/server.js`

Current code/documentation can already satisfy individual parts (for example authenticated access and the Body Map schema). This group is not claimed fully aligned, and no source file is modified here.

### Status

brain_updated
runtime_not_yet_aligned

## Canonical Rule Ownership

| Rule Family | Canonical Note | Referencing Notes |
|---|---|---|
| D01 — voice/tone | [[Personality_and_Voice#Voice and tone]] | [[Athlete_Role]]; [[Trainer_Role]]; [[Response_Principles]]; [[Athlete_Onboarding]]; [[Trainer_Client_Message_Draft]] |
| D02 — safety/no diagnosis/research | [[Safety#Research statement and professional review]] | [[Pain_and_Injury]]; [[Referral_Rules]]; [[Body_Map]]; [[Body_Map_Response]]; [[Output_and_Card_Behaviour]]; [[Deterministic_Reply_Guards]]; [[Trainer_Role]] |
| D03 — Companion trainer ownership | [[Companion_Mode#Trainer ownership]] | [[Athlete_Role]]; [[Solo_Mode]]; [[Trainer_Athlete_Access]]; [[Programs]]; [[Program_Adjustment]]; [[Draft_Message]] |
| D04 — Trainer suggests/approves | [[Trainer_Approval_Model#Trainer suggests, trainer approves]] | [[Trainer_Role]]; [[Trainer_Outputs]]; [[Trainer_Program_Draft]]; [[Trainer_Client_Message_Draft]]; [[Draft_Program]]; [[Approve_Program_Draft]]; [[Update_Assigned_Program]] |
| D05 — Pro deliver-first | [[Response_Principles#Request-specific sufficiency and deliver-first]] | [[Athlete_Pro]]; [[Trainer_Pro]]; [[Athlete_Role]]; [[Trainer_Role]]; [[Intake_and_Journey_Rules]]; [[SESSION]]; [[Program_Generation]] |
| D06 — Free useful basic value | [[Free_Pro_Entitlements#Useful basic value]] | [[Athlete_Free]]; [[Trainer_Free]]; [[Trainer_Outputs]]; [[Output_and_Card_Behaviour]]; [[Check_Ins]]; [[Nutrition_Guidance]] |
| D07 — knowledge provenance/evidence | [[Knowledge_System#Provenance and evidence]] | [[Retrieve_Knowledge]]; [[General]]; [[Bodybuilding]]; [[Calisthenics]]; [[CrossFit]]; [[Powerlifting]]; [[Football]]; [[Basketball]]; [[Swimming]]; [[Padel]]; [[Tennis]]; [[Golf]]; [[Combat]]; [[Rehab_and_Therapy]]; [[Yoga_and_Mind_Body]]; [[Exercise_Library]]; [[Exercise_Media_Catalog]]; [[Form_Demos_By_Wedge]] |
| D08 — fresh data/no invented records | [[Data_Boundary#Data truth precedence]] | [[Known_Context]]; [[SESSION]]; [[Athlete_Snapshot]]; [[Data_Access]]; [[Athlete_Profile]]; [[Check_Ins]]; [[Training_Sessions]]; [[Body_Map]]; [[Todos_and_Habits]]; [[Goals]]; [[Events]]; [[Progress_and_Adherence]]; [[Direct_Messaging]] |

References use their owner rather than repeat the competing rule. Original source_files, the unchanged historical migration map and exact archived source projections preserve traceability. Retained raw knowledge payloads are provenance-bearing source content subordinate to the hierarchy, not additional owners.

## Additional decisions not approved

- P01 — Authoritative mode-state contract: Choose the eventual backend/app mode field and how an active trainer/program relationship establishes ownership. The approved principle is fixed; no new resolver schema or casual-text fallback has been invented.
- P02 — Owned marketplace display/commercial rules: Confirm how an already-owned marketplace program is displayed relative to the RYX subscription tier. The candidate decides RYX-generated coaching depth, preserves current backend catalog/library/stub contracts and changes no owned-content unlock policy or pricing.
- P03 — Billing failure and ledger edge policy: Confirm failed/cancelled turns, concurrent balance checks, retries, refunds and ledger/idempotency semantics beyond the approved final-action cost/verify/charge-once/persist sequence. No new fee/refund or transaction schema is invented.
- P04 — Future durable preference/client-note memory: Confirm future storage scope, retention and permission design if that feature is later implemented. Current capabilities are described truthfully; this is not a current Pro promise or a newly approved feature.

These forward-looking questions do not reverse the H01–H12 decisions. They are recorded for boss/product confirmation in [[CANONICALIZATION_REVIEW#Decisions requiring boss/product confirmation]].

## Source reference

- `CORYX-RYX-Brain/MIGRATION_REVIEW.md`
- `ryx-brain/src/prompts/athlete.js`
- `ryx-brain/src/prompts/trainer.js`
- `ryx-brain/src/envelope.js`
- `ryx-brain/src/profileFunnel.js`
- `ryx-brain/src/server.js`
- `ryx-brain/src/prompts/core.js`
- `ryx-brain/src/replyGuards.js`
- `ryx-brain/src/eval.js`
- `ryx-brain/src/evalOpenai.js`
- `ryx-brain/src/bodymapFormat.js`
- `ryx-brain/src/buildSystemPrompt.js`
- `ryx-landing/src/App.jsx`
- `ryx-landing/src/lib/cardLayout.js`
- `ryx-landing/src/components/cards/RyxContentCard.jsx`
- `ryx-brain/src/accounts.js`
- `ryx-brain/src/credits.js`
- `ryx-brain/README.md`
- `ryx-brain/docs/accounts.md`
- `ryx-brain/docs/shared-athlete-data.md`
- `ryx-brain/src/identityRoutes.js`
- `ryx-brain/src/chatIntake.js`
- `ryx-brain/docs/reports.md`
- `ryx-brain/docs/event-countdown.md`
- `ryx-brain/src/events.js`
- `ryx-brain/src/labMemory.js`
- `ryx-brain/src/identity.js`
- `ryx-brain/src/programs.js`
- `ryx-brain/src/athleteSnapshot.js`
- `ryx-brain/src/runChat.js`
- `ryx-brain/src/openaiRun.js`
- `ryx-brain/src/labSessions.js`
- `ryx-brain/docs/body-map.md`
- `ryx-brain/src/bodymapRegions.js`
- `ryx-brain/src/bodymap.js`
- `RYX_Wedge_Knowledge_Bases_v1/index.json`
- `ryx-brain/src/knowledge/wedgeRouter.js`
- `ryx-brain/src/knowledge/wedgeFormat.js`
- `ryx-brain/src/knowledge/README.md`
- `ryx-brain/src/labInsights.js`
- `ryx-brain/COVERAGE.md`

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
