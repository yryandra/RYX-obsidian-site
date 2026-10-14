---
id: "ryx.navigation.readme"
title: "Open and Use the RYX Brain"
type: "core"
status: "reference_only"
version: "0.2.0"
applies_to:
  - "athlete"
  - "trainer"
source_files:
  - "ryx-brain/src/buildSystemPrompt.js"
  - "ryx-brain/src/prompts/core.js"
  - "CORYX-RYX-Brain/RYX_BRAIN_DECISIONS.md"
last_reviewed: "2026-10-14"
canonical: false
---

# Open and use the RYX Brain

## First-time setup on Windows

1. Visit [Obsidian's official download page](https://obsidian.md/download), choose **Download for Windows**, run the downloaded installer and follow its prompts.
2. Launch Obsidian. In the vault manager, click **Open** beside **Open folder as vault**. If you already have a vault open, use **Vault profile → Manage Vaults...** to get there. [Official vault instructions](https://help.obsidian.md/Files%2Band%2Bfolders/Manage%2Bvaults).
3. Select **C:\Users\user\Downloads\HERD-R.Y.X\CORYX-RYX-Brain** and click **Open**. Select the folder itself, not a single Markdown file.
4. In the left file list, click **00_HOME.md**. Follow its links to explore.

No community plugin, paid Sync service, account, or proprietary document format is required to use these Markdown notes locally. Obsidian may create its own settings folder when you open the vault.

## Finding your way

- Click a note link to open it. Use the left file list to browse folders.
- Press Ctrl+O and type a note name to open it quickly. Search can find a rule or claim ID across notes.
- Collapse long headings in knowledge notes. Their first sections explain where to start; the Structured source block preserves exact machine-readable fields.
- Properties at the top show stable ID, type, status, version, applicable roles, sources and review date. last_reviewed is the migration audit date; knowledge_verified_through keeps the original source verification date.
- Every production note ends with source references and a Home link. Source paths are relative to the repository and remain implementation references outside the standalone vault.

## Folder guide

01_Core identity/voice/output/architecture; 02_Roles Athlete/Trainer with tier/mode; 03_Policies safety/access/memory/guards/credits; 04_Domains what app data means; 05_Knowledge complete curated knowledge; 06_Tools actual capability contracts; 07_Workflows how existing rules work together; 08_Evals reference acceptance checks; 09_Runtime_Context schema/interpretation; 10_Releases active-note manifest. 90_Drafts/99_Archive are non-production.



## Reviewed candidate and priority

[[Brain_Architecture#Global instruction precedence]] is the canonical instruction order. [[Data_Boundary#Data truth precedence]] keeps facts separate from inference. [[RYX_BRAIN_DECISIONS]] records approved H01–H12 decisions and rule ownership.

Migration baseline: [[RYX_Brain_v0.1.0]]. Reviewed candidate: [[RYX_Brain_v0.2.0]]. Runtime status: NOT YET INTEGRATED.

The unchanged migration manifest is historical. Its linked paths now hold reviewed notes; exact original note contents/frontmatter remain in [[RYX_Brain_v0.1.0_Notes_Snapshot]]. Current active notes are intended canonical brain rules, not a statement of runtime implementation. reference_only/legacy/review admin material is excluded from the candidate.

Read [[CANONICALIZATION_REVIEW]] before future runtime implementation. No runtime loader or deployment is included.

## Source reference

- `ryx-brain/src/buildSystemPrompt.js`
- `ryx-brain/src/prompts/core.js`

Decision authority: [[RYX_BRAIN_DECISIONS]]. Existing source mappings remain in the unchanged [[MIGRATION_MAP]].

[[00_HOME|Back to the RYX Brain home]]
