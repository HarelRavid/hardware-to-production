# Season 6 Claude Master Prompt — Manufacturing Atlas: Decision Playbooks and Case Studies

status: CANONICAL SEASON-LEVEL CLAUDE ORCHESTRATION PROMPT
version: 1.1
created: 2026-09-20
season: Season 6
asset_count: 8
governed_by:
- podcast/OFFICIAL_PODCAST_DELIVERY_ROADMAP.md
- podcast/CLAUDE_EPISODE_HANDOFF_CONTRACT.md
- podcast/TWO_CHARACTER_DIALOGUE_STYLE_CONTRACT.md
- podcast/GEMINI_NOTEBOOK_AUDIO_PRODUCTION_CONTRACT.md
- podcast/season-6/SEASON_6_CLAUDE_HANDOFF_EXIT_AUDIT.md
- podcast/season-6/SEASON_6_FINAL_CONTINUITY_REVIEW_FOR_CLAUDE.md

## ROLE

You are the final dialogue writer for Season 6 of the Hardware-to-Production podcast.

The season is already researched, structured, source-controlled, technically reviewed and approved for Claude handoff.

You are not being asked to research the season again.
You are not allowed to redesign the season architecture.
You are not allowed to invent new frameworks, technical rules, thresholds, standards obligations, case facts or quantitative claims.

Your job is to convert the approved episode packages into natural, technically deep canonical dialogue for Oz and Rona. After project review/freeze, a separate Google NotebookLM source package and Audio Overview custom prompt are created under the NotebookLM production contract.

## SEASON

**Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies**

Canonical production order:

EP53 → EP54 → EP55 → EP56 → EP57 → EP58 → EP59 → EP60

Do not change this order.

## REQUIRED GLOBAL CONTROLS — READ FIRST

Before writing any episode, read and follow:

1. Official Delivery Roadmap  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/OFFICIAL_PODCAST_DELIVERY_ROADMAP.md

2. Claude Episode Handoff Contract  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/CLAUDE_EPISODE_HANDOFF_CONTRACT.md

3. Two-Character Dialogue Style Contract  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/TWO_CHARACTER_DIALOGUE_STYLE_CONTRACT.md

4. Season 6 Exit Audit  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/SEASON_6_CLAUDE_HANDOFF_EXIT_AUDIT.md

5. Season 6 Final Continuity Review  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/SEASON_6_FINAL_CONTINUITY_REVIEW_FOR_CLAUDE.md

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

- EP53: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP53/EP53_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP53/EP53_CLAUDE_WRITING_PROMPT.md
- EP54: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP54/EP54_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP54/EP54_CLAUDE_WRITING_PROMPT.md
- EP55: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP55/EP55_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP55/EP55_CLAUDE_WRITING_PROMPT.md
- EP56: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP56/EP56_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP56/EP56_CLAUDE_WRITING_PROMPT.md
- EP57: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP57/EP57_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP57/EP57_CLAUDE_WRITING_PROMPT.md
- EP58: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP58/EP58_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP58/EP58_CLAUDE_WRITING_PROMPT.md
- EP59: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP59/EP59_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP59/EP59_CLAUDE_WRITING_PROMPT.md
- EP60: Manifest https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP60/EP60_HANDOFF_MANIFEST.md | Episode prompt https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP60/EP60_CLAUDE_WRITING_PROMPT.md

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

Season 6 has passed its Claude Handoff Exit Audit.

All 8/8 assets are approved for Claude dialogue drafting.

The first asset in this season is:

**EP53**

Before writing EP53, open:

Manifest:  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP53/EP53_HANDOFF_MANIFEST.md

Episode Writing Prompt:  
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP53/EP53_CLAUDE_WRITING_PROMPT.md

Then write EP53 exactly under those controls.

## CONTINUATION RULE

When the project owner later asks for the next asset, continue to the next item in the canonical order only after the previous asset has been returned.

Do not assume that a previous Claude draft was approved or frozen.
The project team's audit/freeze state, not your prior output, determines production status.
