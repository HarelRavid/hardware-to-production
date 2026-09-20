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

# Claude Writing Prompt — EP49: Standards, Claims and Evidence as a Manufacturing Knowledge Graph

You are writing the final spoken dialogue for the Hardware-to-Production podcast.

## Task
Write the complete two-character dialogue for **EP49 — Standards, Claims and Evidence as a Manufacturing Knowledge Graph**, Season 5.

This is not a research task. Do not redesign the episode, broaden the scope, or invent engineering guidance.

## Read first
Handoff Manifest:
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-5/claude-handoff/EP49/EP49_HANDOFF_MANIFEST.md

Two-Character Dialogue Style Contract:
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/TWO_CHARACTER_DIALOGUE_STYLE_CONTRACT.md

Season 5 Continuity Review:
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-5/SEASON_5_FINAL_CONTINUITY_REVIEW_FOR_CLAUDE.md

Read every file marked MUST READ in the manifest before drafting.

## Authority order
Claim Lock → Source Register → Technical Review → Script Outline → Blueprint → Season Continuity/Backbone → Source Notes → Existing Draft as reference only.

Never resolve a conflict by guessing.

## Characters
**OZ — Lead Host / Systems Engineer**
Owns decision structure, mechanisms, canonical framework/tool, source/applicability boundaries, lifecycle translation and adjacent-episode handoff.

**RONA — Practitioner / Challenger**
Technically competent. Pushes back on automation/data/AI/cyber buzzwords, asks what changes in real production, tests failure/recovery scenarios, and carries real technical content.

## Dialogue requirements
- Open with the approved hook.
- Make the listener transformation clear.
- Follow the Script Outline beats.
- Execute the primary listener tool on the worked example.
- Use concise callbacks instead of re-teaching prior episodes.
- Keep physical production consequences visible even in data/semantic topics.
- Correct the misconceptions in the Outline naturally.
- End with one practical action.
- End with the correct handoff to the next episode/season.

## Technical truth rules
- Use only consequential claims authorized by the Claim Lock.
- Preserve all applicability and standards-status guards.
- Internal Hardware-to-Production frameworks must be presented as our tools, not external standards.
- Do not invent values, standards rules, security levels, network topologies, legal requirements or real incidents.
- If a new consequential claim seems necessary, put it under **REVIEW FLAG — NOT FOR AUDIO**.
- Do not read URLs, file paths, claim IDs or citation syntax aloud.

## Season 5 specific guards
- OEE is a loss lens, not root cause/system capacity proof.
- “Cobot” does not mean the application is safe.
- ISA-95 is not cyber segmentation.
- OPC UA connectivity is not complete semantics or complete OT security.
- Read-only is not automatically safe.
- IEC 62443 does not prescribe one universal topology/security level.
- Running again after disruption is not automatically trustworthy manufacturing recovery.
- AI/derived output does not replace evidence provenance.

## Standards/current-status
Use the current status in the Source Register / Source Notes.
Do not treat revision projects as published standards.

For EP52 specifically, IEC 62443-2-1:2024 remains the current edition as rechecked on 2026-09-19.
NIST SP 800-82 Rev.3 remains the current final guide as rechecked on 2026-09-19.

## Numbers
Use only approved sourced or illustrative numbers.
Preserve assumptions and explain what the calculation does not prove.

## Style
Follow the Two-Character Dialogue Style Contract.
Target approximately 22–32 minutes depending on technical density.
Move spatial architecture/standards metadata to production notes rather than overloading audio.

## Output format
# EP49 — Standards, Claims and Evidence as a Manufacturing Knowledge Graph

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
- handoff correct.
