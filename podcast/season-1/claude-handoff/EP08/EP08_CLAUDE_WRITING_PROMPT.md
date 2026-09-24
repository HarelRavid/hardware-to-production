## CANONICAL HOST NAMES — OVERRIDES LEGACY A/B LABELS

The recurring podcast hosts are:

**OZ — Veteran Engineer / Systems Engineer**  
Experienced, practical and technically rigorous. Oz brings systems, product-development, manufacturing, supplier, test, field and scale experience.

**RONA — Young Engineer / Practitioner / Challenger**  
A younger engineer who is already technically capable, sharp, curious and confident. Rona challenges assumptions, practicality, cost and overgeneralization and contributes her own technical reasoning. She is not a naive student.

Legacy mapping:
- Oz / Oz = Oz
- Rona / Rona = Rona

Mandatory output labels:
`OZ:`
`RONA:`

Never output `OZ:` / `RONA:`.

Claude writes the canonical reviewed-dialogue draft. After project review and final dialogue freeze, the downstream Google NotebookLM package is built separately under `podcast/GEMINI_NOTEBOOK_AUDIO_PRODUCTION_CONTRACT.md`. Do not assume NotebookLM will read this dialogue verbatim.

# Claude Writing Prompt — EP08: Design for Test, Calibration and Traceability

You are writing the final spoken dialogue for the Hardware-to-Production podcast.

## Task
Write the complete two-character dialogue for **EP08 — Design for Test, Calibration and Traceability**, Season 1.

This is not a research task. Do not redesign the episode, broaden scope, or invent engineering guidance.

## Read first
Handoff Manifest:
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/EP08/EP08_HANDOFF_MANIFEST.md

Two-Character Dialogue Style Contract:
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/TWO_CHARACTER_DIALOGUE_STYLE_CONTRACT.md

Season 1 Continuity Review:
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/SEASON_1_FINAL_CONTINUITY_REVIEW_FOR_CLAUDE.md

Read every file marked MUST READ in the manifest before drafting.

## Authority order
Claim Lock → Source Register → Technical Review → Final Outline → Blueprint → Continuity/Backbone → Research Pack.

Never resolve a conflict by guessing.

## Characters
**OZ — Lead Host / Systems Engineer**
Owns decision structure, mechanisms, canonical tool, applicability, lifecycle translation and adjacent-episode boundaries.

**RONA — Practitioner / Challenger**
Technically competent. Pushes on practicality, cost, speed, suppliers, operators and real build constraints. Tests the framework and exposes shortcuts. Must carry real technical content.

## Dialogue requirements
- Open with the approved hook.
- State the listener transformation naturally.
- Follow the Final Outline beats.
- Execute the primary listener tool on the worked example.
- Use concise callbacks instead of re-teaching previous episodes.
- Use DEV/LVP/SVP only where it changes the decision.
- Correct misconceptions through dialogue.
- End with one practical listener action.
- End with the correct handoff to the next episode.

## Technical truth rules
- Use only consequential claims authorized by the Claim Lock.
- Preserve applicability boundaries.
- Internal frameworks must be identified as our series tools, not standards.
- Do not invent values, thresholds, sample sizes, standards rules, legal requirements or real cases.
- If a new consequential claim seems necessary, put it under **REVIEW FLAG — NOT FOR AUDIO** instead of inserting it as fact.
- Do not read URLs, file paths, claim IDs or citations aloud.

## Standards and numbers
Use exact locked standard status only if materially needed in the audio.
Dense standard metadata belongs in production/show notes.
Use only approved sourced or illustrative numbers; preserve units and assumptions.

## Style
Follow the Two-Character Dialogue Style Contract.
Target a natural Season 1 foundation/practitioner episode, approximately 18–30 minutes depending on depth. Never cut a necessary technical distinction just to hit duration.

## Output format
# EP08 — Design for Test, Calibration and Traceability

OZ:
...

RONA:
...

After the dialogue you may add:

## PRODUCTION NOTES — NOT SPOKEN

Only pronunciation, visual cue, show-note reminder or review risk.

## Self-check
Before returning:
- no claim outside locked scope;
- no invented number;
- no strengthened standard/guidance;
- no duplicated adjacent episode;
- listener tool used;
- both Oz and Rona technically useful;
- practical action explicit;
- next handoff correct.
