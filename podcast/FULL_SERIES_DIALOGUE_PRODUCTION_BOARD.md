# Full-Series Dialogue Production Board

status: ACTIVE — CLAUDE DIALOGUE PRODUCTION
created: 2026-09-19
preparation_baseline: 68 / 68 CLAUDE HANDOFF READY
governed_by:
- podcast/OFFICIAL_PODCAST_DELIVERY_ROADMAP.md
- podcast/CLAUDE_EPISODE_HANDOFF_CONTRACT.md
- podcast/TWO_CHARACTER_DIALOGUE_STYLE_CONTRACT.md
- podcast/FULL_SERIES_CLAUDE_HANDOFF_EXIT_AUDIT.md

## 1. Purpose

Track the downstream production lane after completion of all research/source/technical/handoff preparation.

This board does not reopen episode architecture.

For each asset:

CLAUDE HANDOFF READY
→ CLAUDE OZ/RONA DIALOGUE DRAFT
→ CLAIM / TECHNICAL AUDIT
→ QUANTITATIVE / CASE / LEGAL AUDIT where applicable
→ TWO-CHARACTER EDITORIAL REVIEW
→ SOURCE-CURRENTNESS RECHECK
→ FINAL DIALOGUE FREEZE
→ NOTEBOOKLM SOURCE + CUSTOM PROMPT PACKAGE
→ NOTEBOOKLM AUDIO OVERVIEW GENERATED
→ AUDIO QA
→ PODCAST READY

## 2. Current program state

Production architecture:
68 / 68 complete.

Claude handoff:
68 / 68 complete.

Final dialogue frozen:
0 / 68.

NotebookLM production packages:
0 / 68.

Audio QA complete:
0 / 68.

Podcast Ready:
0 / 68.

## 3. Canonical production order

### Season 1
A1 → A2 → A3 → A4 → A5 → A6 → A7 → A8 → EP01 → EP02 → EP03 → EP04 → EP05 → EP06 → EP07 → EP08 → EP09 → EP10

### Season 2
EP11 → EP12 → EP13 → EP14 → EP15 → EP16 → EP17 → EP18 → EP19

### Season 3
EP20 → EP21 → EP22 → EP23 → EP24 → EP25 → EP26 → EP27 → EP28 → EP29 → EP30 → EP31

### Season 4
EP32 → EP33 → EP34 → EP35 → EP36 → EP37 → EP38 → EP39 → EP40

### Season 5
EP41 → EP42 → EP43 → EP44 → EP45 → EP46 → EP47 → EP48 → EP49 → EP50 → EP51 → EP52

### Season 6
EP53 → EP54 → EP55 → EP56 → EP57 → EP58 → EP59 → EP60

## 4. Season-level Claude master prompts

Use the season master prompt as the session-level orchestration entry point, then use each asset's Handoff Manifest and episode-specific Claude Writing Prompt as the immediate authority.

- Season 1: podcast/season-1/SEASON_1_CLAUDE_MASTER_PROMPT.md
- Season 2: podcast/season-2/SEASON_2_CLAUDE_MASTER_PROMPT.md
- Season 3: podcast/season-3/SEASON_3_CLAUDE_MASTER_PROMPT.md
- Season 4: podcast/season-4/SEASON_4_CLAUDE_MASTER_PROMPT.md
- Season 5: podcast/season-5/SEASON_5_CLAUDE_MASTER_PROMPT.md
- Season 6: podcast/season-6/SEASON_6_CLAUDE_MASTER_PROMPT.md

Rule:
the season master prompt controls order and shared writing behavior only. It never overrides an episode Claim Lock, Source Register, Technical Review, Script Outline, Handoff Manifest or episode-specific Claude Writing Prompt.

## 5. Active asset

**A1 — From an Idea to Engineering Requirements**

Status:
**NEXT — SEND TO CLAUDE**

Prompt:
podcast/season-1/claude-handoff/A1/A1_CLAUDE_WRITING_PROMPT.md

Manifest:
podcast/season-1/claude-handoff/A1/A1_HANDOFF_MANIFEST.md

Existing internal draft:
podcast/season-1/A1_SCRIPT_DRAFT_V1.md

Authority rule:
the existing draft is reference only; Claim Lock / Source Register / Technical Review / Outline remain higher authority.

## 6. Per-episode review checklist after Claude returns a draft

### Gate D1 — Dialogue format
- canonical hosts are Oz and Rona;
- output labels are `OZ:` / `RONA:`;
- both hosts technically substantive;
- Rona is a young engineer, not a naive student;
- Oz is a veteran engineer, not the sole technical authority;
- no citation/URL read aloud;
- no internal IDs spoken;
- production notes separated.

### Gate D2 — Claim audit
- every consequential statement inside locked claim set;
- no new framework name;
- no unsourced “typical” rule;
- no guidance strengthened into requirement.

### Gate D3 — Quantitative / case audit
Where applicable:
- arithmetic independently rechecked;
- units/assumptions preserved;
- case populations/dates/configurations/attribution preserved;
- legal/current-status language rechecked.

### Gate D4 — Season editorial review
- no adjacent-episode duplication;
- callbacks concise;
- listener tool executed;
- practical action clear;
- next handoff correct.

### Gate D5 — Source notes finalization
Replace skeleton with only sources actually used by final spoken dialogue.

### Gate D6 — Final dialogue freeze
Assign final version/status.
After freeze, any consequential change requires targeted claim/source review.

### Gate D7 — Google NotebookLM package
Build under `podcast/GEMINI_NOTEBOOK_AUDIO_PRODUCTION_CONTRACT.md`.

Include:
- frozen final dialogue using `OZ:` / `RONA:`;
- clean NotebookLM source document;
- episode-specific NotebookLM custom Audio Overview prompt;
- pronunciation/acronym notes where relevant;
- episode summary / must-cover arc;
- source-vs-synthesis and forbidden-overclaim boundaries;
- tone, audience, pacing and output-language guidance.

Do not assume NotebookLM will read the final dialogue verbatim.

### Gate D8 — Audio QA
Check:
- omissions;
- pronunciation;
- Oz/Rona identity and role consistency;
- no role reversal that changes meaning;
- Rona remains technically capable rather than a naive student;
- technical meaning;
- no invented/fabricated statements;
- rerender if needed.

## 7. Status vocabulary

- NEXT — SEND TO CLAUDE
- CLAUDE DRAFT RECEIVED
- TECHNICAL REVIEW
- EDITORIAL REVIEW
- SOURCE RECHECK
- FINAL DIALOGUE FROZEN
- NOTEBOOKLM SOURCE PACKAGE READY
- NOTEBOOKLM AUDIO OVERVIEW GENERATED
- AUDIO QA PASS
- PODCAST READY

## 8. Program rule

Do not start a new broad research wave during dialogue production.

Open targeted source work only when:
- Claude introduces a needed consequential claim not already locked;
- a current standard/regulatory/case source changes;
- technical review exposes a contradiction or missing applicability condition.

Otherwise:
use the prepared handoff package and keep moving in canonical order.
