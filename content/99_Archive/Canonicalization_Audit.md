---
id: "ryx.audit.canonicalization_0_2_0"
title: "Canonicalization Audit"
type: "eval"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "CORYX-RYX-Brain/MIGRATION_REVIEW.md"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
---

# Canonicalization Audit

All 20 requested validation checks passed. This reference_only evidence does not claim live runtime conformance. Source fingerprints compare this phase start with completion; protected historical files and exact note snapshots were verified.

~~~json
{
  "date": "2026-10-14",
  "passed": true,
  "checks": [
    {
      "number": 1,
      "name": "H01–H12 explicit approved decisions and required statuses",
      "passed": true
    },
    {
      "number": 2,
      "name": "Every H maps back to its C findings and all 22 remain covered",
      "passed": true
    },
    {
      "number": 3,
      "name": "Updated note source_files retained; IDs and status model valid",
      "passed": true
    },
    {
      "number": 4,
      "name": "No introduced secret values; credential inputs excluded",
      "passed": true
    },
    {
      "number": 5,
      "name": "Only Markdown notes introduced; no runtime/user/fixture data introduced",
      "passed": true
    },
    {
      "number": 6,
      "name": "All audited original source code/files unchanged during this phase",
      "passed": true
    },
    {
      "number": 7,
      "name": "v0.1.0 manifest and migration reports unchanged; exact historical notes recoverable",
      "passed": true
    },
    {
      "number": 8,
      "name": "v0.2.0 manifest contains exactly canonical production notes",
      "passed": true
    },
    {
      "number": 9,
      "name": "Exact global hierarchy and owner references; no retained conflicting active projections",
      "passed": true
    },
    {
      "number": 10,
      "name": "Active capability promises limited to implemented or clearly planned capabilities",
      "passed": true
    },
    {
      "number": 11,
      "name": "No active note promises unlimited credits; source allowances and weights unchanged",
      "passed": true
    },
    {
      "number": 12,
      "name": "Inference never canonically establishes medical clearance or protected records",
      "passed": true
    },
    {
      "number": 13,
      "name": "Crisis is terminal and future final safety follows normal coercion",
      "passed": true
    },
    {
      "number": 14,
      "name": "Companion authority comes from state and not casual mention",
      "passed": true
    },
    {
      "number": 15,
      "name": "Trainer delivery/application require execution confirmation",
      "passed": true
    },
    {
      "number": 16,
      "name": "Equipment and program-source gaps obey confirmed context and explicit labelling",
      "passed": true
    },
    {
      "number": 17,
      "name": "Body Map documents current 34-zone schema and original scales; event semantic intent explicit",
      "passed": true
    },
    {
      "number": 18,
      "name": "Complete structured knowledge payloads and stable provenance survive",
      "passed": true
    },
    {
      "number": 19,
      "name": "Evaluation explicitly distinguishes raw-provider tests and full user-visible pipeline",
      "passed": true
    },
    {
      "number": 20,
      "name": "All Obsidian note and heading links resolve; ownership references and table layout valid",
      "passed": true
    }
  ],
  "H_decisions_resolved": 12,
  "notes_modified": 116,
  "notes_created": 7,
  "notes_marked_legacy": 1,
  "notes_marked_reference_only": 17,
  "canonical_production_notes": 102,
  "duplicate_rule_families_centralized": 8,
  "baseline_changed": false,
  "candidate_created": true,
  "production_source_files_changed": false,
  "runtime_integration_performed": false,
  "remaining_product_decisions": 4,
  "remaining_runtime_alignment_groups": 12,
  "historical_conflicts_retained": 22,
  "readiness": "READY FOR IMPLEMENTATION",
  "sourceHashes": {
    "RYX_Wedge_Knowledge_Bases_v1/fitness/bodybuilding.json": "e34c6c45197e65d4f5682ee31bdc669a0c0db34f5bbe2ad174ab6a6aa01bd8da",
    "RYX_Wedge_Knowledge_Bases_v1/fitness/calisthenics.json": "e9e75f6b0ec613fa185a123c7eccffaa014fbb2d5fa60e64b8f96cdce6a9fcfd",
    "RYX_Wedge_Knowledge_Bases_v1/fitness/crossfit.json": "89dd6f208e506f5a67193c2a04bfa9766cc22490012f84bf07e381ee3510c85e",
    "RYX_Wedge_Knowledge_Bases_v1/fitness/general.json": "0edba95e14dc53e9411bcbfcd2fef63260ae0979b06bf17de5d71972eba9fef3",
    "RYX_Wedge_Knowledge_Bases_v1/fitness/powerlifting.json": "cc896f71b93dd9547863a7a73755ce44a1d129e41a81e5c3aa1f697dbd4b4ea8",
    "RYX_Wedge_Knowledge_Bases_v1/index.json": "4cffc2d72933ff96e03eecf793ee201ef122a2b386501c1772b3f548c3fc8b6a",
    "RYX_Wedge_Knowledge_Bases_v1/ryx-wedge-kb.schema.json": "ef0068922c56c10955dd0acc339209621e44d0233325d2616185dfe07a320a6c",
    "RYX_Wedge_Knowledge_Bases_v1/sports/basketball.json": "5f6d99b95278673539ceb14644d76f88cc472091b507ef586987139093fac635",
    "RYX_Wedge_Knowledge_Bases_v1/sports/combat.json": "428201010b11544bcb5a6feddf204fc25e3f6a61527f202277ff0c2c4ced8335",
    "RYX_Wedge_Knowledge_Bases_v1/sports/football.json": "e0176d266ebd3bd16d52399e31efd630d423bdf72bb3277404f104ea66ac82c5",
    "RYX_Wedge_Knowledge_Bases_v1/sports/golf.json": "20ed6f43ff1402d406c3730acb1308114c984fd6b1a1e371f32136403b15b631",
    "RYX_Wedge_Knowledge_Bases_v1/sports/padel.json": "8b00ffc53540afec47ef6c1cd904a2ebba7a24f0480989162d79e5e7395c0bfe",
    "RYX_Wedge_Knowledge_Bases_v1/sports/swimming.json": "3dcdbdbb8b2e99d1315db31c6dca724a70139e6bbfe3430932696f7565e857b3",
    "RYX_Wedge_Knowledge_Bases_v1/sports/tennis.json": "acdb5bc63505b5015832649614a369a8e3eafcee0285408b15499e209f1565d6",
    "RYX_Wedge_Knowledge_Bases_v1/wellness/rehab.json": "7c1707e89eb109201bb41d2bb09d19ca1e5b9e1541461f7098dd993f1bb71719",
    "RYX_Wedge_Knowledge_Bases_v1/wellness/yoga.json": "64e44d28cfefebe12dad5b51c9e6c14439fab5b4e1f33815c9c2507ae119dbde",
    "docs/product/ryx-athlete-persona-plan.md": "2ce3e3ae32a33f7f4158affc09288e4934bf2d821eb928807d02b33b62cddc2b",
    "docs/product/ryx-persona-plan.md": "6434b2e79bfdd18e74211f1f53d3343f8b3279e07294b54371e5acd8d9fe57a9",
    "ryx-brain/COVERAGE.md": "3d2cb9e3e8117c125100ffe9a326148ff20b25f0b36167be6d2276e1cf739af1",
    "ryx-brain/README.md": "d8bf2bde40cd12daf8915c1a665f9396cdcecede47bd1165de5162ec665a6b57",
    "ryx-brain/docs/accounts.md": "ade63a7cec2d07285ef97fb94f51d1de5befbde01914cee7e63f16f5070040e3",
    "ryx-brain/docs/backlog.md": "f4015a9797799df95918b51f27fde517537e21e2555943e74c22ec5c89b5dc23",
    "ryx-brain/docs/body-map.md": "b27e8f4099c00ab6ebd010cca901e6d28c4c41d179850baf80c4bd6d7648ebe2",
    "ryx-brain/docs/checkins.md": "c20f074ee536a89e4d555901906b54835c33c8bd1c1ce892e075e2af5cf5e09b",
    "ryx-brain/docs/envelope-upsell.md": "19a7bccc5ce0bde940bfd1cedaf0ef3f9a3e740d454ce2547e6dbd6a28d6b98e",
    "ryx-brain/docs/event-countdown.md": "fb977fc433f91fe50a12435521bf39a78f8fec24379a56e0f582284724acf05a",
    "ryx-brain/docs/program-marketplace.md": "fb7602f4df3d281dd85126a19a7c4e231e1d64145ac2fa77febcc5ca43929bec",
    "ryx-brain/docs/reports.md": "02ac3731f78c7d622485433c5c163cbb5754f93ce698a122998d89d2585e7294",
    "ryx-brain/docs/sessions.md": "6f52ffc2ce217ae7ce127b198c7dea2b52339614ae9024f695faa4145018a7c3",
    "ryx-brain/docs/shared-athlete-data.md": "e221da34cbad8b890e779ff5961807c558bce2839d81a5b5d0845dcc51512ec1",
    "ryx-brain/docs/todos.md": "d13314ba5019c8b36a838fc96dd94eb1fad68b94add79ee6d7fc862eac6dce7d",
    "ryx-brain/docs/train-live.md": "b73329af0f7d89c977a9819124ffadf7c6700b86a9d0745d2d05181371843056",
    "ryx-brain/package.json": "15a5bbace266e59827fdcb87f3a64022875493b2c8d66e01b26956108faad7cd",
    "ryx-brain/src/accounts.js": "c78307b0732e8a24916e6610cb622d0683e2ffaa8164a693bc92d483166a2fd8",
    "ryx-brain/src/athleteSnapshot.js": "2f63bda7d128e68db8340062997a7b38e42b552534d6c5463c043fd9ea115f15",
    "ryx-brain/src/bodymap.js": "bfb77a82d6b832c89f1d778f96341e62a08cf8801e742addf5f227051e590396",
    "ryx-brain/src/bodymapFormat.js": "33261f032958377bd361c4aab2e8b2444f7bfda12c19d78835f10a80b2ca2127",
    "ryx-brain/src/bodymapRegions.js": "c5e03ed21aee1ea3940f82497d7f37ffefa61e1fa3b21cf7c63784cadb6c9779",
    "ryx-brain/src/buildSystemPrompt.js": "1ae4d7d0fd98aba53231c1559586859c397f4ca16b7df621ad156841cc72305f",
    "ryx-brain/src/cardCoerce.js": "8c171b0b2d17a1f758dbee3ae9b7cf00fe1b9abcb910241f8467ecd9fd7ede52",
    "ryx-brain/src/cardLayout.js": "7dd7ada75e86085ee7d7f987d446197aa99ea7f82ee37f22980495a1601c04d2",
    "ryx-brain/src/chatIntake.js": "ebeae9f43e69396da52c9f83ef338b135918dea6b55fa0f128858bd3010c6a84",
    "ryx-brain/src/checkinFormat.js": "d6db9bd6842b17ac8f2bafb206e55d05cc34e99b45c1002bb21e10be72085ccd",
    "ryx-brain/src/checkins.js": "adc9b1e01a082089c8fa3e53bee02c4db6ca0d178ec5b93a6d0a0add37ea5b34",
    "ryx-brain/src/client.js": "d6f3f3f337592b30e91237ec0862126a92e5a9a478edd87ba58e8676963c94f8",
    "ryx-brain/src/coryxProducts.js": "5a5484b9c81be87729587f050b0fd953905119f7e7117e70469fffea4dba0885",
    "ryx-brain/src/credits.js": "fb6c5dbcfa8929432c28ad4c839179936a100e27e70c0a928cfd6e6b6e6bffbf",
    "ryx-brain/src/directMessages.js": "5fac5245e6abffc1d85907b948a2c1d1a4fa39eafa9fd5f1e69e4dc25c8c2342",
    "ryx-brain/src/envelope.js": "19c48627306e20cabc9bb042a27f5accd0b390b29efe1d9c4e7511576a024152",
    "ryx-brain/src/eval.js": "07c3f94d26a7ebe23bd5ac6bfc92f12debcabc184bde0bb54a50133ad05c110e",
    "ryx-brain/src/evalExerciseMedia.js": "90c4ef1df9626e579cb139b04b9a7e6a027acc37ad5e75d3829f1e7404ed0ab7",
    "ryx-brain/src/evalExerciseMediaNiches.js": "2d389eb47a6f3810599bf76f839994a85bae52b018c64dca0794e557ed47fcb2",
    "ryx-brain/src/evalOpenai.js": "2a74412aa26d90e6bf8efc418158d629e91ebcbd9bcc09bc8d109e4f35a1289b",
    "ryx-brain/src/eventFormat.js": "84b64f9c6dbde988c3db5c95bf1c5eb488de87909d4b938da5e3389f3d631ce6",
    "ryx-brain/src/events.js": "0d071a7ff7559ff60fd2e20394aa5d33e9f1ca4d5903897e87f55ff0520f23c2",
    "ryx-brain/src/exerciseMedia.js": "5a75a4be1ad0c7f3dc1cc4ce35aa6273111d008785bacc9894a3d5720e3557d6",
    "ryx-brain/src/formatCoachReply.js": "fd59de17b77b00f1d3b17efad2051f7e72cd7d1845e9f1639d8fabeb9ffaa9ca",
    "ryx-brain/src/herd.js": "843dbd85e368d438aa8150273736ecc63a4d74b64772e7e39b03e2d324d2cc8f",
    "ryx-brain/src/identity.js": "9d92845f6e1c68d244232e0dfe65f83966018544ef38a1b0e08a6ce9a1c5e54e",
    "ryx-brain/src/identityRoutes.js": "657653eb43b367b3e16f09e4daafbdced908bb07177b23166b6e41b3a58bada3",
    "ryx-brain/src/knowledge/README.md": "13c12a28faab1073743a1d016a2fa285dbb01fe3a4ae934914970e7ddcf28283",
    "ryx-brain/src/knowledge/data/exerciseMediaCatalog.json": "289fee4ae5aa4a47dc34107aae17ca442a779f86f14b0e8328480360a20cc864",
    "ryx-brain/src/knowledge/data/exercises.json": "683a6858bf06018d7db3687a46a0a876bb78d775bae5119861ea8914b90b26e4",
    "ryx-brain/src/knowledge/data/formDemosByWedge.json": "a41d74afb2a2de798a06526d7024b42b058d6c618df729f00ee57f30309e726b",
    "ryx-brain/src/knowledge/data/playbooks.json": "ca24e16706ae1004c0e991fdd4f48c358ac0ea6eda4d1dce76a4ce1fb1c92b8a",
    "ryx-brain/src/knowledge/formDemos.js": "0143a07d73d5864e5f444ed5cd9c07d022edba9462d5a1d8de18828c66e22072",
    "ryx-brain/src/knowledge/nicheMap.js": "ddabb1232c2b55fafe358146c85fd4bba3db4c2d5ad03855c32d4e2de3090b5e",
    "ryx-brain/src/knowledge/retrieve.js": "030b7e1537e783421f6297d883bcc06122101455fe7cd9d7b52eabb833faa3b6",
    "ryx-brain/src/knowledge/wedgeFormat.js": "18f40819a20c17ddd59387ef0097be0e3e9e028792de02eb041655c6bd2418c1",
    "ryx-brain/src/knowledge/wedgeLoader.js": "f1ea761197aac2a0073e56f2ac60cada22a377bd63afffff6cb2ee62b066e81f",
    "ryx-brain/src/knowledge/wedgeRouter.js": "4bb6f8408a077a9e1937646da3cbc04dc8ae4399b9b707d36061c9390e571d7f",
    "ryx-brain/src/labEval.js": "6956bddd0e9313c55b5985219f6abdd9ed0900c3aa477d02464c2b6b49a44f74",
    "ryx-brain/src/labInsights.js": "9aac35f683cdab1d1d1768338217253eb79ddab7915846a4f9c9c3de5856ff8d",
    "ryx-brain/src/labMemory.js": "1964def8dd1dd2043656f892ed2d8b284f250d947566b4e9dd23f75b1d663ac9",
    "ryx-brain/src/labPersonality.js": "d5477409300fc8865f32c4aaceb855086064a29395c88779c107bd1bdc6f5822",
    "ryx-brain/src/labScenarios.js": "2c144fb87749580f68661f1a41f1ccfbfb9081e865a0b53af6aee5cb6b114b1b",
    "ryx-brain/src/labSessions.js": "2ab73aff4b48c765f1bb47dd4f3b9162d0c208cbc54d6f1a75e892ea46220a29",
    "ryx-brain/src/liveEvents.js": "73fecee405644ec46a2305874160f986c14234a47c2b872669b36a7b8bd79b72",
    "ryx-brain/src/llmProvider.js": "f0c0bb7d253265e7b45a72eb00c044225c071df5c3c1d0f792238bb847299ce9",
    "ryx-brain/src/openaiClient.js": "4417a87080dc21a147daad6afcb939cd29b4e77655a00526fac93e01fe8f127d",
    "ryx-brain/src/openaiRun.js": "b787ab9aeeeb3b4fb20705b5bf45fcda5e87e5f7934e2bf54408d98494bef3ee",
    "ryx-brain/src/printPrompt.js": "c53dd522626c3475cf4e234fe9dfc176787c6216f4c2dfa5da41ee922357af9a",
    "ryx-brain/src/profileFunnel.js": "49349b54611a7cc21132e341c953eca3de98c8b845fc01e689da6d5fed16ba05",
    "ryx-brain/src/programCatalog.js": "8afecaf12f1abfbb0947da2a21891ff0f95b5d35d33981e3d5229f19c9c9796d",
    "ryx-brain/src/programFormat.js": "3b206ab6d8964d6177b2d53ea11752222360536843ec64679eef48b65f31e5a8",
    "ryx-brain/src/programs.js": "618565859f956ba5cb7869e6fe463b32019a305c447b1077f9d245c41b6b4bf4",
    "ryx-brain/src/prompts/athlete.js": "8ac6cbf99ea02fdaab520377a36e6d5e9055a2377e1be7c072641f2016fb3418",
    "ryx-brain/src/prompts/core.js": "ae4688eb033dc7866f014f6f7a352abd1f31e26b57c7039cb6cd57862b777b2e",
    "ryx-brain/src/prompts/trainer.js": "b061db716372836abcf73e11969dc4b9fe18f8b4bbe9c01dd518b270f40573b3",
    "ryx-brain/src/replyGuards.js": "320f035eb7663288a805ff6779d3f98263e042959c35a01e5ae20952a8628dd6",
    "ryx-brain/src/reports.js": "cd155b873eabd84f379aa10114c078a5f45fd03d15467180c741e80264941de0",
    "ryx-brain/src/runChat.js": "0762eb989846dc1295c6df679250fdc642ca579c0bcd05a015fb903c068621fc",
    "ryx-brain/src/scenarios/athlete.json": "758ad1c0b69c6a7316422108e9d9a8edf7d6456e68ac80a8d725f229a7dee8aa",
    "ryx-brain/src/scenarios/trainer.json": "663d44a63e36e1a22a737936c8341df29d91cd9342e5bbf46cdc7a6a90af9006",
    "ryx-brain/src/server.js": "68165275a3ba061262e678386fddf4dc2f37f03307abcf2133864bcf05544b03",
    "ryx-brain/src/sessionFormat.js": "cc43b51530f1633f7ac86f9a36c6e1ff614bab123adf70d3ab93d5d7d2b933c8",
    "ryx-brain/src/sessions.js": "d40e05d384234ec55d27328ca10e2746ac14a1d5343815dc98685f7dd971ba18",
    "ryx-brain/src/todoFormat.js": "ac53302b58cf8b0e6d57e24c4ce89962a33b044844f485de5744e4188e561176",
    "ryx-brain/src/todos.js": "74a87271bfaf30e727e1e22d1900050706714eb31bb4b0addb0dfbda69fc9da7",
    "ryx-brain/test/messaging.test.js": "2d1746730b125bb257b7eadcce1dc7d02067b4a9d35fb1bdfbb03cc39a32199f",
    "ryx-brain/test/shared-ryx.test.js": "8ca69d880cbe94d0a7a28bd83d935fb3bba01685036be44876101d3fbdfdcf56",
    "ryx-landing/src/components/cards/RyxContentCard.jsx": "0aa6d1278ee6ab4f74172c380f89292c098161de1b812fb6735ed3ae3233fb6a",
    "ryx-landing/src/lib/cardLayout.js": "9dd0936e493aae7ac7d793f71f654ca96cc93059f599335d42b40574b7db375b",
    "ryx-landing/src/lib/identityApi.js": "aaf323acec39514b6255ac9a4e1d592fc380ea1e9460fc6766c79cbb1f407143",
    "package.json": "705665215b05cd5cf8dd1c9acc2131751416089060fa6e2ac7624b04053854fd",
    "ryx-landing/src/App.jsx": "d68f1e81e5ac14e3f873e5addd39eb29a346e2ea04edb918137de7406c7fbb42",
    "web/src/lib/brainHealth.js": "1422cf8634417cd70f168787bbc46f627394f23616778a285d67e29b6bf59025",
    "web/src/pages/CoachPage.jsx": "8bdfa87d09595a9bf9b829824130eff27cdb4bbcec28726c22b73a94feb6b57f",
    "scripts/dev.mjs": "7d1e63b593e2d8e7d9a3d4579fc9465f6a379c97ef1341b347168aab478ca5e1"
  },
  "protectedHashes": {
    "MIGRATION_REVIEW.md": "3412c0cbb24b0dc1c8d939bd700c734fd50910a86fcabaece344417e26f27106",
    "MIGRATION_MAP.md": "342ea213be203c80a52b1864168f957392eec3d8d157a8a67ab42ad2043c092c",
    "10_Releases/RYX_Brain_v0.1.0.md": "0ab681cd98d5f1ca29c2fef37fbbc19725f4f08c78d788a61479ffb528d4860d"
  },
  "modifiedFiles": [
    "00_HOME.md",
    "00_README.md",
    "01_Core/Brain_Architecture.md",
    "01_Core/Output_and_Card_Behaviour.md",
    "01_Core/Personality_and_Voice.md",
    "01_Core/RYX_Identity.md",
    "01_Core/Response_Principles.md",
    "02_Roles/Athlete/Athlete_Free.md",
    "02_Roles/Athlete/Athlete_Pro.md",
    "02_Roles/Athlete/Athlete_Role.md",
    "02_Roles/Athlete/Companion_Mode.md",
    "02_Roles/Athlete/Solo_Mode.md",
    "02_Roles/Trainer/Trainer_Approval_Model.md",
    "02_Roles/Trainer/Trainer_Free.md",
    "02_Roles/Trainer/Trainer_Outputs.md",
    "02_Roles/Trainer/Trainer_Pro.md",
    "02_Roles/Trainer/Trainer_Role.md",
    "03_Policies/Credit_and_Tier_Rules.md",
    "03_Policies/Crisis_Handling.md",
    "03_Policies/Data_Access.md",
    "03_Policies/Deterministic_Reply_Guards.md",
    "03_Policies/Memory_Policy.md",
    "03_Policies/Pain_and_Injury.md",
    "03_Policies/RYX_Boundaries.md",
    "03_Policies/Referral_Rules.md",
    "03_Policies/Safety.md",
    "03_Policies/Trainer_Athlete_Access.md",
    "04_Domains/Athlete_Profile.md",
    "04_Domains/Body_Map.md",
    "04_Domains/Body_Region_Catalog.md",
    "04_Domains/Check_Ins.md",
    "04_Domains/Direct_Messaging.md",
    "04_Domains/Events.md",
    "04_Domains/Goals.md",
    "04_Domains/Nutrition_Guidance.md",
    "04_Domains/Programs.md",
    "04_Domains/Progress_and_Adherence.md",
    "04_Domains/Todos_and_Habits.md",
    "04_Domains/Training_Sessions.md",
    "05_Knowledge/Exercise_Library.md",
    "05_Knowledge/Exercise_Media_Catalog.md",
    "05_Knowledge/Exercise_Media_Rules.md",
    "05_Knowledge/Fitness/Bodybuilding.md",
    "05_Knowledge/Fitness/Calisthenics.md",
    "05_Knowledge/Fitness/CrossFit.md",
    "05_Knowledge/Fitness/General.md",
    "05_Knowledge/Fitness/Powerlifting.md",
    "05_Knowledge/Form_Demos_By_Wedge.md",
    "05_Knowledge/Knowledge_System.md",
    "05_Knowledge/Legacy_Playbooks.md",
    "05_Knowledge/Marketplace_Program_Templates.md",
    "05_Knowledge/Sports/Basketball.md",
    "05_Knowledge/Sports/Combat.md",
    "05_Knowledge/Sports/Football.md",
    "05_Knowledge/Sports/Golf.md",
    "05_Knowledge/Sports/Padel.md",
    "05_Knowledge/Sports/Swimming.md",
    "05_Knowledge/Sports/Tennis.md",
    "05_Knowledge/Wedge_Index.md",
    "05_Knowledge/Wedge_Routing_Reference.md",
    "05_Knowledge/Wedge_Schema.md",
    "05_Knowledge/Wellness/Rehab_and_Therapy.md",
    "05_Knowledge/Wellness/Yoga_and_Mind_Body.md",
    "06_Tools/Adapt_Purchased_Program.md",
    "06_Tools/Add_Todo.md",
    "06_Tools/Approve_Program_Draft.md",
    "06_Tools/Browse_Programs.md",
    "06_Tools/Change_Plan_and_Credits.md",
    "06_Tools/Direct_Messaging_Capability.md",
    "06_Tools/Draft_Message.md",
    "06_Tools/Draft_Program.md",
    "06_Tools/Get_Account.md",
    "06_Tools/Get_Athlete_Profile.md",
    "06_Tools/Get_Athlete_Snapshot.md",
    "06_Tools/Get_Body_Map.md",
    "06_Tools/Get_Check_Ins.md",
    "06_Tools/Get_Connected_Clients.md",
    "06_Tools/Get_Current_Program.md",
    "06_Tools/Get_Events.md",
    "06_Tools/Get_Exercise_Catalog.md",
    "06_Tools/Get_Program_Library.md",
    "06_Tools/Get_Todos.md",
    "06_Tools/Get_Training_Sessions.md",
    "06_Tools/Log_Body_Report.md",
    "06_Tools/Manage_Events.md",
    "06_Tools/Manage_Trainer_Connection.md",
    "06_Tools/Manage_Training_Sessions.md",
    "06_Tools/Purchase_Program.md",
    "06_Tools/README.md",
    "06_Tools/Report_Conversation.md",
    "06_Tools/Retrieve_Knowledge.md",
    "06_Tools/Save_Check_In.md",
    "06_Tools/Update_Assigned_Program.md",
    "06_Tools/Update_Athlete_Profile.md",
    "06_Tools/Update_or_Delete_Todo.md",
    "07_Workflows/Athlete_Check_In.md",
    "07_Workflows/Athlete_Onboarding.md",
    "07_Workflows/Body_Map_Response.md",
    "07_Workflows/Daily_Training.md",
    "07_Workflows/Intake_and_Journey_Rules.md",
    "07_Workflows/Program_Adjustment.md",
    "07_Workflows/Program_Generation.md",
    "07_Workflows/Trainer_Check_In_Analysis.md",
    "07_Workflows/Trainer_Client_Brief.md",
    "07_Workflows/Trainer_Client_Message_Draft.md",
    "07_Workflows/Trainer_Program_Draft.md",
    "08_Evals/Athlete_Scenarios.md",
    "08_Evals/Coverage.md",
    "08_Evals/Eval_System.md",
    "08_Evals/Exercise_Media_Scenarios.md",
    "08_Evals/Trainer_Scenarios.md",
    "09_Runtime_Context/Athlete_Snapshot.md",
    "09_Runtime_Context/Data_Boundary.md",
    "09_Runtime_Context/Known_Context.md",
    "09_Runtime_Context/SESSION.md",
    "99_Archive/Archive_Index.md"
  ],
  "createdFiles": [
    "03_Policies/Free_Pro_Entitlements.md",
    "10_Releases/RYX_Brain_v0.2.0.md",
    "99_Archive/Canonicalization_Audit.md",
    "99_Archive/Canonicalization_Recipe.md",
    "99_Archive/RYX_Brain_v0.1.0_Notes_Snapshot.md",
    "CANONICALIZATION_REVIEW.md",
    "RYX_BRAIN_DECISIONS.md"
  ],
  "sourceChangesSinceMigration": [],
  "limitations": [
    "Offline structure/content/integrity and documented-rule checks; not proof current runtime satisfies v0.2.0",
    "No live model, full-pipeline or external source freshness tests run",
    "No secret files, runtime records or databases opened",
    "All writes confined to CORYX-RYX-Brain"
  ]
}
~~~

[[CANONICALIZATION_REVIEW]]
