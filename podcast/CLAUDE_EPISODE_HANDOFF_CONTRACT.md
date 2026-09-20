# Claude Episode Handoff Contract — Two-Character Podcast

status: CANONICAL SUPPORTING CONTRACT
version: 2.0
created: 2026-09-19
updated: 2026-09-20
governed_by: podcast/OFFICIAL_PODCAST_DELIVERY_ROADMAP.md

## Purpose

Define the exact minimum package required before an episode may be handed to Claude to write the final two-character podcast dialogue.

## Handoff status

Use:
- HANDOFF BLOCKED
- HANDOFF IN REVIEW
- CLAUDE HANDOFF READY

Only CLAUDE HANDOFF READY episodes may be sent for final dialogue writing.

## Required linked inputs

Every episode prompt must link:
1. Production Blueprint
2. Research/Foundation/Domain pack(s)
3. Source Register
4. Claim Lock
5. Technical Review
6. Quantitative check record where relevant
7. Case Evidence Pack where relevant
8. Script Outline
9. Source Notes / source-note skeleton
10. Season continuity notes
11. Relevant canonical framework source
12. Existing internal full draft if one exists — reference only

## Authority hierarchy for Claude

Claude must treat sources in this order:

1. Claim Lock / Source Register / current-status records
2. Technical Review guards
3. Production Blueprint / Script Outline
4. Canonical frameworks / Knowledge Backbone
5. Research packs / domain material
6. Existing full draft — editorial reference only

If an older draft conflicts with the Claim Lock or Technical Review, the older draft loses.

## Canonical two-character hosts

### OZ — Veteran Engineer / Systems Engineer
Owns structure, definitions, framework, lifecycle logic and experienced engineering context.

### RONA — Young Engineer / Practitioner / Challenger
Challenges assumptions, asks practical questions, runs examples, exposes common mistakes and contributes her own technical reasoning.

Both hosts must carry technical substance.

Historical Speaker A / Character A references map to Oz.
Historical Speaker B / Character B references map to Rona.

All new Claude dialogue output must use:
- `OZ:`
- `RONA:`

Do not return `SPEAKER A:` / `SPEAKER B:` labels.

## Prompt output requirement

Claude must output:
- final two-character canonical dialogue;
- canonical host labels `OZ:` and `RONA:`;
- no URLs/citations read aloud;
- no internal claim IDs spoken aloud;
- no markdown tables in dialogue;
- no fabricated real-world anecdotes;
- no unsourced consequential claims;
- no new framework names where canonical ones exist;
- natural attributions where a regulator/company/investigation owns a fact.

## Mandatory self-check

Before completing the draft Claude must verify:
- every consequential claim is inside the locked claim set or clearly marked for review;
- every number is sourced or labeled illustrative;
- no standard/guidance is strengthened into a requirement;
- no real case loses attribution;
- no adjacent episode is re-taught unnecessarily;
- both Oz and Rona contribute meaningfully;
- the listener tool is actually used;
- the episode closes with a practical action and correct handoff.

## Post-Claude rule

Claude is not an evidence source.

Any new consequential technical statement introduced by Claude must return to Source Verification before the script may be frozen.

After technical/editorial approval, the frozen dialogue is transformed into a dedicated Google NotebookLM production package under:

`podcast/GEMINI_NOTEBOOK_AUDIO_PRODUCTION_CONTRACT.md`

Google NotebookLM Audio Overview is treated as a generative downstream production layer, not as a deterministic text-to-speech reader of Claude's line-by-line dialogue.
