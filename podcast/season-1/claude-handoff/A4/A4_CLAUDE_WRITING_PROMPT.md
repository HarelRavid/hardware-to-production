# Claude Writing Prompt — A4: Choosing Prototype Technologies Without Trapping the Product

You are writing the final spoken dialogue for the Hardware-to-Production podcast.

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

Never output legacy `SPEAKER A:` / `SPEAKER B:` labels.

Claude writes the canonical reviewed-dialogue draft. After project review and final dialogue freeze, the downstream Google NotebookLM package is built separately under `podcast/GEMINI_NOTEBOOK_AUDIO_PRODUCTION_CONTRACT.md`. Do not assume NotebookLM will read this dialogue verbatim.

## TASK

Write the complete final two-character dialogue draft for:

**A4 — Choosing Prototype Technologies Without Trapping the Product**

Season:
**Season 1 — Build the Right Hardware Before Production Finds Your Mistakes**

The downstream audio environment is Google NotebookLM. Claude writes the canonical Oz/Rona dialogue; after review/freeze a separate NotebookLM source/custom-prompt package is created.

This is not a research task.
Do not redesign the episode.
Do not expand the technical scope.
Do not invent new engineering guidance.

Your job is to turn the already verified episode package into a natural, technically deep, practical dialogue.

## FIRST — READ THE HANDOFF PACKAGE

Start with this manifest:

https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/claude-handoff/A4/A4_HANDOFF_MANIFEST.md

Then read every file marked MUST READ in the manifest before drafting.

You must also follow:

Two-Character Dialogue Style Contract:
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/TWO_CHARACTER_DIALOGUE_STYLE_CONTRACT.md

Season 1 Final Continuity Review:
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-1/SEASON_1_FINAL_CONTINUITY_REVIEW_FOR_CLAUDE.md

## AUTHORITY ORDER

When files differ, obey:

Claim Lock
→ Shared Source Register
→ Technical Review
→ Narrative Outline
→ Production Blueprint
→ Season Continuity / Knowledge Backbone
→ Research Pack


Never resolve a conflict by guessing.

## TWO CHARACTERS

### OZ — Veteran Engineer / Systems Engineer
A owns:
- the engineering decision;
- causal/mechanism explanations;
- canonical framework/tool;
- applicability boundaries;
- DEV/LVP/SVP translation;
- connection to adjacent episodes.

A must sound experienced and practical, not academic or bureaucratic.

### RONA — Young Engineer / Practitioner / Challenger
B is technically competent.

B should:
- challenge whether the rigor is really needed;
- ask what changes in practice;
- push on cost, speed, suppliers, operators and real build constraints;
- test the framework using the worked example;
- expose common shortcuts and misunderstandings;
- help summarize the practical action.

B must not be a naive student or a character who only agrees.

## DIALOGUE REQUIREMENTS

1. Open with the hook/scenario defined in the Narrative Outline.
2. Make clear what the listener will be able to do differently after the episode.
3. Follow the teaching beats and ownership boundaries in the Outline.
4. Execute the primary listener tool on the worked example — do not simply read the checklist fields.
5. Use concise callbacks for concepts already taught earlier in Season 1.
6. Include DEV/LVP/SVP only where the decision changes with maturity.
7. Correct the misconceptions defined in the Outline naturally through dialogue.
8. End with one concrete listener action.
9. End with the exact conceptual handoff to the next canonical episode.
10. Keep both characters technically useful throughout.

## TECHNICAL TRUTH RULES

- Every consequential factual or authoritative statement must be supported by the Claim Lock / Source Register.
- Internal Hardware-to-Production frameworks must be presented as “our tool,” “our working model,” or equivalent — never as an external standard.
- Do not upgrade guidance into a mandatory requirement.
- Do not invent typical values, thresholds, sample sizes, capability criteria, life factors or standards rules.
- Preserve all applicability limitations.
- Preserve source/company/regulator attribution when source ownership matters.
- If the package says a statement belongs in show notes rather than audio, do not force it into spoken dialogue.
- If a new technical statement seems necessary but is not in the locked package, add it only in a final section named **REVIEW FLAG — NOT FOR AUDIO** and explain what source verification would be needed.

## NUMBERS

Use only:
- sourced numbers explicitly approved in the package; or
- illustrative numbers explicitly approved in the package.

For any calculation:
- preserve units;
- preserve assumptions;
- explain what the number does not prove.

Do not invent convenient numbers to improve the story.

## STANDARDS

Do not make the episode sound like a standards lecture.

Do not read URLs, editions, clauses or citation metadata aloud unless the Outline explicitly says the edition/status is part of the lesson.

If a standard is named:
- use the exact locked name/status;
- never combine ASME/ISO/IEEE/NASA/AIAG rules casually;
- never claim universal applicability.

## STYLE / LENGTH

Follow the Two-Character Dialogue Style Contract.

For a Season 1 foundation/practitioner episode:
- target roughly 18–30 minutes depending on technical depth;
- prefer depth and clarity over forcing a word count;
- break dense explanation with challenge, example and practical consequence;
- avoid long checklist recitations.

## OUTPUT FORMAT

Return exactly:

# A4 — Choosing Prototype Technologies Without Trapping the Product

OZ:
...

RONA:
...

Continue alternating naturally.

After the spoken dialogue, optionally include:

## PRODUCTION NOTES — NOT SPOKEN

Only include:
- pronunciation/acronym note;
- visual/diagram cue;
- show-note source reminder;
- review risk.

Do not put citations or URLs into the spoken dialogue.

## FINAL SELF-CHECK

Before returning the draft verify:

- No consequential claim exists outside the locked claim set.
- No number was invented.
- No external standard/guidance was strengthened.
- No real case was invented or de-attributed.
- No adjacent episode was substantially re-taught.
- Canonical framework names were preserved.
- The listener tool was actually used.
- Rona carried real technical value.
- The practical action is explicit.
- The next-episode handoff is correct.
- Illustrative scenarios remain obviously illustrative.

If any check fails, revise the dialogue before returning it.
