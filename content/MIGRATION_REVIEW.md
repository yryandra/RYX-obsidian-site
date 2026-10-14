# Migration Review

Reviewed: 2026-10-13. Faithful extraction only; no production code, API behavior, database, frontend, prompt wording, credit logic or runtime integration changed.

## Sources inspected

109 explicitly selected nonsecret source files were read or structurally inspected. Prompts, runtime/guard/funnel/context, domain stores/formatters, knowledge selection/data, access/approval/messaging and eval contracts received behavior review. Lab presentation/diagnostics were inspected for relevant symbols/call sites, not copied wholesale. Security/data exclusions were applied before source selection. The persona planning documents were inspected only for their proposed/not-run status; their persona records were not promoted into brain instructions.

- RYX_Wedge_Knowledge_Bases_v1/fitness/bodybuilding.json
- RYX_Wedge_Knowledge_Bases_v1/fitness/calisthenics.json
- RYX_Wedge_Knowledge_Bases_v1/fitness/crossfit.json
- RYX_Wedge_Knowledge_Bases_v1/fitness/general.json
- RYX_Wedge_Knowledge_Bases_v1/fitness/powerlifting.json
- RYX_Wedge_Knowledge_Bases_v1/index.json
- RYX_Wedge_Knowledge_Bases_v1/ryx-wedge-kb.schema.json
- RYX_Wedge_Knowledge_Bases_v1/sports/basketball.json
- RYX_Wedge_Knowledge_Bases_v1/sports/combat.json
- RYX_Wedge_Knowledge_Bases_v1/sports/football.json
- RYX_Wedge_Knowledge_Bases_v1/sports/golf.json
- RYX_Wedge_Knowledge_Bases_v1/sports/padel.json
- RYX_Wedge_Knowledge_Bases_v1/sports/swimming.json
- RYX_Wedge_Knowledge_Bases_v1/sports/tennis.json
- RYX_Wedge_Knowledge_Bases_v1/wellness/rehab.json
- RYX_Wedge_Knowledge_Bases_v1/wellness/yoga.json
- docs/product/ryx-athlete-persona-plan.md
- docs/product/ryx-persona-plan.md
- package.json
- ryx-brain/COVERAGE.md
- ryx-brain/README.md
- ryx-brain/docs/accounts.md
- ryx-brain/docs/backlog.md
- ryx-brain/docs/body-map.md
- ryx-brain/docs/checkins.md
- ryx-brain/docs/envelope-upsell.md
- ryx-brain/docs/event-countdown.md
- ryx-brain/docs/program-marketplace.md
- ryx-brain/docs/reports.md
- ryx-brain/docs/sessions.md
- ryx-brain/docs/shared-athlete-data.md
- ryx-brain/docs/todos.md
- ryx-brain/docs/train-live.md
- ryx-brain/package.json
- ryx-brain/src/accounts.js
- ryx-brain/src/athleteSnapshot.js
- ryx-brain/src/bodymap.js
- ryx-brain/src/bodymapFormat.js
- ryx-brain/src/bodymapRegions.js
- ryx-brain/src/buildSystemPrompt.js
- ryx-brain/src/cardCoerce.js
- ryx-brain/src/cardLayout.js
- ryx-brain/src/chatIntake.js
- ryx-brain/src/checkinFormat.js
- ryx-brain/src/checkins.js
- ryx-brain/src/client.js
- ryx-brain/src/coryxProducts.js
- ryx-brain/src/credits.js
- ryx-brain/src/directMessages.js
- ryx-brain/src/envelope.js
- ryx-brain/src/eval.js
- ryx-brain/src/evalExerciseMedia.js
- ryx-brain/src/evalExerciseMediaNiches.js
- ryx-brain/src/evalOpenai.js
- ryx-brain/src/eventFormat.js
- ryx-brain/src/events.js
- ryx-brain/src/exerciseMedia.js
- ryx-brain/src/formatCoachReply.js
- ryx-brain/src/herd.js
- ryx-brain/src/identity.js
- ryx-brain/src/identityRoutes.js
- ryx-brain/src/knowledge/README.md
- ryx-brain/src/knowledge/data/exerciseMediaCatalog.json
- ryx-brain/src/knowledge/data/exercises.json
- ryx-brain/src/knowledge/data/formDemosByWedge.json
- ryx-brain/src/knowledge/data/playbooks.json
- ryx-brain/src/knowledge/formDemos.js
- ryx-brain/src/knowledge/nicheMap.js
- ryx-brain/src/knowledge/retrieve.js
- ryx-brain/src/knowledge/wedgeFormat.js
- ryx-brain/src/knowledge/wedgeLoader.js
- ryx-brain/src/knowledge/wedgeRouter.js
- ryx-brain/src/labEval.js
- ryx-brain/src/labInsights.js
- ryx-brain/src/labMemory.js
- ryx-brain/src/labPersonality.js
- ryx-brain/src/labScenarios.js
- ryx-brain/src/labSessions.js
- ryx-brain/src/liveEvents.js
- ryx-brain/src/llmProvider.js
- ryx-brain/src/openaiClient.js
- ryx-brain/src/openaiRun.js
- ryx-brain/src/printPrompt.js
- ryx-brain/src/profileFunnel.js
- ryx-brain/src/programCatalog.js
- ryx-brain/src/programFormat.js
- ryx-brain/src/programs.js
- ryx-brain/src/prompts/athlete.js
- ryx-brain/src/prompts/core.js
- ryx-brain/src/prompts/trainer.js
- ryx-brain/src/replyGuards.js
- ryx-brain/src/reports.js
- ryx-brain/src/runChat.js
- ryx-brain/src/scenarios/athlete.json
- ryx-brain/src/scenarios/trainer.json
- ryx-brain/src/server.js
- ryx-brain/src/sessionFormat.js
- ryx-brain/src/sessions.js
- ryx-brain/src/todoFormat.js
- ryx-brain/src/todos.js
- ryx-brain/test/messaging.test.js
- ryx-brain/test/shared-ryx.test.js
- ryx-landing/src/App.jsx
- ryx-landing/src/components/cards/RyxContentCard.jsx
- ryx-landing/src/lib/cardLayout.js
- ryx-landing/src/lib/identityApi.js
- scripts/dev.mjs
- web/src/lib/brainHealth.js
- web/src/pages/CoachPage.jsx

## Additional repository discovery

The repository also contains RYX_Business_Model_and_Credit_Economics.pdf, RYX_User_Scenarios_and_UI_UX.pdf, RYX QA Framework.xlsx, and the Athlete Assistant SoW/User Scenerios DOCX files. These were inventoried by filename only, not content-audited or migrated. They are supplemental historical requirements/QA artifacts rather than files loaded by the inspected runtime. Their referenced implemented behavior is audited from credits/prompts/scenarios/coverage and current code; no unseen artifact wording is treated as authoritative. A future historical-requirements reconciliation can review them separately. Visual assets and design-system component prompts are presentation resources and were not promoted into coaching knowledge.

## Brain content migrated

113 notes with YAML properties: 106 active production/manifest notes and 7 reference notes. Types: core 5, role 10, policy 10, domain 12, knowledge 24, tool 31, workflow 11, eval 5, runtime-context 4, release 1. Navigation/audit guides are additional Markdown files.

All original CORE and Athlete/Trainer role/tier instruction blocks are retained verbatim. All 14 wedge JSON payloads survive losslessly with readable projections, along with 18 movement entries, 113 media entries, manifests/index/schema, ordered routing/media match rules and static program template content. All 50 Athlete and 47 Trainer acceptance scenarios are retained without profile objects or HERD fixture values. Media scenario definitions and full coverage text are retained. Reference-only legacy playbooks are clearly excluded from the release.

## Runtime implementation deliberately left in code

JavaScript prompt/string assembly, provider clients and selection, classification and credit calculations, envelope serialization/normalization, regex detection, deterministic guards/intake/coercion/media attachment, identity/authorization, SQLite/JSON persistence, SSE delivery, route handlers, program validation/version writes, frontend gating/rendering, tests and eval runners remain implementation. Behavior/contracts are represented here, but Markdown does not replace enforcement. No application module was imported/executed for generation except isolated evaluation of vetted static literals/pure definitions; no database loaders, auth sessions, providers or secret resolvers ran.

## Duplicate instructions

8 repeated rule families found. They were retained as source evidence and linked task-oriented projections; no canonical precedence was invented and no original module was deleted.

### D01

Voice, warmth and concise next steps repeat in core, both role workflows and response directive.

### D02

Research sentence and no-diagnosis/pain caution repeat in core, trainer judgment/workflows, SESSION hints, wedge boundaries and reply guards.

### D03

Companion trainer ownership/no-send repeat in athlete role/workflow, SESSION, directive, guards and assigned-program context.

### D04

Trainer suggests/approves/no-auto-send/apply repeat in core control, trainer blocks, directive, guards and approval documentation.

### D05

Pro deliver-first behavior repeats in tier blocks, role workflows, SESSION and response directive.

### D06

Free useful-basic-value plus one upgrade line repeats in tier blocks, workflows, SESSION and directive.

### D07

Niche knowledge precedence/evidence caveats repeat in builder, envelope directive, wedge formatter and KB quality rules.

### D08

Known facts, fresh data precedence, no invented records and app-confirmed actions repeat in core, role workflows, snapshot/formatters and shared-data docs.

## Conflicting instructions

22 behavior/documentation discrepancies are recorded below. “Executed” means identified from source and, for selected pure stages, offline audit probes; it does not claim a live model run. Both source intent and actual conditions are preserved without changing either.

### C01 — Pro delivery versus incomplete-intake gate

Pro prompts say deliver concrete output first when context exists; the production athlete intake gate strips weekly_plan/major_adjustment/advanced_multistep cards on incomplete profiles without a tier exemption. The post-model executed gate can defeat the prompt contract.

Sources: `ryx-brain/src/prompts/athlete.js`, `ryx-brain/src/prompts/trainer.js`, `ryx-brain/src/envelope.js`, `ryx-brain/src/profileFunnel.js`, `ryx-brain/src/server.js`.

### C02 — Crisis safety versus later intake processing

The crisis guard removes questions/cards and returns quick_question. Production still runs intake enforcement and question coercion afterward without a crisis exemption; an incomplete profile can receive an intake question again. The inspected pipeline does not rerun guards at the end.

Sources: `ryx-brain/src/prompts/core.js`, `ryx-brain/src/replyGuards.js`, `ryx-brain/src/profileFunnel.js`, `ryx-brain/src/server.js`.

### C03 — Crisis prompt versus keyword guard acceptance

Prompt requires no fitness/questions, care/urgency and 2–4 sentences, with broad crisis/hopelessness recognition. Guard triggers on a narrower phrase set and accepts any existing lead containing emergency/999/911/crisis/helpline/suicide, without checking fitness framing, sentence count or coaching questions.

Sources: `ryx-brain/src/prompts/core.js`, `ryx-brain/src/replyGuards.js`.

### C04 — Exact research sentence/order/referral versus prefix guard

Prompt requires the full verbatim sentence before any treatment-style suggestion. Guard checks only a prefix across lead/card note, appends the sentence after existing content, and adds a physiotherapist referral only if that prefix is absent. A partial prefix or existing card-note prefix may bypass lead/referral/order requirements. Eval hard gates also check the prefix.

Sources: `ryx-brain/src/prompts/core.js`, `ryx-brain/src/prompts/trainer.js`, `ryx-brain/src/replyGuards.js`, `ryx-brain/src/eval.js`, `ryx-brain/src/evalOpenai.js`.

### C05 — Active-pain clearance versus body-map modification advice

Core prohibits exercise modifications before professional clearance when pain is active. Body-map SESSION instructs modifications/avoidance for flagged regions and swaps/mobility for severe regions without a separate clearance condition. Keep both sources visible; safety is explicitly highest priority in the prompt but the lower block still exists.

Sources: `ryx-brain/src/prompts/core.js`, `ryx-brain/src/bodymapFormat.js`.

### C06 — Unknown-mode Companion prompt versus renderer/guard parameter

Athlete prompt treats a mentioned existing coach with unknown mode as Companion. Renderer uses Solo for any mode other than companion, guards depend on explicit mode, and production forces Companion only for an assigned program. The live frontend also sends mode solo. A relationship or trainer mention alone is not the same executed mode signal.

Sources: `ryx-brain/src/prompts/athlete.js`, `ryx-brain/src/buildSystemPrompt.js`, `ryx-brain/src/server.js`, `ryx-brain/src/replyGuards.js`, `ryx-landing/src/App.jsx`.

### C07 — Companion drafting format and conditional override protection

Role requests quoted draft text starting Draft message:. Guard wraps tell/message-my-trainer replies under another label and has a fixed leg-day draft for recognized change requests. If lead already contains draft message to your trainer, the change branch leaves any existing card/question intact. Trigger vocabulary is narrower than the role rule.

Sources: `ryx-brain/src/prompts/athlete.js`, `ryx-brain/src/replyGuards.js`.

### C08 — Free useful reflection versus feature/depth restrictions

Athlete workflows allow a basic plateau explanation while ATHLETE_FREE gates plateau analysis; trainer Free summary/message contracts coexist with the output directive requiring full matching formats. UI locks later analysis/meal sections, including hydration, observations and suggested actions. These overlapping depth distinctions remain unresolved, not expanded by migration.

Sources: `ryx-brain/src/prompts/athlete.js`, `ryx-brain/src/prompts/trainer.js`, `ryx-brain/src/envelope.js`, `ryx-landing/src/lib/cardLayout.js`.

### C09 — Free advanced-section previews versus basic-only cards

SESSION tells Free athlete cards to include Warm-up/Main and advanced Finisher/Cool-down/Form cues/Progression/Recovery sections for UI locks. RESPONSE_DIRECTIVE says Free cards should remain basic. Actual app gating changes visibility, not the received payload.

Sources: `ryx-brain/src/buildSystemPrompt.js`, `ryx-brain/src/envelope.js`, `ryx-brain/src/prompts/athlete.js`.

### C10 — Mandatory safety card note versus Free note locking

The output directive uses card.note for the mandatory research statement. Free workout/program/meal/analysis note footers are locked in the app. Guards may add it to lead, but an existing prefix in card.note suppresses that addition. The required statement can remain in a locked note.

Sources: `ryx-brain/src/prompts/core.js`, `ryx-brain/src/envelope.js`, `ryx-landing/src/lib/cardLayout.js`, `ryx-landing/src/components/cards/RyxContentCard.jsx`, `ryx-brain/src/replyGuards.js`.

### C11 — Unlimited-credit upsell example versus actual metering

Directive upsell examples include unlimited credits. Actual Pro account grants 600 per fixed 30-day cycle plus capped 100 rollover and remains action-metered. No entitlement/credit logic was changed.

Sources: `ryx-brain/src/envelope.js`, `ryx-brain/src/accounts.js`, `ryx-brain/src/credits.js`.

### C12 — Older fixture/userId documentation versus authenticated production

Older README/account sections describe fixture-backed HERD context/localStorage user IDs and request userId. Current production uses authenticated role/identity, relationship-checked fresh snapshots and saved profiles, and ignores HERD fixtures. Shared-athlete-data documentation describes the newer implementation; preserve the distinction.

Sources: `ryx-brain/README.md`, `ryx-brain/docs/accounts.md`, `ryx-brain/docs/shared-athlete-data.md`, `ryx-brain/src/server.js`, `ryx-brain/src/identityRoutes.js`, `ryx-brain/src/chatIntake.js`.

### C13 — Report listing/auth and auto-escalation documentation

reports.md labels GET report listing no-auth admin/Lab MVP; current ordinary user sessions are blocked from that diagnostic listing. A user-submitted persisted report exists; trainer prompt/guard still says automatic human escalation is unavailable. No email/webhook or guaranteed human response is implemented.

Sources: `ryx-brain/docs/reports.md`, `ryx-brain/src/identityRoutes.js`, `ryx-brain/src/server.js`, `ryx-brain/src/prompts/trainer.js`.

### C14 — Past active-event selector

Documentation says nearest future or most recent past active event. getActiveEvent sorts ascending and chooses the earliest when all active candidates are past. Current write paths tend to enforce a single active event; the fallback still differs.

Sources: `ryx-brain/docs/event-countdown.md`, `ryx-brain/src/events.js`.

### C15 — No invented context/clearance versus intake heuristics

Executed extraction can infer equipment from sport, schedule from the whole thread including assistant suggestions, noInjuries from sessionStart+schedule, and cleared/monitoring return from the word physio. Scored labels can overwrite specific extracted values. Some inferred fields are not persisted by saveProfile. These may be rendered as established facts despite the prompt prohibition on inventing data; no inference fix applied.

Sources: `ryx-brain/src/prompts/core.js`, `ryx-brain/src/labMemory.js`, `ryx-brain/src/identity.js`.

### C16 — Equipment-only prescriptions versus marketplace bodyweight swaps

Athlete rules use only available equipment. Adapt hook groups home and bodyweight together and replaces gym movements with DB/band alternatives, so a bodyweight-only profile can receive equipment it lacks. This fixed hook remains separate from LLM behavior.

Sources: `ryx-brain/src/prompts/athlete.js`, `ryx-brain/src/programs.js`.

### C17 — Free/Pro memory promise versus current loading/persistence

Pro promises long-term client/style memory and Free recent context only. The same trainer-history query loads at most 24 turns for either tier; no dedicated durable client-note/style preference store is present. Raw snapshot additions also bypass several formatted Free history caps. Actual persistence is documented separately from prompt promises.

Sources: `ryx-brain/src/prompts/trainer.js`, `ryx-brain/src/identity.js`, `ryx-brain/src/athleteSnapshot.js`.

### C18 — Returned action versus final billed cost

Model action sets creditCost after a pre-estimate gate. Crisis guard changes action without recalculating cost; production funnel stripping also changes action without explicit cost update (Lab recalculates). Later card coercion recalculates only on its own action change. Final cost can exceed available prechecked credits; deduction floors at zero. No charging change applied.

Sources: `ryx-brain/src/runChat.js`, `ryx-brain/src/openaiRun.js`, `ryx-brain/src/replyGuards.js`, `ryx-brain/src/profileFunnel.js`, `ryx-brain/src/server.js`, `ryx-brain/src/labSessions.js`, `ryx-brain/src/accounts.js`.

### C19 — Trainer first-contact prompt versus mandatory client selection

Prompt says greet a first-time trainer by name/category/specialization and list capabilities. Production resolveAthlete can return which-client/no-athletes clarification before invoking the model, even for hey/first-contact requests. The general prompt introduction is therefore not always reached.

Sources: `ryx-brain/src/prompts/trainer.js`, `ryx-brain/src/server.js`, `ryx-brain/src/identity.js`.

### C20 — Body-map documentation versus current catalog/schema

Older document lists23 coarse regions and only1–10 input. Code has34 zones, more aliases, feelType and original5/10 reporting scales. The vault domain/catalog follows executed schema and records the stale document explicitly.

Sources: `ryx-brain/docs/body-map.md`, `ryx-brain/src/bodymapRegions.js`, `ryx-brain/src/bodymap.js`, `ryx-brain/src/athleteSnapshot.js`.

### C21 — Intended retrieval contract versus actual projection

Index describes taxonomy filtering, meaningful chunks, claim/source preservation and validation/refresh checks. Current router is substring scoring; formatter drops IDs, omits fields, slices arrays/objects and capscharacters. Knowledge README also shows an older collection path; loader uses repository root. Full KB storage is preserved without assuming the current model receives it all.

Sources: `RYX_Wedge_Knowledge_Bases_v1/index.json`, `ryx-brain/src/knowledge/wedgeRouter.js`, `ryx-brain/src/knowledge/wedgeFormat.js`, `ryx-brain/src/knowledge/README.md`.

### C22 — Evaluation-path descriptions versus executed coverage

Anthropic evaluator bypasses retrieval/envelope/guards/server processing. OpenAI evaluator comments imply Lab+funnel equivalence but it omits actual server/Lab postprocessing; provider selection can follow configuration. Coverage is a documentary matrix, not an up-to-date passing report, and Lab safety metrics permit weaker generic review wording.

Sources: `ryx-brain/src/eval.js`, `ryx-brain/src/evalOpenai.js`, `ryx-brain/src/labInsights.js`, `ryx-brain/COVERAGE.md`, `ryx-brain/src/server.js`.

## Hardcoded behaviour discovered

- Exact research sentence, crisis fallback, Companion leg-day fallback, draft wrappers and support-escalation suffix in replyGuards.
- Latest-message keyword hints in buildSystemPrompt; one-question funnel, five-pillar completeness and closure conditions.
- Stable role/tier defaults, authoritative assigned-program priority and forced Companion.
- Fixed credit weights, Free 30/Pro 600 grants, 100 rollover cap, fixed 30-day refresh and heuristic classification order.
- Free card heading/template/note locks, media catalog order, card fallback and plain-text cleanup.
- Tier formatter caps plus untiered raw snapshot details; 24-turn trainer history and restricted profile save keys.
- Eight marketplace equipment swaps, beginner set/RPE 6 adjustment and missing-week/day fallback; stub payments/purchases.
- Event phase thresholds/date offsets and active-event selection; 34 body zones, aliases and 5/10 scale conversion.
- DM 4000-character limit, idempotency key,100-message paging, explicit read receipt and relationship/auth rechecks.

## Missing / undefined brain areas

- No Markdown compiler/loader, note precedence/deduplication policy, release activation pipeline or Obsidian-to-runtime synchronization is implemented. This migration intentionally stops before integration.
- No explicit model tool dispatcher/function-calling registry; tool notes describe real internal/app contracts only.
- No standalone goals CRUD, durable client-note save, unlimited long-term trainer-style memory, advanced habit/streak engine or multimodal upload analysis in the inspected production path.
- No automatic backend event for chat-requested send/apply/escalate; explicit app DM/program/report operations are distinct.
- Shared target CORYX service/database for CMS/iOS is an architecture decision; this task does not prove those clients are integrated. Current persistence is SQLite plus domain JSON with single-process limitations.
- No payment/creator-payout verification or complete week expansion/automatic marketplace progression; no research-source refresh/schema validator execution in current knowledge loader.
- Safety guard coverage is conditional and narrower than policy; no comprehensive final safety stage after all coercion exists in the inspected server path.
- Persona plans are 176 proposed evaluation hypotheses, not validated personas, production behavior or current test results. Historical eval outputs were not migrated.

## Security exclusions

Excluded without reading credential values: ryx-brain/.openai-key, ryx-brain/.anthropic-key, API Keys/, .env/.env.*, private-key/token/credential files, key resolver source keys.js and authentication secret records. Source code may reference credential mechanisms/field names, but generated notes contain no values. No example/template key file was used as an input. Only generated vault content is scanned for potential secret patterns; excluded credential sources are never opened for comparison.

## Runtime/user-data exclusions

ryx-brain/data/ was neither read nor copied: identity.sqlite and journals, accounts.json, sessions.json, checkins.json, bodymap.json, programs.json, reports.json, todos.json, events.json and any other runtime records remain outside the vault. No athlete fixture/profile object from herd.js, Lab seeds, test setup or scenario.profile/scenario.herd was migrated. Public curated knowledge under src/knowledge/data is intentionally included: its data folder contains knowledge catalogs, not live user stores. Static catalog training templates omit mock creator identity objects. Evaluation user/should/accept prose is retained only as test stimulus, with external-context dependencies marked.

## Items requiring human review

12 grouped review items; nothing was applied as a behavioral change.

- H01: Review precedence between deliver-first prompts and deterministic intake; C01.
- H02: Review the complete crisis pipeline, recognition and final output; C02/C03.
- H03: Review exact research sentence/order/referral enforcement and visibility; C04/C10.
- H04: Review active pain/clearance and inferred safety context; C05/C15.
- H05: Review authoritative Companion mode and drafting behavior; C06/C07.
- H06: Review Free feature/depth boundaries and advanced-section previews; C08/C09.
- H07: Review credit entitlement wording and action/cost consistency; C11/C18.
- H08: Review current authentication/report documentation; C12/C13.
- H09: Review event fallback and body-map schema documentation; C14/C20.
- H10: Review real memory promises, tier limits and trainer greeting selection; C17/C19.
- H11: Review marketplace equipment adaptation and incomplete template weeks; C16 and Programs.
- H12: Review retained knowledge versus runtime retrieval/evaluation coverage before any integration; C21/C22.

## Recommended next steps

### Recommendation — NOT APPLIED

Open [[00_HOME]] and review the original identity, role/tier blocks and disputed findings. Decide the desired behavior for H01–H12 before a separate runtime integration. Agree which notes are authoritative modules versus duplicate topic projections; define a compiler/retrieval contract preserving stable IDs/caveats and live-data boundaries. Bring current HTTP/pipeline tests and exact-language checks into that later release validation, and separately review source freshness. None of these recommendations has changed production.

## Final validation

- [x] No API-key/credential files read or copied; generated content passes secret-pattern checks.
- [x] No live user records, athlete fixture/profile objects, test account objects, SQLite files or runtime JSON databases copied.
- [x] Every active brain note has valid properties, a unique ID, existing audited source_files, source references and migration-map rows.
- [x] All18 original instruction blocks retained verbatim, including identity/personality, Solo/Companion, Trainer approval, Free/Pro and deliver-first language.
- [x] Every deterministic reply-guard branch represented; selected exact fallback/conditional behavior verified offline.
- [x] SESSION and Athlete Snapshot document runtime schemas/interpretation only.
- [x] All14 wedge payloads and curated knowledge catalogs compare losslessly against their originals.
- [x] All50 Athlete and47 Trainer scenario IDs/texts/flags retained with profile/herd values excluded; coverage and media cases retained.
- [x] All Obsidian links resolve without ambiguity.
- [x] Release manifest contains exactly the active production notes; excludes eval/admin/reference/draft/archive material.
- [x] All 109 audited original files retain their SHA-256 baseline; existing source implementation was not edited.

Offline validator: 15 checks passed. 120 Markdown files total, including navigation/audit guides. No live provider evaluations or online video checks were run. The successful validation.json is stored outside the production vault in outputs/ryx-obsidian-migration-2026-10-13/. Source integrity is relative to the audited migration baseline, not Git HEAD; any preexisting repository work is preserved. Secret scanning is pattern-based and complements the input allowlist, not a claim of comparison against excluded secret files.
