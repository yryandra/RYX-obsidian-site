---
id: "ryx.knowledge.exercise_media_rules"
title: "Exercise Media Rules"
type: "knowledge"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/exerciseMedia.js"
  - "ryx-brain/src/cardCoerce.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
decision_ids:
  - "H08"
  - "H12"
---

# Exercise Media Rules

## Reference status

Retained historical/source evidence, excluded from the candidate manifest. It is not an independent canonical instruction or claim of a new passing run. See [[RYX_BRAIN_DECISIONS]] for intended rules and [[Knowledge_System#Future retrieval contract]] / [[Eval_System#Production-quality evaluation contract]] for future integration.

# Exercise Media Rules

Current ordered media matching prioritizes an explicit movement in the latest user message. A specific unmatched “what about/how/show/teach” movement follow-up returns no match rather than an unrelated prior movement; generic basics/play and video-only follow-ups can use context. Video-only requests resolve from prior context first. Candidate text groups are then scanned in catalog order. Entries without a YouTube identifier produce no video.

Media objects carry mediaType youtube, src, title, alt and exerciseId. Multi-exercise workout/plan/meal cards avoid a single unrelated demo. Exercise explanations use exact movement titles and form/regression sections. The lead's claims that video cannot be shown are only removed when valid media is attached.

## Ordered source match rules

Regex source and flags are retained here because catalog order/matcher coverage materially determines which movement is shown; general JavaScript implementation remains in code.

## Dumbbell bench press

- **id**: dumbbell-bench-press
- **title**: Dumbbell bench press
- **match**: \bdumbbell\s+bench[\s-]?press\b|\bdb\s+bench\b
- **flags**: i
- **youtube**: VmB1G1K7v94
- **niches**: undefined

## Bench press

- **id**: bench-press
- **title**: Bench press
- **match**: \b(?:barbell\s+)?bench[\s-]?press\b|\bhow do i bench\b|\bhow to bench\b|\blearn how to bench\b
- **flags**: i
- **youtube**: vthMCtgVtFw
- **niches**: undefined

## Incline push-up

- **id**: incline-push-up
- **title**: Incline push-up
- **match**: \bincline\s+push[\s-]?ups?\b
- **flags**: i
- **youtube**: cfns5VDVVvk
- **niches**: undefined

## Scapular push-up

- **id**: scapular-push-up
- **title**: Scapular push-up
- **match**: \bscapular\s+push[\s-]?ups?\b|\bscap\s+push[\s-]?ups?\b|\bpush[\s-]?up\s+plus\b
- **flags**: i
- **youtube**: LeMk15TN0No
- **niches**: undefined

## Push-up

- **id**: push-up
- **title**: Push-up
- **match**: \b(?!(?:scapular|scap|incline)\s+)push[\s-]?ups?\b
- **flags**: i
- **youtube**: IODxDxX7oi4
- **niches**: undefined

## Goblet squat

- **id**: goblet-squat
- **title**: Goblet squat
- **match**: \bgoblet\s+squats?\b
- **flags**: i
- **youtube**: 0OWbS1WiUGU
- **niches**: undefined

## Front squat

- **id**: front-squat
- **title**: Front squat
- **match**: \bfront\s+squats?\b
- **flags**: i
- **youtube**: 6HDiP65lO8Y
- **niches**: undefined

## Bulgarian split squat

- **id**: bulgarian-split-squat
- **title**: Bulgarian split squat
- **match**: \b(bulgarian\s+)?split\s+squats?\b
- **flags**: i
- **youtube**: 2C-uNgKwPLE
- **niches**: undefined

## Spanish squat

- **id**: spanish-squat
- **title**: Spanish squat
- **match**: \bspanish\s+squats?\b
- **flags**: i
- **youtube**: hgFxm5KIF7M
- **niches**: undefined

## Hip thrust

- **id**: hip-thrust
- **title**: Hip thrust
- **match**: \bhip\s+thrusts?\b
- **flags**: i
- **youtube**: SEdqd1n0cvg
- **niches**: undefined

## Leg press

- **id**: leg-press
- **title**: Leg press
- **match**: \bleg\s+press\b
- **flags**: i
- **youtube**: K5n2vg3oZa4
- **niches**: undefined

## Box step-up

- **id**: box-step-up
- **title**: Box step-up
- **match**: \bbox\s+step[\s-]?ups?\b
- **flags**: i
- **youtube**: WCFCdxzFBa4
- **niches**: undefined

## Squat

- **id**: squat
- **title**: Squat
- **match**: \b(?!(?:front|goblet|bulgarian|split|spanish)\s+)squats?\b
- **flags**: i
- **youtube**: ultWZbUMPL8
- **niches**: undefined

## Romanian deadlift

- **id**: rdl
- **title**: Romanian deadlift
- **match**: \b(romanian\s+deadlifts?|rdl)\b
- **flags**: i
- **youtube**: 5bJEigM5iVg
- **niches**: undefined

## Deadlift

- **id**: deadlift
- **title**: Deadlift
- **match**: \b(barbell\s+)?deadlifts?\b
- **flags**: i
- **youtube**: wYREQkVtvEc
- **niches**: undefined

## Lunge

- **id**: lunge
- **title**: Lunge
- **match**: \b(walking\s+)?lunges?\b
- **flags**: i
- **youtube**: QOVaHwm-Q6U
- **niches**: undefined

## Side plank

- **id**: side-plank
- **title**: Side plank
- **match**: \bside\s+planks?\b
- **flags**: i
- **youtube**: XeN4pEZZJNI
- **niches**: undefined

## Plank

- **id**: plank
- **title**: Plank
- **match**: \b(?!(?:side\s+))planks?\b
- **flags**: i
- **youtube**: ASdvN_XEl_c
- **niches**: undefined

## Pull-up

- **id**: pull-up
- **title**: Pull-up
- **match**: \bpull[\s-]?ups?\b
- **flags**: i
- **youtube**: eGo4IYlbE5g
- **niches**: undefined

## Lat pulldown

- **id**: lat-pulldown
- **title**: Lat pulldown
- **match**: \blat\s+pulldowns?\b
- **flags**: i
- **youtube**: CAwf7n6Luuc
- **niches**: undefined

## Inverted row

- **id**: inverted-row
- **title**: Inverted row
- **match**: \binverted\s+rows?\b|\bbodyweight\s+rows?\b
- **flags**: i
- **youtube**: OYUxXMGVuuU
- **niches**: undefined

## Shoulder press

- **id**: shoulder-press
- **title**: Shoulder press
- **match**: \b(shoulder|overhead)\s+press\b|\bmilitary\s+press\b
- **flags**: i
- **youtube**: B-aVuyhvLHU
- **niches**: undefined

## Row

- **id**: row
- **title**: Row
- **match**: \b(dumbbell\s+rows?|bent[- ]over\s+rows?|how (?:do i|to) row|rows?\s+properly)\b
- **flags**: i
- **youtube**: 6TSP1TRMUzs
- **niches**: undefined

## Dip

- **id**: dip
- **title**: Dip
- **match**: \b(tricep\s+)?dips?\b
- **flags**: i
- **youtube**: c3ZGl4pAwZ4
- **niches**: undefined

## Burpee

- **id**: burpee
- **title**: Burpee
- **match**: \bburpees?\b
- **flags**: i
- **youtube**: wS4OsJ4yzx4
- **niches**: undefined

## Farmer carry

- **id**: farmer-carry
- **title**: Farmer carry
- **match**: \bfarmer\s+(carry|walk)s?\b
- **flags**: i
- **youtube**: 8OtwXwrJizk
- **niches**: undefined

## Dead bug

- **id**: dead-bug
- **title**: Dead bug
- **match**: \bdead[\s-]?bugs?\b
- **flags**: i
- **youtube**: JrcoGEZn6L4
- **niches**: undefined

## Bird dog

- **id**: bird-dog
- **title**: Bird dog
- **match**: \bbird[\s-]?dogs?\b
- **flags**: i
- **youtube**: Jmq2El0u8T0
- **niches**: undefined

## Clamshell

- **id**: clamshell
- **title**: Clamshell
- **match**: \bclamshells?\b
- **flags**: i
- **youtube**: ymjOGuPjOSE
- **niches**: undefined

## Glute bridge

- **id**: glute-bridge
- **title**: Glute bridge
- **match**: \bglute\s+bridges?\b
- **flags**: i
- **youtube**: 8bbE64NuDTU
- **niches**: undefined

## Cat-cow stretch

- **id**: cat-cow
- **title**: Cat-cow stretch
- **match**: \bcat[\s-]?cows?\b|\bcat\s+cow\b
- **flags**: i
- **youtube**: rbuptYr2CGM
- **niches**: undefined

## Band pull-apart

- **id**: band-pull-apart
- **title**: Band pull-apart
- **match**: \bband\s+pull[\s-]?aparts?\b
- **flags**: i
- **youtube**: 7tkCzLwZnpI
- **niches**: undefined

## Pallof press

- **id**: pallof-press
- **title**: Pallof press
- **match**: \bpallof\s+press\b
- **flags**: i
- **youtube**: f_D0GByfZh0
- **niches**: undefined

## Wall slide

- **id**: wall-slide
- **title**: Wall slide
- **match**: \bwall\s+slides?\b
- **flags**: i
- **youtube**: rw35lIr2LjA
- **niches**: undefined

## Foam roll (quads)

- **id**: foam-roll-quads
- **title**: Foam roll (quads)
- **match**: \bfoam\s+roll(ing)?\b.*\bquads?\b|\broll(ing)?\s+(my\s+)?quads?\b
- **flags**: i
- **youtube**: Ukk_LNN_uPc
- **niches**: undefined

## Padel basics

- **id**: padel-basics
- **title**: Padel basics
- **match**: \bpadel\b.*\b(basics?|beginner|learn|play|rules|start|right)\b|\b(basics?|beginner|learn|play|rules|start|right)\b.*\bpadel\b|\b(how to|learn to)\s+play\s+padel\b|\bplay\s+padel\b|\bnever played padel\b
- **flags**: i
- **youtube**: V_Gqgbk7Yxw
- **niches**: undefined

## Padel swing

- **id**: padel-swing
- **title**: Padel swing
- **match**: \bpadel\b.*\b(swing|racket|forehand|backhand|strokes?)\b|\b(swing|racket)\b.*\bpadel\b
- **flags**: i
- **youtube**: STtWns5jXrY
- **niches**: undefined

## Padel serve

- **id**: padel-serve
- **title**: Padel serve
- **match**: \bpadel\s+serve\b|\bserve\s+in\s+padel\b
- **flags**: i
- **youtube**: YSCbbCYfc9Y
- **niches**: undefined

## Tennis forehand

- **id**: tennis-forehand
- **title**: Tennis forehand
- **match**: \b(tennis\s+)?forehand\b
- **flags**: i
- **youtube**: 8V_KWh1Uoeo
- **niches**: undefined

## Rainbow flick

- **id**: rainbow-flick
- **title**: Rainbow flick
- **match**: \brainbow\s+flick\b|\brainbow\s+in\s+soccer\b
- **flags**: i
- **youtube**: zzFOco6x5VU
- **niches**: undefined

## Basketball layup

- **id**: basketball-layup
- **title**: Basketball layup
- **match**: \b(basketball\s+)?layups?\b|\blayup\s+form\b
- **flags**: i
- **youtube**: q4IqeXob_qg
- **niches**: undefined

## Basketball dribbling

- **id**: basketball-dribble
- **title**: Basketball dribbling
- **match**: \bdribbl(?:e|ing)\s+(?:a\s+)?basketball\b|\bbasketball\s+dribbl
- **flags**: i
- **youtube**: 2FdfRrXsQ2g
- **niches**: undefined

## Basketball shooting form

- **id**: basketball-shot
- **title**: Basketball shooting form
- **match**: \b(shoot(?:ing)?\s+a?\s*basketball|basketball\s+shot)\b
- **flags**: i
- **youtube**: r8s2LKc9H0w
- **niches**: undefined

## Golf swing

- **id**: golf-swing
- **title**: Golf swing
- **match**: \bgolf\s+swing\b|\bswing\s+a?\s+golf\b
- **flags**: i
- **youtube**: me5gjIUe1Ks
- **niches**: undefined

## Sprint starting blocks

- **id**: sprint-blocks
- **title**: Sprint starting blocks
- **match**: \b(starting\s+blocks?|block\s+starts?|sprint\s+blocks?)\b
- **flags**: i
- **youtube**: SQsiWySb7UQ
- **niches**: undefined

## Football tackling

- **id**: football-tackle
- **title**: Football tackling
- **match**: \bfootball\s+tackling\b|\btackling\s+form\b|\bhow\s+to\s+tackle\b
- **flags**: i
- **youtube**: ltBIMo72C94
- **niches**: undefined

## Box jump

- **id**: box-jump
- **title**: Box jump
- **match**: \bbox\s+jumps?\b
- **flags**: i
- **youtube**: G-bxQY57mKc
- **niches**: undefined

## Sled push

- **id**: sled-push
- **title**: Sled push
- **match**: \bsled\s+push(?:es)?\b|\bprowler\s+push\b
- **flags**: i
- **youtube**: 1PmO6kzBEc8
- **niches**: undefined

## Step-up

- **id**: step-up
- **title**: Step-up
- **match**: \bstep[\s-]?ups?\b
- **flags**: i
- **youtube**: WCFCdxzFBa4
- **niches**: undefined

## Bicep curl

- **id**: bicep-curl
- **title**: Bicep curl
- **match**: \b(bicep|biceps)\s+curls?\b|\bhow (?:do i|to) (?:do a )?curl\b
- **flags**: i
- **youtube**: sAq_ocpRh_I
- **niches**: undefined

## Tricep pushdown

- **id**: tricep-pushdown
- **title**: Tricep pushdown
- **match**: \btricep\s+push[\s-]?downs?\b|\bcable\s+push[\s-]?downs?\b
- **flags**: i
- **youtube**: 2-LAMcpzODU
- **niches**: undefined

## Lateral raise

- **id**: lateral-raise
- **title**: Lateral raise
- **match**: \blateral\s+raises?\b|\bside\s+lateral\s+raises?\b
- **flags**: i
- **youtube**: 3VcKaXpzqRo
- **niches**: undefined

## Face pull

- **id**: face-pull
- **title**: Face pull
- **match**: \bface\s+pulls?\b
- **flags**: i
- **youtube**: sHSY0Ao8QHs
- **niches**: undefined

## Cable fly

- **id**: cable-fly
- **title**: Cable fly
- **match**: \bcable\s+(?:chest\s+)?flies?\b|\bcable\s+fly\b
- **flags**: i
- **youtube**: Iwe6AmxVf7o
- **niches**: undefined

## Chin-up

- **id**: chin-up
- **title**: Chin-up
- **match**: \bchin[\s-]?ups?\b
- **flags**: i
- **youtube**: bZ6Ysk9jf6E
- **niches**: undefined

## Leg curl

- **id**: leg-curl
- **title**: Leg curl
- **match**: \b(seated\s+|lying\s+)?leg\s+curls?\b
- **flags**: i
- **youtube**: ELOCsoDSmrg
- **niches**: undefined

## Calf raise

- **id**: calf-raise
- **title**: Calf raise
- **match**: \bcalf\s+raises?\b|\bstanding\s+calf\b
- **flags**: i
- **youtube**: 3UWi44yN-wM
- **niches**: undefined

## Hip hinge drill

- **id**: hip-hinge-drill
- **title**: Hip hinge drill
- **match**: \bhip\s+hinge\b|\bhinge\s+drill\b
- **flags**: i
- **youtube**: BIpnVb8v27Q
- **niches**: undefined

## Good morning

- **id**: good-morning
- **title**: Good morning
- **match**: \bgood\s+mornings?\b
- **flags**: i
- **youtube**: f23vXjoG2e8
- **niches**: undefined

## Kettlebell swing

- **id**: kettlebell-swing
- **title**: Kettlebell swing
- **match**: \bkettlebell\s+swings?\b|\bkb\s+swings?\b
- **flags**: i
- **youtube**: TjarIpMne1w
- **niches**: undefined

## Turkish get-up

- **id**: turkish-get-up
- **title**: Turkish get-up
- **match**: \bturkish\s+get[\s-]?ups?\b|\bget[\s-]?ups?\b.*\bkettlebell\b
- **flags**: i
- **youtube**: 0bWRPC49-KI
- **niches**: undefined

## Power clean

- **id**: power-clean
- **title**: Power clean
- **match**: \bpower\s+cleans?\b|\bhow (?:do i|to) (?:do a )?clean\b
- **flags**: i
- **youtube**: KwYJTpQ_x5A
- **niches**: undefined

## Barbell snatch

- **id**: barbell-snatch
- **title**: Barbell snatch
- **match**: \b(barbell\s+)?snatch(?:es)?\b|\bpower\s+snatch\b
- **flags**: i
- **youtube**: ydHHsju1-Nc
- **niches**: undefined

## Battle ropes

- **id**: battle-ropes
- **title**: Battle ropes
- **match**: \bbattle\s+ropes?\b|\bheavy\s+ropes?\b
- **flags**: i
- **youtube**: nzlmTiKqno0
- **niches**: undefined

## Rowing machine

- **id**: rowing-machine
- **title**: Rowing machine
- **match**: \browing\s+machine\b|\b(?:concept\s*2|erg)\s+row\b|\brow(?:ing)?\s+machine\s+technique\b
- **flags**: i
- **youtube**: 4zWu1yuJ0_g
- **niches**: undefined

## Jump rope

- **id**: jump-rope
- **title**: Jump rope
- **match**: \bjump\s+rope\b|\bskip(?:ping)?\s+rope\b
- **flags**: i
- **youtube**: u3zgHI8QnqE
- **niches**: undefined

## Mountain climbers

- **id**: mountain-climbers
- **title**: Mountain climbers
- **match**: \bmountain\s+climbers?\b
- **flags**: i
- **youtube**: nmwgirgXLYM
- **niches**: undefined

## Hollow body hold

- **id**: hollow-body-hold
- **title**: Hollow body hold
- **match**: \bhollow\s+(?:body\s+)?holds?\b|\bhollow\s+body\b
- **flags**: i
- **youtube**: n-H5EpKcP60
- **niches**: undefined

## Ab wheel rollout

- **id**: ab-wheel
- **title**: Ab wheel rollout
- **match**: \bab\s+wheel\b|\bab\s+roll[\s-]?outs?\b
- **flags**: i
- **youtube**: 5I3LgiumTJM
- **niches**: undefined

## World's greatest stretch

- **id**: worlds-greatest-stretch
- **title**: World's greatest stretch
- **match**: \bworlds?\s+greatest\s+stretch\b
- **flags**: i
- **youtube**: nnbYao-5bSI
- **niches**: undefined

## Tennis backhand

- **id**: tennis-backhand
- **title**: Tennis backhand
- **match**: \btennis\s+backhand\b|\bbackhand\s+(?:stroke|technique)\b
- **flags**: i
- **youtube**: gU0ueKnfePY
- **niches**: undefined

## Tennis serve

- **id**: tennis-serve
- **title**: Tennis serve
- **match**: \btennis\s+serve\b|\bserve\s+(?:in\s+)?tennis\b
- **flags**: i
- **youtube**: CXgfNBnetzQ
- **niches**: undefined

## Tennis volley

- **id**: tennis-volley
- **title**: Tennis volley
- **match**: \btennis\s+volley\b|\bvolley\s+(?:in\s+)?tennis\b
- **flags**: i
- **youtube**: ixtikTVrpEY
- **niches**: undefined

## Volley smash

- **id**: volley-smash
- **title**: Volley smash
- **match**: \bvolley\s+smash\b|\boverhead\s+smash\b|\bsmash\b.*\b(?:volley|padel|tennis)\b|\b(?:volley|padel)\b.*\bsmash\b
- **flags**: i
- **youtube**: Z-N3FYk7Qao
- **niches**: undefined

## Padel bandeja

- **id**: padel-bandeja
- **title**: Padel bandeja
- **match**: \bpadel\s+bandeja\b|\bbandeja\s+(?:shot|stroke)\b
- **flags**: i
- **youtube**: Z-N3FYk7Qao
- **niches**: undefined

## Padel volley

- **id**: padel-volley
- **title**: Padel volley
- **match**: \bpadel\s+volley\b|\bvolley\s+in\s+padel\b
- **flags**: i
- **youtube**: esVPzDJ6dV4
- **niches**: undefined

## Soccer shooting

- **id**: soccer-shoot
- **title**: Soccer shooting
- **match**: \bsoccer\s+shoot(?:ing)?\b|\bshoot(?:ing)?\s+a\s+soccer\b|\bfootball\s+shoot(?:ing)?\b
- **flags**: i
- **youtube**: AgrINZyoeeo
- **niches**: undefined

## Soccer kick

- **id**: soccer-kick
- **title**: Soccer kick
- **match**: \bhow\s+to\s+kick\s+a\s+soccer\b|\bkick(?:ing)?\s+a\s+soccer\s+ball\b|\bsoccer\s+kick\b
- **flags**: i
- **youtube**: 859umlqnjqw
- **niches**: undefined

## Boxing jab

- **id**: boxing-jab
- **title**: Boxing jab
- **match**: \b(?:how\s+to\s+)?throw\s+a\s+jab\b|\bboxing\s+jab\b|\bjab\s+(?:technique|form)\b
- **flags**: i
- **youtube**: YsFK1MMDQgk
- **niches**: undefined

## Boxing hook

- **id**: boxing-hook
- **title**: Boxing hook
- **match**: \bboxing\s+hook\b|\bhook\s+(?:punch|technique)\b
- **flags**: i
- **youtube**: ywzNGhZi3hg
- **niches**: undefined

## Triangle choke

- **id**: triangle-choke
- **title**: Triangle choke
- **match**: \btriangle\s+choke\b|\btriangle\s+submission\b
- **flags**: i
- **youtube**: k54daRsX3co
- **niches**: undefined

## Freestyle swimming

- **id**: freestyle-swim
- **title**: Freestyle swimming
- **match**: \bfreestyle\s+swim(?:ming)?\b|\bfront\s+crawl\b|\bswim(?:ming)?\s+stroke\b
- **flags**: i
- **youtube**: 5HLW2AI1Ink
- **niches**: undefined

## Volleyball set

- **id**: volleyball-set
- **title**: Volleyball set
- **match**: \bvolleyball\s+set(?:ting)?\b|\bset(?:ting)?\b.*\bvolleyball\b|\b(?:volleyball|volley)\s+set\b
- **flags**: i
- **youtube**: h5mpBCRK_yk
- **niches**: undefined

## Volleyball serve

- **id**: volleyball-serve
- **title**: Volleyball serve
- **match**: \bvolleyball\s+serve\b|\boverhand\s+serve\b.*\bvolleyball\b
- **flags**: i
- **youtube**: au3QYrvsy9k
- **niches**: undefined

## Running form

- **id**: running-form
- **title**: Running form
- **match**: \b(?:proper\s+)?running\s+form\b|\brunning\s+technique\b|\brun\s+form\b
- **flags**: i
- **youtube**: NhXSuyklE48
- **niches**: undefined

## Indoor cycling form

- **id**: indoor-cycling
- **title**: Indoor cycling form
- **match**: \bindoor\s+cycl(?:ing|e)\b|\bspin(?:ning)?\s+(?:bike|class)\s+form\b|\bbike\s+setup\b
- **flags**: i
- **youtube**: vDus3tYFEeg
- **niches**: undefined

## Football throw

- **id**: football-throw
- **title**: Football throw
- **match**: \bhow\s+to\s+throw\s+a\s+football\b|\bfootball\s+throw(?:ing)?\b|\bquarterback\s+throw\b
- **flags**: i
- **youtube**: uqqtmAl7Mdk
- **niches**: undefined

## Foam roll (IT band)

- **id**: foam-roll-it-band
- **title**: Foam roll (IT band)
- **match**: \bfoam\s+roll(?:ing)?\b.*\bit\s+bands?\b|\broll(?:ing)?\s+(?:my\s+)?it\s+bands?\b
- **flags**: i
- **youtube**: i9DvJa0mZQA
- **niches**: undefined

## Foam roll (upper back)

- **id**: foam-roll-upper-back
- **title**: Foam roll (upper back)
- **match**: \bfoam\s+roll(?:ing)?\b.*\b(upper\s+back|thoracic)\b|\broll(?:ing)?\s+(?:my\s+)?upper\s+back\b
- **flags**: i
- **youtube**: NS73eSohTbc
- **niches**: undefined

## 90/90 hip stretch

- **id**: 90-90-hip-stretch
- **title**: 90/90 hip stretch
- **match**: \b90\s*[-/]?\s*90\s+hip\b|\b90\s+90\s+stretch\b
- **flags**: i
- **youtube**: VYvMMw8z3rE
- **niches**: undefined

## Pigeon stretch

- **id**: pigeon-stretch
- **title**: Pigeon stretch
- **match**: \bpigeon\s+(?:pose|stretch)\b
- **flags**: i
- **youtube**: op-eDU9eNqM
- **niches**: undefined

## Hip flexor stretch

- **id**: hip-flexor-stretch
- **title**: Hip flexor stretch
- **match**: \bhip\s+flexor\s+stretch\b|\bhip\s+flexor\s+(?:stretch|mobility)\b
- **flags**: i
- **youtube**: tsGPYSQbZx4
- **niches**: undefined

## YTWL shoulder exercise

- **id**: ytwl-shoulder
- **title**: YTWL shoulder exercise
- **match**: \bytwl\b|\by\s+t\s+w\s+l\b|\bshoulder\s+ytwl\b
- **flags**: i
- **youtube**: Lk9ot_6zquk
- **niches**: undefined

## Sleeper stretch

- **id**: sleeper-stretch
- **title**: Sleeper stretch
- **match**: \bsleeper\s+stretch\b
- **flags**: i
- **youtube**: OX6GtqNsHjE
- **niches**: undefined

## McGill Big 3

- **id**: mcgill-big-3
- **title**: McGill Big 3
- **match**: \bmcgill\s+big\s+3\b|\bbig\s+3\s+exercises?\b
- **flags**: i
- **youtube**: P8YiZO3OGjk
- **niches**: undefined

## Terminal knee extension

- **id**: terminal-knee-extension
- **title**: Terminal knee extension
- **match**: \bterminal\s+knee\s+extension\b|\btke\b
- **flags**: i
- **youtube**: ppzDDzy0pRY
- **niches**: undefined

## Calf stretch (Achilles)

- **id**: calf-stretch-achilles
- **title**: Calf stretch (Achilles)
- **match**: \bcalf\s+stretch\b.*\bachilles\b|\bachilles\s+stretch\b
- **flags**: i
- **youtube**: y01ri_43G50
- **niches**: undefined

## Banded lateral walk

- **id**: banded-lateral-walk
- **title**: Banded lateral walk
- **match**: \bbanded\s+lateral\s+walks?\b|\blateral\s+band\s+walks?\b
- **flags**: i
- **youtube**: YCqrtnr6g5g
- **niches**: undefined

## Monster walk

- **id**: monster-walk
- **title**: Monster walk
- **match**: \bmonster\s+walks?\b
- **flags**: i
- **youtube**: yjN_sDUGHnQ
- **niches**: undefined

## Wall angel

- **id**: wall-angel
- **title**: Wall angel
- **match**: \bwall\s+angels?\b
- **flags**: i
- **youtube**: 4Fm0gLIeVcU
- **niches**: undefined

## Chin tuck

- **id**: chin-tuck
- **title**: Chin tuck
- **match**: \bchin\s+tucks?\b|\bchin\s+tuck\s+exercise\b
- **flags**: i
- **youtube**: 7rnlAVhAK-8
- **niches**: undefined

## Downward dog

- **id**: downward-dog
- **title**: Downward dog
- **match**: \bdownward\s+(?:facing\s+)?dog\b|\bdown\s+dog\b|\badho\s+mukha\b
- **flags**: i
- **youtube**: YqOqM79McYY
- **niches**: undefined

## Sun salutation

- **id**: sun-salutation
- **title**: Sun salutation
- **match**: \bsun\s+salutation\b|\bsurya\s+namaskar\b
- **flags**: i
- **youtube**: 8AakYeM23sI
- **niches**: undefined

## Warrior 2

- **id**: warrior-2
- **title**: Warrior 2
- **match**: \bwarrior\s+2\b|\bvirabhadrasana\s+ii\b
- **flags**: i
- **youtube**: 4Ejz7IgODlU
- **niches**: undefined

## Child's pose

- **id**: childs-pose
- **title**: Child's pose
- **match**: \bchild'?s?\s+pose\b|\bbalasana\b
- **flags**: i
- **youtube**: 2MJGg-dUKh0
- **niches**: undefined

## Pilates hundred

- **id**: pilates-hundred
- **title**: Pilates hundred
- **match**: \bpilates\s+hundred\b|\bthe\s+hundred\b.*\bpilates\b
- **flags**: i
- **youtube**: 9mlone4NObI
- **niches**: undefined

## Pilates roll-up

- **id**: pilates-roll-up
- **title**: Pilates roll-up
- **match**: \bpilates\s+roll[\s-]?ups?\b|\broll[\s-]?up\b.*\bpilates\b
- **flags**: i
- **youtube**: HB9ex7zlpcE
- **niches**: undefined

## Thoracic rotation

- **id**: thoracic-rotation
- **title**: Thoracic rotation
- **match**: \bthoracic\s+rotation\b|\bthoracic\s+mobility\b
- **flags**: i
- **youtube**: 76TrGccD9r4
- **niches**: undefined

## Hip CARs

- **id**: hip-cars
- **title**: Hip CARs
- **match**: \bhip\s+cars\b|\bcontrolled\s+articular\s+rotations?\b.*\bhip\b
- **flags**: i
- **youtube**: hRMrq6G81p8
- **niches**: undefined

## Diaphragmatic breathing

- **id**: diaphragmatic-breathing
- **title**: Diaphragmatic breathing
- **match**: \bdiaphragmatic\s+breath(?:ing)?\b|\bbelly\s+breath(?:ing)?\b
- **flags**: i
- **youtube**: Mg2ar-7_HfA
- **niches**: undefined

## Box breathing

- **id**: box-breathing
- **title**: Box breathing
- **match**: \bbox\s+breath(?:ing)?\b|\bsquare\s+breath(?:ing)?\b
- **flags**: i
- **youtube**: oq5pZ7dpUDc
- **niches**: undefined

## Hamstring stretch

- **id**: hamstring-stretch
- **title**: Hamstring stretch
- **match**: \bhamstring\s+stretch(?:es)?\b
- **flags**: i
- **youtube**: Il1L75v6gq0
- **niches**: undefined

## Figure-four stretch

- **id**: figure-four-stretch
- **title**: Figure-four stretch
- **match**: \bfigure\s+four\s+stretch\b|\bfigure[\s-]?4\s+stretch\b
- **flags**: i
- **youtube**: -g0nuyTHMrI
- **niches**: undefined

## Structured source (complete)

The following JSON retains all original keys, types, order of array entries, IDs, caveats and source references for machine comparison. The readable sections above are a view of the same data. This is knowledge/schema content, not a runtime user database.

```json
[
  {
    "id": "dumbbell-bench-press",
    "title": "Dumbbell bench press",
    "match": "\\bdumbbell\\s+bench[\\s-]?press\\b|\\bdb\\s+bench\\b",
    "flags": "i",
    "youtube": "VmB1G1K7v94"
  },
  {
    "id": "bench-press",
    "title": "Bench press",
    "match": "\\b(?:barbell\\s+)?bench[\\s-]?press\\b|\\bhow do i bench\\b|\\bhow to bench\\b|\\blearn how to bench\\b",
    "flags": "i",
    "youtube": "vthMCtgVtFw"
  },
  {
    "id": "incline-push-up",
    "title": "Incline push-up",
    "match": "\\bincline\\s+push[\\s-]?ups?\\b",
    "flags": "i",
    "youtube": "cfns5VDVVvk"
  },
  {
    "id": "scapular-push-up",
    "title": "Scapular push-up",
    "match": "\\bscapular\\s+push[\\s-]?ups?\\b|\\bscap\\s+push[\\s-]?ups?\\b|\\bpush[\\s-]?up\\s+plus\\b",
    "flags": "i",
    "youtube": "LeMk15TN0No"
  },
  {
    "id": "push-up",
    "title": "Push-up",
    "match": "\\b(?!(?:scapular|scap|incline)\\s+)push[\\s-]?ups?\\b",
    "flags": "i",
    "youtube": "IODxDxX7oi4"
  },
  {
    "id": "goblet-squat",
    "title": "Goblet squat",
    "match": "\\bgoblet\\s+squats?\\b",
    "flags": "i",
    "youtube": "0OWbS1WiUGU"
  },
  {
    "id": "front-squat",
    "title": "Front squat",
    "match": "\\bfront\\s+squats?\\b",
    "flags": "i",
    "youtube": "6HDiP65lO8Y"
  },
  {
    "id": "bulgarian-split-squat",
    "title": "Bulgarian split squat",
    "match": "\\b(bulgarian\\s+)?split\\s+squats?\\b",
    "flags": "i",
    "youtube": "2C-uNgKwPLE"
  },
  {
    "id": "spanish-squat",
    "title": "Spanish squat",
    "match": "\\bspanish\\s+squats?\\b",
    "flags": "i",
    "youtube": "hgFxm5KIF7M"
  },
  {
    "id": "hip-thrust",
    "title": "Hip thrust",
    "match": "\\bhip\\s+thrusts?\\b",
    "flags": "i",
    "youtube": "SEdqd1n0cvg"
  },
  {
    "id": "leg-press",
    "title": "Leg press",
    "match": "\\bleg\\s+press\\b",
    "flags": "i",
    "youtube": "K5n2vg3oZa4"
  },
  {
    "id": "box-step-up",
    "title": "Box step-up",
    "match": "\\bbox\\s+step[\\s-]?ups?\\b",
    "flags": "i",
    "youtube": "WCFCdxzFBa4"
  },
  {
    "id": "squat",
    "title": "Squat",
    "match": "\\b(?!(?:front|goblet|bulgarian|split|spanish)\\s+)squats?\\b",
    "flags": "i",
    "youtube": "ultWZbUMPL8"
  },
  {
    "id": "rdl",
    "title": "Romanian deadlift",
    "match": "\\b(romanian\\s+deadlifts?|rdl)\\b",
    "flags": "i",
    "youtube": "5bJEigM5iVg"
  },
  {
    "id": "deadlift",
    "title": "Deadlift",
    "match": "\\b(barbell\\s+)?deadlifts?\\b",
    "flags": "i",
    "youtube": "wYREQkVtvEc"
  },
  {
    "id": "lunge",
    "title": "Lunge",
    "match": "\\b(walking\\s+)?lunges?\\b",
    "flags": "i",
    "youtube": "QOVaHwm-Q6U"
  },
  {
    "id": "side-plank",
    "title": "Side plank",
    "match": "\\bside\\s+planks?\\b",
    "flags": "i",
    "youtube": "XeN4pEZZJNI"
  },
  {
    "id": "plank",
    "title": "Plank",
    "match": "\\b(?!(?:side\\s+))planks?\\b",
    "flags": "i",
    "youtube": "ASdvN_XEl_c"
  },
  {
    "id": "pull-up",
    "title": "Pull-up",
    "match": "\\bpull[\\s-]?ups?\\b",
    "flags": "i",
    "youtube": "eGo4IYlbE5g"
  },
  {
    "id": "lat-pulldown",
    "title": "Lat pulldown",
    "match": "\\blat\\s+pulldowns?\\b",
    "flags": "i",
    "youtube": "CAwf7n6Luuc"
  },
  {
    "id": "inverted-row",
    "title": "Inverted row",
    "match": "\\binverted\\s+rows?\\b|\\bbodyweight\\s+rows?\\b",
    "flags": "i",
    "youtube": "OYUxXMGVuuU"
  },
  {
    "id": "shoulder-press",
    "title": "Shoulder press",
    "match": "\\b(shoulder|overhead)\\s+press\\b|\\bmilitary\\s+press\\b",
    "flags": "i",
    "youtube": "B-aVuyhvLHU"
  },
  {
    "id": "row",
    "title": "Row",
    "match": "\\b(dumbbell\\s+rows?|bent[- ]over\\s+rows?|how (?:do i|to) row|rows?\\s+properly)\\b",
    "flags": "i",
    "youtube": "6TSP1TRMUzs"
  },
  {
    "id": "dip",
    "title": "Dip",
    "match": "\\b(tricep\\s+)?dips?\\b",
    "flags": "i",
    "youtube": "c3ZGl4pAwZ4"
  },
  {
    "id": "burpee",
    "title": "Burpee",
    "match": "\\bburpees?\\b",
    "flags": "i",
    "youtube": "wS4OsJ4yzx4"
  },
  {
    "id": "farmer-carry",
    "title": "Farmer carry",
    "match": "\\bfarmer\\s+(carry|walk)s?\\b",
    "flags": "i",
    "youtube": "8OtwXwrJizk"
  },
  {
    "id": "dead-bug",
    "title": "Dead bug",
    "match": "\\bdead[\\s-]?bugs?\\b",
    "flags": "i",
    "youtube": "JrcoGEZn6L4"
  },
  {
    "id": "bird-dog",
    "title": "Bird dog",
    "match": "\\bbird[\\s-]?dogs?\\b",
    "flags": "i",
    "youtube": "Jmq2El0u8T0"
  },
  {
    "id": "clamshell",
    "title": "Clamshell",
    "match": "\\bclamshells?\\b",
    "flags": "i",
    "youtube": "ymjOGuPjOSE"
  },
  {
    "id": "glute-bridge",
    "title": "Glute bridge",
    "match": "\\bglute\\s+bridges?\\b",
    "flags": "i",
    "youtube": "8bbE64NuDTU"
  },
  {
    "id": "cat-cow",
    "title": "Cat-cow stretch",
    "match": "\\bcat[\\s-]?cows?\\b|\\bcat\\s+cow\\b",
    "flags": "i",
    "youtube": "rbuptYr2CGM"
  },
  {
    "id": "band-pull-apart",
    "title": "Band pull-apart",
    "match": "\\bband\\s+pull[\\s-]?aparts?\\b",
    "flags": "i",
    "youtube": "7tkCzLwZnpI"
  },
  {
    "id": "pallof-press",
    "title": "Pallof press",
    "match": "\\bpallof\\s+press\\b",
    "flags": "i",
    "youtube": "f_D0GByfZh0"
  },
  {
    "id": "wall-slide",
    "title": "Wall slide",
    "match": "\\bwall\\s+slides?\\b",
    "flags": "i",
    "youtube": "rw35lIr2LjA"
  },
  {
    "id": "foam-roll-quads",
    "title": "Foam roll (quads)",
    "match": "\\bfoam\\s+roll(ing)?\\b.*\\bquads?\\b|\\broll(ing)?\\s+(my\\s+)?quads?\\b",
    "flags": "i",
    "youtube": "Ukk_LNN_uPc"
  },
  {
    "id": "padel-basics",
    "title": "Padel basics",
    "match": "\\bpadel\\b.*\\b(basics?|beginner|learn|play|rules|start|right)\\b|\\b(basics?|beginner|learn|play|rules|start|right)\\b.*\\bpadel\\b|\\b(how to|learn to)\\s+play\\s+padel\\b|\\bplay\\s+padel\\b|\\bnever played padel\\b",
    "flags": "i",
    "youtube": "V_Gqgbk7Yxw"
  },
  {
    "id": "padel-swing",
    "title": "Padel swing",
    "match": "\\bpadel\\b.*\\b(swing|racket|forehand|backhand|strokes?)\\b|\\b(swing|racket)\\b.*\\bpadel\\b",
    "flags": "i",
    "youtube": "STtWns5jXrY"
  },
  {
    "id": "padel-serve",
    "title": "Padel serve",
    "match": "\\bpadel\\s+serve\\b|\\bserve\\s+in\\s+padel\\b",
    "flags": "i",
    "youtube": "YSCbbCYfc9Y"
  },
  {
    "id": "tennis-forehand",
    "title": "Tennis forehand",
    "match": "\\b(tennis\\s+)?forehand\\b",
    "flags": "i",
    "youtube": "8V_KWh1Uoeo"
  },
  {
    "id": "rainbow-flick",
    "title": "Rainbow flick",
    "match": "\\brainbow\\s+flick\\b|\\brainbow\\s+in\\s+soccer\\b",
    "flags": "i",
    "youtube": "zzFOco6x5VU"
  },
  {
    "id": "basketball-layup",
    "title": "Basketball layup",
    "match": "\\b(basketball\\s+)?layups?\\b|\\blayup\\s+form\\b",
    "flags": "i",
    "youtube": "q4IqeXob_qg"
  },
  {
    "id": "basketball-dribble",
    "title": "Basketball dribbling",
    "match": "\\bdribbl(?:e|ing)\\s+(?:a\\s+)?basketball\\b|\\bbasketball\\s+dribbl",
    "flags": "i",
    "youtube": "2FdfRrXsQ2g"
  },
  {
    "id": "basketball-shot",
    "title": "Basketball shooting form",
    "match": "\\b(shoot(?:ing)?\\s+a?\\s*basketball|basketball\\s+shot)\\b",
    "flags": "i",
    "youtube": "r8s2LKc9H0w"
  },
  {
    "id": "golf-swing",
    "title": "Golf swing",
    "match": "\\bgolf\\s+swing\\b|\\bswing\\s+a?\\s+golf\\b",
    "flags": "i",
    "youtube": "me5gjIUe1Ks"
  },
  {
    "id": "sprint-blocks",
    "title": "Sprint starting blocks",
    "match": "\\b(starting\\s+blocks?|block\\s+starts?|sprint\\s+blocks?)\\b",
    "flags": "i",
    "youtube": "SQsiWySb7UQ"
  },
  {
    "id": "football-tackle",
    "title": "Football tackling",
    "match": "\\bfootball\\s+tackling\\b|\\btackling\\s+form\\b|\\bhow\\s+to\\s+tackle\\b",
    "flags": "i",
    "youtube": "ltBIMo72C94"
  },
  {
    "id": "box-jump",
    "title": "Box jump",
    "match": "\\bbox\\s+jumps?\\b",
    "flags": "i",
    "youtube": "G-bxQY57mKc"
  },
  {
    "id": "sled-push",
    "title": "Sled push",
    "match": "\\bsled\\s+push(?:es)?\\b|\\bprowler\\s+push\\b",
    "flags": "i",
    "youtube": "1PmO6kzBEc8"
  },
  {
    "id": "step-up",
    "title": "Step-up",
    "match": "\\bstep[\\s-]?ups?\\b",
    "flags": "i",
    "youtube": "WCFCdxzFBa4"
  },
  {
    "id": "bicep-curl",
    "title": "Bicep curl",
    "match": "\\b(bicep|biceps)\\s+curls?\\b|\\bhow (?:do i|to) (?:do a )?curl\\b",
    "flags": "i",
    "youtube": "sAq_ocpRh_I"
  },
  {
    "id": "tricep-pushdown",
    "title": "Tricep pushdown",
    "match": "\\btricep\\s+push[\\s-]?downs?\\b|\\bcable\\s+push[\\s-]?downs?\\b",
    "flags": "i",
    "youtube": "2-LAMcpzODU"
  },
  {
    "id": "lateral-raise",
    "title": "Lateral raise",
    "match": "\\blateral\\s+raises?\\b|\\bside\\s+lateral\\s+raises?\\b",
    "flags": "i",
    "youtube": "3VcKaXpzqRo"
  },
  {
    "id": "face-pull",
    "title": "Face pull",
    "match": "\\bface\\s+pulls?\\b",
    "flags": "i",
    "youtube": "sHSY0Ao8QHs"
  },
  {
    "id": "cable-fly",
    "title": "Cable fly",
    "match": "\\bcable\\s+(?:chest\\s+)?flies?\\b|\\bcable\\s+fly\\b",
    "flags": "i",
    "youtube": "Iwe6AmxVf7o"
  },
  {
    "id": "chin-up",
    "title": "Chin-up",
    "match": "\\bchin[\\s-]?ups?\\b",
    "flags": "i",
    "youtube": "bZ6Ysk9jf6E"
  },
  {
    "id": "leg-curl",
    "title": "Leg curl",
    "match": "\\b(seated\\s+|lying\\s+)?leg\\s+curls?\\b",
    "flags": "i",
    "youtube": "ELOCsoDSmrg"
  },
  {
    "id": "calf-raise",
    "title": "Calf raise",
    "match": "\\bcalf\\s+raises?\\b|\\bstanding\\s+calf\\b",
    "flags": "i",
    "youtube": "3UWi44yN-wM"
  },
  {
    "id": "hip-hinge-drill",
    "title": "Hip hinge drill",
    "match": "\\bhip\\s+hinge\\b|\\bhinge\\s+drill\\b",
    "flags": "i",
    "youtube": "BIpnVb8v27Q"
  },
  {
    "id": "good-morning",
    "title": "Good morning",
    "match": "\\bgood\\s+mornings?\\b",
    "flags": "i",
    "youtube": "f23vXjoG2e8"
  },
  {
    "id": "kettlebell-swing",
    "title": "Kettlebell swing",
    "match": "\\bkettlebell\\s+swings?\\b|\\bkb\\s+swings?\\b",
    "flags": "i",
    "youtube": "TjarIpMne1w"
  },
  {
    "id": "turkish-get-up",
    "title": "Turkish get-up",
    "match": "\\bturkish\\s+get[\\s-]?ups?\\b|\\bget[\\s-]?ups?\\b.*\\bkettlebell\\b",
    "flags": "i",
    "youtube": "0bWRPC49-KI"
  },
  {
    "id": "power-clean",
    "title": "Power clean",
    "match": "\\bpower\\s+cleans?\\b|\\bhow (?:do i|to) (?:do a )?clean\\b",
    "flags": "i",
    "youtube": "KwYJTpQ_x5A"
  },
  {
    "id": "barbell-snatch",
    "title": "Barbell snatch",
    "match": "\\b(barbell\\s+)?snatch(?:es)?\\b|\\bpower\\s+snatch\\b",
    "flags": "i",
    "youtube": "ydHHsju1-Nc"
  },
  {
    "id": "battle-ropes",
    "title": "Battle ropes",
    "match": "\\bbattle\\s+ropes?\\b|\\bheavy\\s+ropes?\\b",
    "flags": "i",
    "youtube": "nzlmTiKqno0"
  },
  {
    "id": "rowing-machine",
    "title": "Rowing machine",
    "match": "\\browing\\s+machine\\b|\\b(?:concept\\s*2|erg)\\s+row\\b|\\brow(?:ing)?\\s+machine\\s+technique\\b",
    "flags": "i",
    "youtube": "4zWu1yuJ0_g"
  },
  {
    "id": "jump-rope",
    "title": "Jump rope",
    "match": "\\bjump\\s+rope\\b|\\bskip(?:ping)?\\s+rope\\b",
    "flags": "i",
    "youtube": "u3zgHI8QnqE"
  },
  {
    "id": "mountain-climbers",
    "title": "Mountain climbers",
    "match": "\\bmountain\\s+climbers?\\b",
    "flags": "i",
    "youtube": "nmwgirgXLYM"
  },
  {
    "id": "hollow-body-hold",
    "title": "Hollow body hold",
    "match": "\\bhollow\\s+(?:body\\s+)?holds?\\b|\\bhollow\\s+body\\b",
    "flags": "i",
    "youtube": "n-H5EpKcP60"
  },
  {
    "id": "ab-wheel",
    "title": "Ab wheel rollout",
    "match": "\\bab\\s+wheel\\b|\\bab\\s+roll[\\s-]?outs?\\b",
    "flags": "i",
    "youtube": "5I3LgiumTJM"
  },
  {
    "id": "worlds-greatest-stretch",
    "title": "World's greatest stretch",
    "match": "\\bworlds?\\s+greatest\\s+stretch\\b",
    "flags": "i",
    "youtube": "nnbYao-5bSI"
  },
  {
    "id": "tennis-backhand",
    "title": "Tennis backhand",
    "match": "\\btennis\\s+backhand\\b|\\bbackhand\\s+(?:stroke|technique)\\b",
    "flags": "i",
    "youtube": "gU0ueKnfePY"
  },
  {
    "id": "tennis-serve",
    "title": "Tennis serve",
    "match": "\\btennis\\s+serve\\b|\\bserve\\s+(?:in\\s+)?tennis\\b",
    "flags": "i",
    "youtube": "CXgfNBnetzQ"
  },
  {
    "id": "tennis-volley",
    "title": "Tennis volley",
    "match": "\\btennis\\s+volley\\b|\\bvolley\\s+(?:in\\s+)?tennis\\b",
    "flags": "i",
    "youtube": "ixtikTVrpEY"
  },
  {
    "id": "volley-smash",
    "title": "Volley smash",
    "match": "\\bvolley\\s+smash\\b|\\boverhead\\s+smash\\b|\\bsmash\\b.*\\b(?:volley|padel|tennis)\\b|\\b(?:volley|padel)\\b.*\\bsmash\\b",
    "flags": "i",
    "youtube": "Z-N3FYk7Qao"
  },
  {
    "id": "padel-bandeja",
    "title": "Padel bandeja",
    "match": "\\bpadel\\s+bandeja\\b|\\bbandeja\\s+(?:shot|stroke)\\b",
    "flags": "i",
    "youtube": "Z-N3FYk7Qao"
  },
  {
    "id": "padel-volley",
    "title": "Padel volley",
    "match": "\\bpadel\\s+volley\\b|\\bvolley\\s+in\\s+padel\\b",
    "flags": "i",
    "youtube": "esVPzDJ6dV4"
  },
  {
    "id": "soccer-shoot",
    "title": "Soccer shooting",
    "match": "\\bsoccer\\s+shoot(?:ing)?\\b|\\bshoot(?:ing)?\\s+a\\s+soccer\\b|\\bfootball\\s+shoot(?:ing)?\\b",
    "flags": "i",
    "youtube": "AgrINZyoeeo"
  },
  {
    "id": "soccer-kick",
    "title": "Soccer kick",
    "match": "\\bhow\\s+to\\s+kick\\s+a\\s+soccer\\b|\\bkick(?:ing)?\\s+a\\s+soccer\\s+ball\\b|\\bsoccer\\s+kick\\b",
    "flags": "i",
    "youtube": "859umlqnjqw"
  },
  {
    "id": "boxing-jab",
    "title": "Boxing jab",
    "match": "\\b(?:how\\s+to\\s+)?throw\\s+a\\s+jab\\b|\\bboxing\\s+jab\\b|\\bjab\\s+(?:technique|form)\\b",
    "flags": "i",
    "youtube": "YsFK1MMDQgk"
  },
  {
    "id": "boxing-hook",
    "title": "Boxing hook",
    "match": "\\bboxing\\s+hook\\b|\\bhook\\s+(?:punch|technique)\\b",
    "flags": "i",
    "youtube": "ywzNGhZi3hg"
  },
  {
    "id": "triangle-choke",
    "title": "Triangle choke",
    "match": "\\btriangle\\s+choke\\b|\\btriangle\\s+submission\\b",
    "flags": "i",
    "youtube": "k54daRsX3co"
  },
  {
    "id": "freestyle-swim",
    "title": "Freestyle swimming",
    "match": "\\bfreestyle\\s+swim(?:ming)?\\b|\\bfront\\s+crawl\\b|\\bswim(?:ming)?\\s+stroke\\b",
    "flags": "i",
    "youtube": "5HLW2AI1Ink"
  },
  {
    "id": "volleyball-set",
    "title": "Volleyball set",
    "match": "\\bvolleyball\\s+set(?:ting)?\\b|\\bset(?:ting)?\\b.*\\bvolleyball\\b|\\b(?:volleyball|volley)\\s+set\\b",
    "flags": "i",
    "youtube": "h5mpBCRK_yk"
  },
  {
    "id": "volleyball-serve",
    "title": "Volleyball serve",
    "match": "\\bvolleyball\\s+serve\\b|\\boverhand\\s+serve\\b.*\\bvolleyball\\b",
    "flags": "i",
    "youtube": "au3QYrvsy9k"
  },
  {
    "id": "running-form",
    "title": "Running form",
    "match": "\\b(?:proper\\s+)?running\\s+form\\b|\\brunning\\s+technique\\b|\\brun\\s+form\\b",
    "flags": "i",
    "youtube": "NhXSuyklE48"
  },
  {
    "id": "indoor-cycling",
    "title": "Indoor cycling form",
    "match": "\\bindoor\\s+cycl(?:ing|e)\\b|\\bspin(?:ning)?\\s+(?:bike|class)\\s+form\\b|\\bbike\\s+setup\\b",
    "flags": "i",
    "youtube": "vDus3tYFEeg"
  },
  {
    "id": "football-throw",
    "title": "Football throw",
    "match": "\\bhow\\s+to\\s+throw\\s+a\\s+football\\b|\\bfootball\\s+throw(?:ing)?\\b|\\bquarterback\\s+throw\\b",
    "flags": "i",
    "youtube": "uqqtmAl7Mdk"
  },
  {
    "id": "foam-roll-it-band",
    "title": "Foam roll (IT band)",
    "match": "\\bfoam\\s+roll(?:ing)?\\b.*\\bit\\s+bands?\\b|\\broll(?:ing)?\\s+(?:my\\s+)?it\\s+bands?\\b",
    "flags": "i",
    "youtube": "i9DvJa0mZQA"
  },
  {
    "id": "foam-roll-upper-back",
    "title": "Foam roll (upper back)",
    "match": "\\bfoam\\s+roll(?:ing)?\\b.*\\b(upper\\s+back|thoracic)\\b|\\broll(?:ing)?\\s+(?:my\\s+)?upper\\s+back\\b",
    "flags": "i",
    "youtube": "NS73eSohTbc"
  },
  {
    "id": "90-90-hip-stretch",
    "title": "90/90 hip stretch",
    "match": "\\b90\\s*[-/]?\\s*90\\s+hip\\b|\\b90\\s+90\\s+stretch\\b",
    "flags": "i",
    "youtube": "VYvMMw8z3rE"
  },
  {
    "id": "pigeon-stretch",
    "title": "Pigeon stretch",
    "match": "\\bpigeon\\s+(?:pose|stretch)\\b",
    "flags": "i",
    "youtube": "op-eDU9eNqM"
  },
  {
    "id": "hip-flexor-stretch",
    "title": "Hip flexor stretch",
    "match": "\\bhip\\s+flexor\\s+stretch\\b|\\bhip\\s+flexor\\s+(?:stretch|mobility)\\b",
    "flags": "i",
    "youtube": "tsGPYSQbZx4"
  },
  {
    "id": "ytwl-shoulder",
    "title": "YTWL shoulder exercise",
    "match": "\\bytwl\\b|\\by\\s+t\\s+w\\s+l\\b|\\bshoulder\\s+ytwl\\b",
    "flags": "i",
    "youtube": "Lk9ot_6zquk"
  },
  {
    "id": "sleeper-stretch",
    "title": "Sleeper stretch",
    "match": "\\bsleeper\\s+stretch\\b",
    "flags": "i",
    "youtube": "OX6GtqNsHjE"
  },
  {
    "id": "mcgill-big-3",
    "title": "McGill Big 3",
    "match": "\\bmcgill\\s+big\\s+3\\b|\\bbig\\s+3\\s+exercises?\\b",
    "flags": "i",
    "youtube": "P8YiZO3OGjk"
  },
  {
    "id": "terminal-knee-extension",
    "title": "Terminal knee extension",
    "match": "\\bterminal\\s+knee\\s+extension\\b|\\btke\\b",
    "flags": "i",
    "youtube": "ppzDDzy0pRY"
  },
  {
    "id": "calf-stretch-achilles",
    "title": "Calf stretch (Achilles)",
    "match": "\\bcalf\\s+stretch\\b.*\\bachilles\\b|\\bachilles\\s+stretch\\b",
    "flags": "i",
    "youtube": "y01ri_43G50"
  },
  {
    "id": "banded-lateral-walk",
    "title": "Banded lateral walk",
    "match": "\\bbanded\\s+lateral\\s+walks?\\b|\\blateral\\s+band\\s+walks?\\b",
    "flags": "i",
    "youtube": "YCqrtnr6g5g"
  },
  {
    "id": "monster-walk",
    "title": "Monster walk",
    "match": "\\bmonster\\s+walks?\\b",
    "flags": "i",
    "youtube": "yjN_sDUGHnQ"
  },
  {
    "id": "wall-angel",
    "title": "Wall angel",
    "match": "\\bwall\\s+angels?\\b",
    "flags": "i",
    "youtube": "4Fm0gLIeVcU"
  },
  {
    "id": "chin-tuck",
    "title": "Chin tuck",
    "match": "\\bchin\\s+tucks?\\b|\\bchin\\s+tuck\\s+exercise\\b",
    "flags": "i",
    "youtube": "7rnlAVhAK-8"
  },
  {
    "id": "downward-dog",
    "title": "Downward dog",
    "match": "\\bdownward\\s+(?:facing\\s+)?dog\\b|\\bdown\\s+dog\\b|\\badho\\s+mukha\\b",
    "flags": "i",
    "youtube": "YqOqM79McYY"
  },
  {
    "id": "sun-salutation",
    "title": "Sun salutation",
    "match": "\\bsun\\s+salutation\\b|\\bsurya\\s+namaskar\\b",
    "flags": "i",
    "youtube": "8AakYeM23sI"
  },
  {
    "id": "warrior-2",
    "title": "Warrior 2",
    "match": "\\bwarrior\\s+2\\b|\\bvirabhadrasana\\s+ii\\b",
    "flags": "i",
    "youtube": "4Ejz7IgODlU"
  },
  {
    "id": "childs-pose",
    "title": "Child's pose",
    "match": "\\bchild'?s?\\s+pose\\b|\\bbalasana\\b",
    "flags": "i",
    "youtube": "2MJGg-dUKh0"
  },
  {
    "id": "pilates-hundred",
    "title": "Pilates hundred",
    "match": "\\bpilates\\s+hundred\\b|\\bthe\\s+hundred\\b.*\\bpilates\\b",
    "flags": "i",
    "youtube": "9mlone4NObI"
  },
  {
    "id": "pilates-roll-up",
    "title": "Pilates roll-up",
    "match": "\\bpilates\\s+roll[\\s-]?ups?\\b|\\broll[\\s-]?up\\b.*\\bpilates\\b",
    "flags": "i",
    "youtube": "HB9ex7zlpcE"
  },
  {
    "id": "thoracic-rotation",
    "title": "Thoracic rotation",
    "match": "\\bthoracic\\s+rotation\\b|\\bthoracic\\s+mobility\\b",
    "flags": "i",
    "youtube": "76TrGccD9r4"
  },
  {
    "id": "hip-cars",
    "title": "Hip CARs",
    "match": "\\bhip\\s+cars\\b|\\bcontrolled\\s+articular\\s+rotations?\\b.*\\bhip\\b",
    "flags": "i",
    "youtube": "hRMrq6G81p8"
  },
  {
    "id": "diaphragmatic-breathing",
    "title": "Diaphragmatic breathing",
    "match": "\\bdiaphragmatic\\s+breath(?:ing)?\\b|\\bbelly\\s+breath(?:ing)?\\b",
    "flags": "i",
    "youtube": "Mg2ar-7_HfA"
  },
  {
    "id": "box-breathing",
    "title": "Box breathing",
    "match": "\\bbox\\s+breath(?:ing)?\\b|\\bsquare\\s+breath(?:ing)?\\b",
    "flags": "i",
    "youtube": "oq5pZ7dpUDc"
  },
  {
    "id": "hamstring-stretch",
    "title": "Hamstring stretch",
    "match": "\\bhamstring\\s+stretch(?:es)?\\b",
    "flags": "i",
    "youtube": "Il1L75v6gq0"
  },
  {
    "id": "figure-four-stretch",
    "title": "Figure-four stretch",
    "match": "\\bfigure\\s+four\\s+stretch\\b|\\bfigure[\\s-]?4\\s+stretch\\b",
    "flags": "i",
    "youtube": "-g0nuyTHMrI"
  }
]
```

## Source reference

- `ryx-brain/src/exerciseMedia.js` — Complete file (785 lines)
- `ryx-brain/src/cardCoerce.js` — Complete file (266 lines)

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
