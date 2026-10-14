---
id: "ryx.fitness.powerlifting.v1"
title: "Powerlifting"
type: "knowledge"
status: "active"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "RYX_Wedge_Knowledge_Bases_v1/fitness/powerlifting.json"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
kb_id: "ryx.fitness.powerlifting.v1"
knowledge_verified_through: "2026-07-28"
canonical: true
decision_ids:
  - "H04"
  - "H11"
  - "H12"
---

# Powerlifting

## Canonical interpretation and retained source

Canonical rule: [[Knowledge_System#Provenance and evidence]]; [[Knowledge_System#Future retrieval contract]]. Apply [[Brain_Architecture#Global instruction precedence]], [[Data_Boundary#Data truth precedence]], [[Pain_and_Injury#Active pain and clearance]] and [[Athlete_Profile#Confirmed equipment]] before using this lower-priority knowledge. Complete source payloads below remain unchanged; they do not create user facts or override safety/access/tier constraints.

# Powerlifting

## How to read this knowledge

Strength sport contested in the squat, bench press, and deadlift, usually ranked by total and federation formula.

Start with Scope, Quality Rules For Ryx and Safety And Escalation; then read the programming, nutrition, recovery and niche sections that fit the request. This migration retains the whole source, including material the current SESSION formatter omits/truncates. Original kb_id, claim_id, source_ids, evidence_strength, dates and safety caveats are preserved. The source's verification date has not been advanced and its scientific/rules claims have not been independently revalidated.

[[Knowledge_System]] explains selection and limits. [[Safety]] remains highest priority.

## Kb Metadata

- **kb_id**: ryx.fitness.powerlifting.v1
- **title**: RYX Powerlifting Wedge Knowledge Base
- **category**: Fitness
- **niche**: Powerlifting
- **version**: 1.0.0
- **language**: en
- **created_at**: 2026-07-28
- **knowledge_cutoff_verified**: 2026-07-28
- **intended_use**:
  - retrieval_augmented_generation
  - coach_copilot
  - athlete_education
  - program_design_support
- **not_intended_use**:
  - medical_diagnosis
  - emergency_care
  - replacement_for_qualified_coach_or_clinician
- **coverage_contract**: High-coverage foundation, not a claim of literally exhaustive knowledge. Time-sensitive rules and evidence must be revalidated.
- **refresh_policy**:
  - **rules**: before_each_competition_season
  - **research**: quarterly
  - **urgent_safety_updates**: immediately

## Scope

- **definition**: Strength sport contested in the squat, bench press, and deadlift, usually ranked by total and federation formula.
- **included**:
  - (empty array)
- **excluded_or_separate**:
  - (empty array)

## Retrieval Taxonomy

- **intents**:
  - learn
  - assess
  - plan
  - modify_plan
  - technique_help
  - competition_prep
  - nutrition
  - recovery
  - injury_risk
  - return_to_sport
  - rules
- **athlete_levels**:
  - novice
  - beginner
  - intermediate
  - advanced
  - elite
- **life_stages**:
  - youth
  - adult
  - masters
  - pregnant_or_postpartum
- **contexts**:
  - general_health
  - recreation
  - performance
  - competition
  - rehabilitation_adjacent

## Minimum User Profile

- age
- sex_if_relevant_to_health_or_performance
- training_age
- goals
- schedule
- equipment_and_facilities
- current_performance
- injury_and_medical_history
- medications_or_contraindications
- sleep
- nutrition_context
- competition_date_and_ruleset

## Universal Principles

- Item 1:
  - **claim_id**: specificity
  - **statement**: Adaptation is specific to the movement, muscle action, range of motion, velocity, energy system, and skill practiced.
  - **evidence_strength**: high
  - **applies_to**: healthy_adults
  - **last_verified**: 2026-07-28
  - **source_ids**:
    - ACSM_RT_2026
- Item 2:
  - **claim_id**: progressive_overload
  - **statement**: Progress training stress gradually by manipulating load, repetitions, sets, range, density, complexity, frequency, or velocity while preserving technique.
  - **evidence_strength**: high
  - **applies_to**: healthy_adults
  - **last_verified**: 2026-07-28
  - **source_ids**:
    - ACSM_RT_2026
- Item 3:
  - **claim_id**: individualization
  - **statement**: Use response trends rather than a single session: performance, symptoms, readiness, adherence, and enjoyment determine progression.
  - **evidence_strength**: high
  - **applies_to**: healthy_adults
  - **last_verified**: 2026-07-28
  - **source_ids**:
    - ACSM_RT_2026
- Item 4:
  - **claim_id**: fatigue_management
  - **statement**: Distribute hard sessions, manage monotony and spikes, and reduce load when performance and recovery markers deteriorate together.
  - **evidence_strength**: moderate
  - **applies_to**: healthy_adults
  - **last_verified**: 2026-07-28
  - **source_ids**:
    - (empty array)
- Item 5:
  - **claim_id**: skill_before_fatigue
  - **statement**: Teach high-skill or high-velocity work while fresh; fatigue should not be used to normalize unsafe technique.
  - **evidence_strength**: high
  - **applies_to**: healthy_adults
  - **last_verified**: 2026-07-28
  - **source_ids**:
    - (empty array)

## Assessment Framework

- **preparticipation**:
  - goal_and_history_interview
  - medical_red_flags
  - pain_and_injury_screen
  - baseline_skill
  - baseline_capacity
  - constraints
- **monitoring**:
  - session_RPE_x_minutes
  - performance_trend
  - pain_0_to_10
  - sleep_duration_and_quality
  - motivation
  - competition_or_match_load
- **reassessment**: Use the smallest valid test battery every 4-8 weeks or at phase transitions; do not test maximally when fatigue, pain, illness, or unfamiliarity invalidates results.

## Programming Engine

- **workflow**:
  - classify_goal_and_deadline
  - identify_limiting_factors
  - select_minimum_effective_dose
  - place_high_priority_work_first
  - set_progression_and_regression_rules
  - schedule_recovery
  - monitor_response
  - change_one_major_variable_at_a_time
- **autoregulatory_rules**:
  - Item 1:
    - **if**: pain_is_sharp_increasing_or_changes_mechanics
    - **then**: stop_or_regress_and_screen; do_not_push_through
  - Item 2:
    - **if**: target_RIR_missed_by_2_or_more_for_two_sessions
    - **then**: reduce_load_or_volume_and_check_recovery
  - Item 3:
    - **if**: all_work_sets_exceed_top_of_rep_range_with_target_RIR
    - **then**: increase_load_or_difficulty_by_smallest_practical_step
  - Item 4:
    - **if**: illness_fever_chest_symptoms_or_systemic_malaise
    - **then**: do_not_train_hard; seek medical guidance when indicated

## Nutrition And Hydration

- **principles**:
  - Item 1:
    - **claim_id**: energy_availability
    - **statement**: Adequate energy availability supports adaptation, endocrine and bone health, immunity, and performance; screen for REDs risk when restriction, menstrual disturbance, recurrent injury, or performance decline appears.
    - **evidence_strength**: high
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-07-28
    - **source_ids**:
      - IOC_REDS_2023
  - Item 2:
    - **claim_id**: protein
    - **statement**: For most exercising adults, about 1.4-2.0 g/kg/day protein is sufficient; higher intakes may help preserve lean mass during energy restriction.
    - **evidence_strength**: high
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-07-28
    - **source_ids**:
      - ISSN_PROTEIN_2017
  - Item 3:
    - **claim_id**: carbohydrate
    - **statement**: Scale carbohydrate to training volume and intensity; higher-intensity and longer-duration work generally requires more carbohydrate.
    - **evidence_strength**: high
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-07-28
    - **source_ids**:
      - (empty array)
  - Item 4:
    - **claim_id**: hydration
    - **statement**: Begin adequately hydrated and individualize fluid and sodium using environment, sweat rate, session duration, and tolerance; avoid both excessive dehydration and forced overdrinking.
    - **evidence_strength**: high
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-07-28
    - **source_ids**:
      - (empty array)
  - Item 5:
    - **claim_id**: supplements
    - **statement**: Food, training, and sleep come first. Evidence is strongest for context-appropriate use of creatine, caffeine, beta-alanine, nitrate, and protein; screen health, dose, side effects, and anti-doping contamination.
    - **evidence_strength**: moderate
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-07-28
    - **source_ids**:
      - SUPPLEMENTS_2024
      - ISSN_CREATINE_2017
- **anti_doping**: Use only products permitted by the applicable rules and prefer independently batch-tested supplements; RYX must never guarantee a supplement is contamination-free.

## Recovery

- **sleep**: Target a consistent schedule and usually 7-9 hours for adults, often more for youth or high training loads; individual need varies.
- **active_recovery**: Low-intensity activity may improve perceived recovery but does not replace sleep, nutrition, or load management.
- **deload**: Use a planned or responsive reduction in volume and/or intensity when accumulated fatigue masks fitness or before priority competition.

## Safety And Escalation

- **emergency**:
  - chest_pain
  - fainting
  - severe_breathlessness
  - signs_of_heat_stroke
  - suspected_spinal_injury
  - severe_allergic_reaction
  - stroke_signs
- **urgent_clinical_review**:
  - suspected_concussion
  - inability_to_bear_weight
  - visible_deformity
  - rapid_swelling
  - neurological_symptoms
  - dark_urine_after_extreme_exertion
  - persistent_night_pain
- **coaching_boundary**: RYX may educate and adjust general training, but must not diagnose injury, clear return to sport, prescribe medication, or override a clinician.
- **concussion_rule**: Remove from play immediately when concussion is suspected; no same-day return; use qualified medical assessment and a graduated return process.

## Quality Rules For Ryx

- Ask only questions that materially change the recommendation.
- State assumptions and confidence when data are missing.
- Separate rule, consensus, common practice, and emerging evidence.
- Never present correlation, tradition, or elite practice as proof of causation.
- Provide regressions, progressions, and stop criteria with exercise advice.
- Use metric units and optionally show imperial equivalents.
- For minors, pregnancy, chronic disease, eating-disorder risk, or post-injury return, apply stricter escalation.

## Sources

- Item 1:
  - **id**: ACSM_RT_2026
  - **title**: ACSM Position Stand: Resistance Training Prescription for Muscle Function, Hypertrophy, and Physical Performance
  - **year**: 2026
  - **url**: https://pubmed.ncbi.nlm.nih.gov/41843416/
  - **type**: consensus_position_stand
  - **note**: 
- Item 2:
  - **id**: IOC_REDS_2023
  - **title**: IOC consensus statement on Relative Energy Deficiency in Sport
  - **year**: 2023
  - **url**: https://bjsm.bmj.com/content/57/17/1073
  - **type**: consensus_statement
  - **note**: 
- Item 3:
  - **id**: IOC_CONCUSSION_2023
  - **title**: Consensus statement on concussion in sport: Amsterdam 2022
  - **year**: 2023
  - **url**: https://pubmed.ncbi.nlm.nih.gov/37316210/
  - **type**: consensus_statement
  - **note**: 
- Item 4:
  - **id**: ISSN_PROTEIN_2017
  - **title**: ISSN position stand: protein and exercise
  - **year**: 2017
  - **url**: https://pubmed.ncbi.nlm.nih.gov/28642676/
  - **type**: position_stand
  - **note**: 
- Item 5:
  - **id**: ISSN_CREATINE_2017
  - **title**: ISSN position stand: creatine supplementation
  - **year**: 2017
  - **url**: https://pubmed.ncbi.nlm.nih.gov/28615996/
  - **type**: position_stand
  - **note**: 
- Item 6:
  - **id**: SUPPLEMENTS_2024
  - **title**: The Top 5 Can't-Miss Sport Supplements
  - **year**: 2024
  - **url**: https://pubmed.ncbi.nlm.nih.gov/39408214/
  - **type**: peer_reviewed_review
  - **note**: 
- Item 7:
  - **id**: IPF_RULES_2026
  - **title**: IPF Technical Rulebook effective 1 March 2026
  - **year**: 2026
  - **url**: https://www.powerlifting.sport/fileadmin/ipf/data/rules/technical-rules/english/2026_IPF_Technical_Rulebook__effective_01_March_2026__v3.pdf
  - **type**: official_rules
  - **note**: 
- Item 8:
  - **id**: PL_SCOPING_2025
  - **title**: The Applied Sport Science and Medicine of Powerlifting
  - **year**: 2025
  - **url**: https://pubmed.ncbi.nlm.nih.gov/40924269/
  - **type**: peer_reviewed_scoping_review
  - **note**: 
- Item 9:
  - **id**: PL_PELVIC_2025
  - **title**: Powerlifting/weightlifting and female pelvic floor dysfunction
  - **year**: 2025
  - **url**: https://pubmed.ncbi.nlm.nih.gov/39918585/
  - **type**: systematic_review
  - **note**: 

## Exercise Science

- **dose_dimensions**:
  - weekly_hard_sets
  - load_or_difficulty
  - repetitions
  - RIR_or_RPE
  - frequency
  - range_of_motion
  - tempo
  - rest
  - exercise_order
- **hypertrophy**:
  - Item 1:
    - **claim_id**: hyper_effort
    - **statement**: Hypertrophy can occur across a broad load range when sets are sufficiently challenging; very light loads may require closer proximity to failure.
    - **evidence_strength**: high
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-07-28
    - **source_ids**:
      - ACSM_RT_2026
  - Item 2:
    - **claim_id**: hyper_volume
    - **statement**: More weekly sets generally produce more hypertrophy up to diminishing returns; start conservatively and add only when recovery and performance support it.
    - **evidence_strength**: high
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-07-28
    - **source_ids**:
      - ACSM_RT_2026
  - Item 3:
    - **claim_id**: hyper_failure
    - **statement**: Training to momentary failure is not required for most sets; usually retain about 1-3 repetitions in reserve and use failure selectively.
    - **evidence_strength**: high
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-07-28
    - **source_ids**:
      - ACSM_RT_2026
  - Item 4:
    - **claim_id**: hyper_rom
    - **statement**: Use controlled, tolerable range of motion, often emphasizing long muscle lengths where appropriate; anatomy and symptoms constrain selection.
    - **evidence_strength**: moderate
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-07-28
    - **source_ids**:
      - ACSM_RT_2026
- **strength**:
  - Item 1:
    - **claim_id**: strength_load
    - **statement**: Heavier loads and practice of the target lift or movement are most specific for maximal strength, supported by submaximal volume.
    - **evidence_strength**: high
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-07-28
    - **source_ids**:
      - ACSM_RT_2026
  - Item 2:
    - **claim_id**: strength_rest
    - **statement**: Longer inter-set rests, commonly 2-5 minutes for demanding compound work, better preserve force and quality than very short rests.
    - **evidence_strength**: high
    - **applies_to**: healthy_adults
    - **last_verified**: 2026-07-28
    - **source_ids**:
      - (empty array)
- **warm_up**:
  - raise_temperature
  - mobilize_only_as_needed
  - movement_rehearsal
  - progressive_specific_sets
  - avoid_fatiguing_prework

## Competition Lifts

- **squat**:
  - **commands**:
    - squat
    - rack
  - **technical_focus**:
    - walkout_and_setup
    - bracing
    - federation_depth
    - bar_path
    - lockout
  - **common_faults**:
    - depth
    - downward_movement
    - missed_commands
    - unlocked_knees
- **bench_press**:
  - **commands**:
    - start
    - press
    - rack
  - **technical_focus**:
    - stable_setup
    - legal_contact_points
    - motionless_pause
    - press_path
    - elbow_lockout
  - **common_faults**:
    - heave_or_sink
    - butt_lift
    - downward_movement
    - missed_commands
- **deadlift**:
  - **commands**:
    - down
  - **technical_focus**:
    - wedge_and_brace
    - bar_close
    - continuous_rise
    - locked_knees_and_hips
  - **common_faults**:
    - hitching_or_supporting_on_thighs
    - downward_movement
    - soft_lockout
    - dropping_bar

## Programming Model

- **specificity_layers**:
  - competition_lift
  - close_variation
  - developmental_variant
  - accessory
- **periods**:
  - general_preparation
  - strength
  - competition_specific
  - taper
  - competition
  - transition
- **intensity_tools**:
  - percentage_1RM
  - RPE
  - RIR
  - velocity_when_valid
- **weekly_frequency**: Commonly 2-4 squat, 3-5 bench, and 1-3 deadlift exposures depending on level, variation, and tolerance; these are ranges, not requirements.
- **peaking**: Increase competition specificity, reduce accessory fatigue, retain some heavy exposure, and taper volume while avoiding unaccustomed maximal work.
- **attempt_selection**:
  - **opener**: high-confidence legal lift, often about 90-93% of realistic max
  - **second**: secure total or position
  - **third**: goal based on second-attempt speed, ranking, and risk

## Equipment And Rules

- **classes_and_equipment**: Use current federation rulebook for age/weight classes, raw/classic/equipped definitions, approved gear, weigh-in, commands, and records.
- **rule_priority**: Federation and meet-specific rules override generic RYX guidance.
- **weight_cut**: Avoid aggressive acute cuts, especially for youth or inexperienced lifters. Refer substantial cuts to qualified sports dietitian/medical staff.

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
{
  "kb_metadata": {
    "kb_id": "ryx.fitness.powerlifting.v1",
    "title": "RYX Powerlifting Wedge Knowledge Base",
    "category": "Fitness",
    "niche": "Powerlifting",
    "version": "1.0.0",
    "language": "en",
    "created_at": "2026-07-28",
    "knowledge_cutoff_verified": "2026-07-28",
    "intended_use": [
      "retrieval_augmented_generation",
      "coach_copilot",
      "athlete_education",
      "program_design_support"
    ],
    "not_intended_use": [
      "medical_diagnosis",
      "emergency_care",
      "replacement_for_qualified_coach_or_clinician"
    ],
    "coverage_contract": "High-coverage foundation, not a claim of literally exhaustive knowledge. Time-sensitive rules and evidence must be revalidated.",
    "refresh_policy": {
      "rules": "before_each_competition_season",
      "research": "quarterly",
      "urgent_safety_updates": "immediately"
    }
  },
  "scope": {
    "definition": "Strength sport contested in the squat, bench press, and deadlift, usually ranked by total and federation formula.",
    "included": [],
    "excluded_or_separate": []
  },
  "retrieval_taxonomy": {
    "intents": [
      "learn",
      "assess",
      "plan",
      "modify_plan",
      "technique_help",
      "competition_prep",
      "nutrition",
      "recovery",
      "injury_risk",
      "return_to_sport",
      "rules"
    ],
    "athlete_levels": [
      "novice",
      "beginner",
      "intermediate",
      "advanced",
      "elite"
    ],
    "life_stages": [
      "youth",
      "adult",
      "masters",
      "pregnant_or_postpartum"
    ],
    "contexts": [
      "general_health",
      "recreation",
      "performance",
      "competition",
      "rehabilitation_adjacent"
    ]
  },
  "minimum_user_profile": [
    "age",
    "sex_if_relevant_to_health_or_performance",
    "training_age",
    "goals",
    "schedule",
    "equipment_and_facilities",
    "current_performance",
    "injury_and_medical_history",
    "medications_or_contraindications",
    "sleep",
    "nutrition_context",
    "competition_date_and_ruleset"
  ],
  "universal_principles": [
    {
      "claim_id": "specificity",
      "statement": "Adaptation is specific to the movement, muscle action, range of motion, velocity, energy system, and skill practiced.",
      "evidence_strength": "high",
      "applies_to": "healthy_adults",
      "last_verified": "2026-07-28",
      "source_ids": [
        "ACSM_RT_2026"
      ]
    },
    {
      "claim_id": "progressive_overload",
      "statement": "Progress training stress gradually by manipulating load, repetitions, sets, range, density, complexity, frequency, or velocity while preserving technique.",
      "evidence_strength": "high",
      "applies_to": "healthy_adults",
      "last_verified": "2026-07-28",
      "source_ids": [
        "ACSM_RT_2026"
      ]
    },
    {
      "claim_id": "individualization",
      "statement": "Use response trends rather than a single session: performance, symptoms, readiness, adherence, and enjoyment determine progression.",
      "evidence_strength": "high",
      "applies_to": "healthy_adults",
      "last_verified": "2026-07-28",
      "source_ids": [
        "ACSM_RT_2026"
      ]
    },
    {
      "claim_id": "fatigue_management",
      "statement": "Distribute hard sessions, manage monotony and spikes, and reduce load when performance and recovery markers deteriorate together.",
      "evidence_strength": "moderate",
      "applies_to": "healthy_adults",
      "last_verified": "2026-07-28",
      "source_ids": []
    },
    {
      "claim_id": "skill_before_fatigue",
      "statement": "Teach high-skill or high-velocity work while fresh; fatigue should not be used to normalize unsafe technique.",
      "evidence_strength": "high",
      "applies_to": "healthy_adults",
      "last_verified": "2026-07-28",
      "source_ids": []
    }
  ],
  "assessment_framework": {
    "preparticipation": [
      "goal_and_history_interview",
      "medical_red_flags",
      "pain_and_injury_screen",
      "baseline_skill",
      "baseline_capacity",
      "constraints"
    ],
    "monitoring": [
      "session_RPE_x_minutes",
      "performance_trend",
      "pain_0_to_10",
      "sleep_duration_and_quality",
      "motivation",
      "competition_or_match_load"
    ],
    "reassessment": "Use the smallest valid test battery every 4-8 weeks or at phase transitions; do not test maximally when fatigue, pain, illness, or unfamiliarity invalidates results."
  },
  "programming_engine": {
    "workflow": [
      "classify_goal_and_deadline",
      "identify_limiting_factors",
      "select_minimum_effective_dose",
      "place_high_priority_work_first",
      "set_progression_and_regression_rules",
      "schedule_recovery",
      "monitor_response",
      "change_one_major_variable_at_a_time"
    ],
    "autoregulatory_rules": [
      {
        "if": "pain_is_sharp_increasing_or_changes_mechanics",
        "then": "stop_or_regress_and_screen; do_not_push_through"
      },
      {
        "if": "target_RIR_missed_by_2_or_more_for_two_sessions",
        "then": "reduce_load_or_volume_and_check_recovery"
      },
      {
        "if": "all_work_sets_exceed_top_of_rep_range_with_target_RIR",
        "then": "increase_load_or_difficulty_by_smallest_practical_step"
      },
      {
        "if": "illness_fever_chest_symptoms_or_systemic_malaise",
        "then": "do_not_train_hard; seek medical guidance when indicated"
      }
    ]
  },
  "nutrition_and_hydration": {
    "principles": [
      {
        "claim_id": "energy_availability",
        "statement": "Adequate energy availability supports adaptation, endocrine and bone health, immunity, and performance; screen for REDs risk when restriction, menstrual disturbance, recurrent injury, or performance decline appears.",
        "evidence_strength": "high",
        "applies_to": "healthy_adults",
        "last_verified": "2026-07-28",
        "source_ids": [
          "IOC_REDS_2023"
        ]
      },
      {
        "claim_id": "protein",
        "statement": "For most exercising adults, about 1.4-2.0 g/kg/day protein is sufficient; higher intakes may help preserve lean mass during energy restriction.",
        "evidence_strength": "high",
        "applies_to": "healthy_adults",
        "last_verified": "2026-07-28",
        "source_ids": [
          "ISSN_PROTEIN_2017"
        ]
      },
      {
        "claim_id": "carbohydrate",
        "statement": "Scale carbohydrate to training volume and intensity; higher-intensity and longer-duration work generally requires more carbohydrate.",
        "evidence_strength": "high",
        "applies_to": "healthy_adults",
        "last_verified": "2026-07-28",
        "source_ids": []
      },
      {
        "claim_id": "hydration",
        "statement": "Begin adequately hydrated and individualize fluid and sodium using environment, sweat rate, session duration, and tolerance; avoid both excessive dehydration and forced overdrinking.",
        "evidence_strength": "high",
        "applies_to": "healthy_adults",
        "last_verified": "2026-07-28",
        "source_ids": []
      },
      {
        "claim_id": "supplements",
        "statement": "Food, training, and sleep come first. Evidence is strongest for context-appropriate use of creatine, caffeine, beta-alanine, nitrate, and protein; screen health, dose, side effects, and anti-doping contamination.",
        "evidence_strength": "moderate",
        "applies_to": "healthy_adults",
        "last_verified": "2026-07-28",
        "source_ids": [
          "SUPPLEMENTS_2024",
          "ISSN_CREATINE_2017"
        ]
      }
    ],
    "anti_doping": "Use only products permitted by the applicable rules and prefer independently batch-tested supplements; RYX must never guarantee a supplement is contamination-free."
  },
  "recovery": {
    "sleep": "Target a consistent schedule and usually 7-9 hours for adults, often more for youth or high training loads; individual need varies.",
    "active_recovery": "Low-intensity activity may improve perceived recovery but does not replace sleep, nutrition, or load management.",
    "deload": "Use a planned or responsive reduction in volume and/or intensity when accumulated fatigue masks fitness or before priority competition."
  },
  "safety_and_escalation": {
    "emergency": [
      "chest_pain",
      "fainting",
      "severe_breathlessness",
      "signs_of_heat_stroke",
      "suspected_spinal_injury",
      "severe_allergic_reaction",
      "stroke_signs"
    ],
    "urgent_clinical_review": [
      "suspected_concussion",
      "inability_to_bear_weight",
      "visible_deformity",
      "rapid_swelling",
      "neurological_symptoms",
      "dark_urine_after_extreme_exertion",
      "persistent_night_pain"
    ],
    "coaching_boundary": "RYX may educate and adjust general training, but must not diagnose injury, clear return to sport, prescribe medication, or override a clinician.",
    "concussion_rule": "Remove from play immediately when concussion is suspected; no same-day return; use qualified medical assessment and a graduated return process."
  },
  "quality_rules_for_ryx": [
    "Ask only questions that materially change the recommendation.",
    "State assumptions and confidence when data are missing.",
    "Separate rule, consensus, common practice, and emerging evidence.",
    "Never present correlation, tradition, or elite practice as proof of causation.",
    "Provide regressions, progressions, and stop criteria with exercise advice.",
    "Use metric units and optionally show imperial equivalents.",
    "For minors, pregnancy, chronic disease, eating-disorder risk, or post-injury return, apply stricter escalation."
  ],
  "sources": [
    {
      "id": "ACSM_RT_2026",
      "title": "ACSM Position Stand: Resistance Training Prescription for Muscle Function, Hypertrophy, and Physical Performance",
      "year": 2026,
      "url": "https://pubmed.ncbi.nlm.nih.gov/41843416/",
      "type": "consensus_position_stand",
      "note": ""
    },
    {
      "id": "IOC_REDS_2023",
      "title": "IOC consensus statement on Relative Energy Deficiency in Sport",
      "year": 2023,
      "url": "https://bjsm.bmj.com/content/57/17/1073",
      "type": "consensus_statement",
      "note": ""
    },
    {
      "id": "IOC_CONCUSSION_2023",
      "title": "Consensus statement on concussion in sport: Amsterdam 2022",
      "year": 2023,
      "url": "https://pubmed.ncbi.nlm.nih.gov/37316210/",
      "type": "consensus_statement",
      "note": ""
    },
    {
      "id": "ISSN_PROTEIN_2017",
      "title": "ISSN position stand: protein and exercise",
      "year": 2017,
      "url": "https://pubmed.ncbi.nlm.nih.gov/28642676/",
      "type": "position_stand",
      "note": ""
    },
    {
      "id": "ISSN_CREATINE_2017",
      "title": "ISSN position stand: creatine supplementation",
      "year": 2017,
      "url": "https://pubmed.ncbi.nlm.nih.gov/28615996/",
      "type": "position_stand",
      "note": ""
    },
    {
      "id": "SUPPLEMENTS_2024",
      "title": "The Top 5 Can't-Miss Sport Supplements",
      "year": 2024,
      "url": "https://pubmed.ncbi.nlm.nih.gov/39408214/",
      "type": "peer_reviewed_review",
      "note": ""
    },
    {
      "id": "IPF_RULES_2026",
      "title": "IPF Technical Rulebook effective 1 March 2026",
      "year": 2026,
      "url": "https://www.powerlifting.sport/fileadmin/ipf/data/rules/technical-rules/english/2026_IPF_Technical_Rulebook__effective_01_March_2026__v3.pdf",
      "type": "official_rules",
      "note": ""
    },
    {
      "id": "PL_SCOPING_2025",
      "title": "The Applied Sport Science and Medicine of Powerlifting",
      "year": 2025,
      "url": "https://pubmed.ncbi.nlm.nih.gov/40924269/",
      "type": "peer_reviewed_scoping_review",
      "note": ""
    },
    {
      "id": "PL_PELVIC_2025",
      "title": "Powerlifting/weightlifting and female pelvic floor dysfunction",
      "year": 2025,
      "url": "https://pubmed.ncbi.nlm.nih.gov/39918585/",
      "type": "systematic_review",
      "note": ""
    }
  ],
  "exercise_science": {
    "dose_dimensions": [
      "weekly_hard_sets",
      "load_or_difficulty",
      "repetitions",
      "RIR_or_RPE",
      "frequency",
      "range_of_motion",
      "tempo",
      "rest",
      "exercise_order"
    ],
    "hypertrophy": [
      {
        "claim_id": "hyper_effort",
        "statement": "Hypertrophy can occur across a broad load range when sets are sufficiently challenging; very light loads may require closer proximity to failure.",
        "evidence_strength": "high",
        "applies_to": "healthy_adults",
        "last_verified": "2026-07-28",
        "source_ids": [
          "ACSM_RT_2026"
        ]
      },
      {
        "claim_id": "hyper_volume",
        "statement": "More weekly sets generally produce more hypertrophy up to diminishing returns; start conservatively and add only when recovery and performance support it.",
        "evidence_strength": "high",
        "applies_to": "healthy_adults",
        "last_verified": "2026-07-28",
        "source_ids": [
          "ACSM_RT_2026"
        ]
      },
      {
        "claim_id": "hyper_failure",
        "statement": "Training to momentary failure is not required for most sets; usually retain about 1-3 repetitions in reserve and use failure selectively.",
        "evidence_strength": "high",
        "applies_to": "healthy_adults",
        "last_verified": "2026-07-28",
        "source_ids": [
          "ACSM_RT_2026"
        ]
      },
      {
        "claim_id": "hyper_rom",
        "statement": "Use controlled, tolerable range of motion, often emphasizing long muscle lengths where appropriate; anatomy and symptoms constrain selection.",
        "evidence_strength": "moderate",
        "applies_to": "healthy_adults",
        "last_verified": "2026-07-28",
        "source_ids": [
          "ACSM_RT_2026"
        ]
      }
    ],
    "strength": [
      {
        "claim_id": "strength_load",
        "statement": "Heavier loads and practice of the target lift or movement are most specific for maximal strength, supported by submaximal volume.",
        "evidence_strength": "high",
        "applies_to": "healthy_adults",
        "last_verified": "2026-07-28",
        "source_ids": [
          "ACSM_RT_2026"
        ]
      },
      {
        "claim_id": "strength_rest",
        "statement": "Longer inter-set rests, commonly 2-5 minutes for demanding compound work, better preserve force and quality than very short rests.",
        "evidence_strength": "high",
        "applies_to": "healthy_adults",
        "last_verified": "2026-07-28",
        "source_ids": []
      }
    ],
    "warm_up": [
      "raise_temperature",
      "mobilize_only_as_needed",
      "movement_rehearsal",
      "progressive_specific_sets",
      "avoid_fatiguing_prework"
    ]
  },
  "competition_lifts": {
    "squat": {
      "commands": [
        "squat",
        "rack"
      ],
      "technical_focus": [
        "walkout_and_setup",
        "bracing",
        "federation_depth",
        "bar_path",
        "lockout"
      ],
      "common_faults": [
        "depth",
        "downward_movement",
        "missed_commands",
        "unlocked_knees"
      ]
    },
    "bench_press": {
      "commands": [
        "start",
        "press",
        "rack"
      ],
      "technical_focus": [
        "stable_setup",
        "legal_contact_points",
        "motionless_pause",
        "press_path",
        "elbow_lockout"
      ],
      "common_faults": [
        "heave_or_sink",
        "butt_lift",
        "downward_movement",
        "missed_commands"
      ]
    },
    "deadlift": {
      "commands": [
        "down"
      ],
      "technical_focus": [
        "wedge_and_brace",
        "bar_close",
        "continuous_rise",
        "locked_knees_and_hips"
      ],
      "common_faults": [
        "hitching_or_supporting_on_thighs",
        "downward_movement",
        "soft_lockout",
        "dropping_bar"
      ]
    }
  },
  "programming_model": {
    "specificity_layers": [
      "competition_lift",
      "close_variation",
      "developmental_variant",
      "accessory"
    ],
    "periods": [
      "general_preparation",
      "strength",
      "competition_specific",
      "taper",
      "competition",
      "transition"
    ],
    "intensity_tools": [
      "percentage_1RM",
      "RPE",
      "RIR",
      "velocity_when_valid"
    ],
    "weekly_frequency": "Commonly 2-4 squat, 3-5 bench, and 1-3 deadlift exposures depending on level, variation, and tolerance; these are ranges, not requirements.",
    "peaking": "Increase competition specificity, reduce accessory fatigue, retain some heavy exposure, and taper volume while avoiding unaccustomed maximal work.",
    "attempt_selection": {
      "opener": "high-confidence legal lift, often about 90-93% of realistic max",
      "second": "secure total or position",
      "third": "goal based on second-attempt speed, ranking, and risk"
    }
  },
  "equipment_and_rules": {
    "classes_and_equipment": "Use current federation rulebook for age/weight classes, raw/classic/equipped definitions, approved gear, weigh-in, commands, and records.",
    "rule_priority": "Federation and meet-specific rules override generic RYX guidance.",
    "weight_cut": "Avoid aggressive acute cuts, especially for youth or inexperienced lifters. Refer substantial cuts to qualified sports dietitian/medical staff."
  }
}
```

## Release and runtime boundary

Canonical intended rule for the v0.2.0 candidate. Production runtime is not yet aligned with all approved decisions. Historical implementation and the original note text are preserved in [[MIGRATION_REVIEW]] and [[RYX_Brain_v0.1.0_Notes_Snapshot]].

## Source reference

- `RYX_Wedge_Knowledge_Bases_v1/fitness/powerlifting.json` — Complete file (517 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
