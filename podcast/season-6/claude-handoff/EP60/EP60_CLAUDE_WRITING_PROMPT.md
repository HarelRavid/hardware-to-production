# Claude Writing Prompt — EP60: From Prototype to Production: The Full Decision Story

You are writing the final episode of the Hardware-to-Production podcast.

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
Write the complete final two-character dialogue for:

**EP60 — From Prototype to Production: The Full Decision Story**

Season 6 and full-series finale.

This is an integration task, not a research task and not a recap exercise.

## READ FIRST
Handoff Manifest:
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/claude-handoff/EP60/EP60_HANDOFF_MANIFEST.md

Two-Character Dialogue Style Contract:
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/TWO_CHARACTER_DIALOGUE_STYLE_CONTRACT.md

Season 6 Final Continuity Review:
https://github.com/HarelRavid/hardware-to-production/blob/main/podcast/season-6/SEASON_6_FINAL_CONTINUITY_REVIEW_FOR_CLAUDE.md

Read every MUST READ file in the manifest.

## CORE JOB
Use the fictional Sentinel Node to show how the same hardware product moves through:

Idea
→ Requirements
→ Architecture
→ POC
→ Integrated Prototype
→ Engineering Prototype
→ Production-Intent Hardware
→ LVP
→ Production Validation
→ Ramp
→ SVP
→ Field learning/change.

At each transition, show:
- what decision becomes necessary;
- what evidence now exists;
- what assumption/shortcut can still be tolerated;
- what shortcut has expired;
- what product/process/supplier/measurement/rate/economic context changed.

## CHARACTERS
**OZ — Lead Host / Systems Engineer**
Connects the decisions and explains why evidence burden changes with commitment.

**RONA — Practitioner / Challenger**
Keeps asking:
“Why can’t we make this decision once and keep it?”
and tests whether the framework changes real engineering behavior.

B must be technically competent and should surface the temptation to:
- freeze too early;
- keep shortcuts too long;
- overbuild systems too early;
- treat release as the end of learning.

## FRAMEWORK RULES
Use only existing canonical frameworks.

Do NOT invent:
- a new final maturity model;
- a new mega-framework;
- a new score;
- a new lifecycle.

Use compact callbacks for:
requirements, interfaces, representativeness, verification, configuration, process selection, quality/measurement, pilot/validation/rate, supplier/economics, automation/data/security, field evidence.

Do not re-teach them.

## PRIMARY TOOL
Execute the **Full Decision Ledger** on a few key Sentinel decisions:

Decision
→ lifecycle context
→ configuration
→ assumption/unknown
→ alternatives
→ evidence available then
→ chosen path
→ shortcut/debt
→ expiration/change trigger
→ outcome
→ learning.

Use the tool to show decision evolution, not to read every field repeatedly.

## QUANTITATIVE / CASE RULE
Sentinel Node is fictional.
Every quantity is illustrative.
Do not present any value as benchmark or real-company data.

No new public case is permitted.

## STYLE
This should feel like the payoff of the full series:
- confident;
- practical;
- reflective but technical;
- not nostalgic;
- not a two-hour recap.

Target about 30–40 minutes if needed for a satisfying full journey, but prioritize decision integration over duration.

## SERIES CLOSE
End with the core principle:
the goal is not more manufacturing paperwork; it is preserving engineering truth while hardware changes, scales and recovers.

## OUTPUT
# EP60 — From Prototype to Production: The Full Decision Story

OZ:
...

RONA:
...

Optionally add:

## PRODUCTION NOTES — NOT SPOKEN

Only visual/callback/pronunciation/show-note reminders.

## SELF-CHECK
- no new framework;
- no new public fact/case;
- all quantities clearly illustrative;
- no excessive re-teaching;
- Full Decision Ledger actually used;
- lifecycle transitions are clear;
- both Oz and Rona technically useful;
- final series message matches the locked outline.
