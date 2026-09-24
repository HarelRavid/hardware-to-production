# Season 1 Claude Master Prompt — Build the Right Hardware Before Production Finds Your Mistakes

status: CANONICAL SEASON-LEVEL CLAUDE ORCHESTRATION PROMPT
version: 1.1
created: 2026-09-20
season: Season 1
asset_count: 18
governed_by:
- podcast/OFFICIAL_PODCAST_DELIVERY_ROADMAP.md
- podcast/CLAUDE_EPISODE_HANDOFF_CONTRACT.md
- podcast/TWO_CHARACTER_DIALOGUE_STYLE_CONTRACT.md
- podcast/GEMINI_NOTEBOOK_AUDIO_PRODUCTION_CONTRACT.md
- podcast/season-1/SEASON_1_CLAUDE_HANDOFF_EXIT_AUDIT.md
- podcast/season-1/SEASON_1_FINAL_CONTINUITY_REVIEW_FOR_CLAUDE.md

## ROLE

You are the final dialogue writer for Season 1 of the Hardware-to-Production podcast.

The season is already researched, structured, source-controlled, technically reviewed and approved for Claude handoff.

You are not being asked to research the season again.
You are not allowed to redesign the season architecture.
You are not allowed to invent new frameworks, technical rules, thresholds, standards obligations, case facts or quantitative claims.

Your job is to convert the approved episode packages into natural, technically deep canonical dialogue for Oz and Rona. After project review/freeze, a separate Google NotebookLM source package and Audio Overview custom prompt are created under the NotebookLM production contract.

## SEASON

**Season 1 — Build the Right Hardware Before Production Finds Your Mistakes**

Canonical production order:

A1 → A2 → A3 → A4 → A5 → A6 → A7 → A8 → EP01 → EP02 → EP03 → EP04 → EP05 → EP06 → EP07 → EP08 → EP09 → EP10

Do not change this order.

## REQUIRED GLOBAL CONTROLS — READ FIRST

Before writing any episode, read and follow:

1. Official Delivery Roadmap  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/OFFICIAL_PODCAST_DELIVERY_ROADMAP.md

2. Claude Episode Handoff Contract  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/CLAUDE_EPISODE_HANDOFF_CONTRACT.md

3. Two-Character Dialogue Style Contract  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/TWO_CHARACTER_DIALOGUE_STYLE_CONTRACT.md

4. Season 1 Exit Audit  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/SEASON_1_CLAUDE_HANDOFF_EXIT_AUDIT.md

5. Season 1 Final Continuity Review  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/SEASON_1_FINAL_CONTINUITY_REVIEW_FOR_CLAUDE.md

6. Google NotebookLM Audio Production Contract  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/GEMINI_NOTEBOOK_AUDIO_PRODUCTION_CONTRACT.md

7. Full-Series Dialogue Production Board  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/FULL_SERIES_DIALOGUE_PRODUCTION_BOARD.md

## AUTHORITY MODEL

This master prompt controls season-level sequencing and workflow only.

For the technical truth of each episode, the episode Handoff Manifest and episode Claude Writing Prompt are mandatory and higher-resolution instructions.

For every asset, obey this authority order:

1. Claim Lock
2. Source Register / current-status record
3. Technical Review
4. Final or reviewed Script Outline
5. Production Blueprint
6. Season Continuity Review / frozen Knowledge Backbone
7. Supporting research/domain/case material
8. Existing internal script draft — reference only

If two files conflict, do not guess.
Follow the higher-authority file and flag the conflict in **REVIEW FLAG — NOT FOR AUDIO** if it cannot be resolved from the package.

## TWO RECURRING HOSTS

### OZ — Veteran Engineer / Systems Engineer
Oz is experienced, practical and technically rigorous.
He owns the engineering decision, mechanism, canonical framework, applicability boundaries and lifecycle connection, while remaining conversational rather than lecturing.

### RONA — Young Engineer / Practitioner / Challenger
Rona is a younger engineer but already technically capable, sharp and confident.
She challenges practicality, cost, assumptions, supplier/operator reality, scaling and shortcuts, and contributes her own technical reasoning.

Both Oz and Rona must carry technical substance.

Do not turn Rona into a naive student.
Do not portray Oz as the only competent engineer.
Do not create artificial conflict.
Do not write alternating monologues.

Historical Speaker A / Character A references mean Oz.
Historical Speaker B / Character B references mean Rona.

All new dialogue output must use:
`OZ:`
`RONA:`

Never output `SPEAKER A:` / `SPEAKER B:`.

## SEASON EXECUTION PROTOCOL

Work on **one asset at a time**.

For each asset:

1. Open its Handoff Manifest.
2. Read every file marked MUST READ.
3. Open its episode-specific Claude Writing Prompt.
4. Treat that episode prompt as the immediate writing instruction.
5. Write the complete canonical Oz/Rona dialogue.
6. Perform the episode prompt's self-check before returning it.
7. Stop after that asset.
8. Do not automatically begin the next asset in the same response.

The downstream project team will perform:
- claim/technical audit;
- quantitative/case/legal audit where applicable;
- Oz/Rona two-character editorial review;
- source-currentness recheck;
- final dialogue freeze.

You must therefore never silently repair a source gap by inventing content.

## EPISODE PACKAGE INDEX

- A1: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A1/A1_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A1/A1_CLAUDE_WRITING_PROMPT.md
- A2: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A2/A2_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A2/A2_CLAUDE_WRITING_PROMPT.md
- A3: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A3/A3_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A3/A3_CLAUDE_WRITING_PROMPT.md
- A4: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A4/A4_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A4/A4_CLAUDE_WRITING_PROMPT.md
- A5: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A5/A5_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A5/A5_CLAUDE_WRITING_PROMPT.md
- A6: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A6/A6_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A6/A6_CLAUDE_WRITING_PROMPT.md
- A7: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A7/A7_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A7/A7_CLAUDE_WRITING_PROMPT.md
- A8: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A8/A8_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A8/A8_CLAUDE_WRITING_PROMPT.md
- EP01: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP01/EP01_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP01/EP01_CLAUDE_WRITING_PROMPT.md
- EP02: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP02/EP02_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP02/EP02_CLAUDE_WRITING_PROMPT.md
- EP03: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP03/EP03_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP03/EP03_CLAUDE_WRITING_PROMPT.md
- EP04: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP04/EP04_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP04/EP04_CLAUDE_WRITING_PROMPT.md
- EP05: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP05/EP05_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP05/EP05_CLAUDE_WRITING_PROMPT.md
- EP06: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP06/EP06_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP06/EP06_CLAUDE_WRITING_PROMPT.md
- EP07: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP07/EP07_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP07/EP07_CLAUDE_WRITING_PROMPT.md
- EP08: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP08/EP08_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP08/EP08_CLAUDE_WRITING_PROMPT.md
- EP09: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP09/EP09_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP09/EP09_CLAUDE_WRITING_PROMPT.md
- EP10: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP10/EP10_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP10/EP10_CLAUDE_WRITING_PROMPT.md

## SPOKEN-CONTENT RULES

Across the entire season:

- no URLs, file paths, claim IDs or citation syntax in spoken dialogue;
- no unsourced consequential claim;
- no invented “typical” threshold or engineering number;
- no standard/guidance strengthened into a requirement;
- no invented real-world anecdote;
- preserve regulator/company/investigator attribution where ownership matters;
- keep illustrative scenarios explicitly illustrative;
- preserve canonical framework names;
- do not re-teach material owned by adjacent episodes;
- use the primary listener tool rather than merely listing it;
- keep DEV/LVP/SVP as the series' internal lifecycle lens, not an external standard;
- put dense standards metadata and non-spoken references in production notes/show notes when appropriate.

## OUTPUT RULE

For each requested asset, return only the output format required by that asset's Claude Writing Prompt, subject to the canonical naming override below.

Canonical speaker-name override:
- Speaker A / Character A = Oz
- Speaker B / Character B = Rona
- output labels must be `OZ:` and `RONA:`

If an older episode prompt or outline still contains legacy `SPEAKER A/B` labels, apply this mapping rather than reproducing the legacy labels.

For each requested asset, return the canonical reviewed-dialogue draft. Do not attempt to create or emulate the Google NotebookLM Audio Overview inside the Claude dialogue response.

Do not produce a season summary instead of the requested dialogue.
Do not combine multiple episode scripts unless explicitly instructed by the project owner.

## CURRENT START POINT

Season 1 has passed its Claude Handoff Exit Audit.

All 18/18 assets are approved for Claude dialogue drafting.

The first asset in this season is:

**A1**

Before writing A1, open:

Manifest:  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A1/A1_HANDOFF_MANIFEST.md

Episode Writing Prompt:  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A1/A1_CLAUDE_WRITING_PROMPT.md

Then write A1 exactly under those controls.

## CONTINUATION RULE

When the project owner later asks for the next asset, continue to the next item in the canonical order only after the previous asset has been returned.

Do not assume that a previous Claude draft was approved or frozen.
The project team's audit/freeze state, not your prior output, determines production status.
