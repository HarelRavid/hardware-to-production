# EP09 Final Script Outline — Tolerance, GD&T/GPS and Variation

status: FINAL SCRIPT OUTLINE COMPLETE — SEASON CONTINUITY PENDING
season: Season 1
audience: mechanical / manufacturing / metrology / NPI / quality
lifecycle: DEV → LVP → SVP
source_lock: evidence/source-lock/season-1/S1C_EP09_CLAIM_LOCK.md
technical_review: evidence/source-lock/season-1/S1C_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-1/EP09_PRODUCTION_BLUEPRINT.md
research: podcast/season-2/EP09_RESEARCH_PACK.md

## Listener transformation
Before:
“The prototype fits, so the dimensions are fine.”

After:
“I can reason from function to allowable variation, reference strategy, tolerance accumulation, measurement and population evidence.”

## Two-character opportunity
Speaker B:
“Why not just tighten every dimension until the stack works?”
Speaker A:
Because that may raise cost without creating functional margin or measurable capability.

## Cold open
[ILLUSTRATIVE]
One enclosure, PCB and connector fit perfectly; production distributions occasionally collide.

## Beat 1 — CAD nominal vs production variation
Claims: EP09-C01/C05.

## Beat 2 — Function before tolerance
Claim: EP09-C02.

## Beat 3 — Datum/reference concept
Claim: EP09-C03.
Current standards context:
- ASME Y14.5-2018 (R2024);
- ISO 8015:2011;
- ISO 1101:2017;
- ISO 5459:2024;
- ISO 2692:2021.
Guard:
do not teach exact protected rule/default/modifier from memory.

## Beat 4 — ASME vs ISO GPS boundary
Claim: EP09-C08.
Do not mix rule systems casually.

## Beat 5 — Tolerance accumulation
Claim: EP09-C04.
Use enclosure/PCB/connector.

## Beat 6 — Worst-case vs statistical stack
Claim: EP09-C07.
Illustrative Stack A:
±0.20, ±0.15, ±0.10 mm
worst case ±0.45 mm;
RSS ≈ ±0.2693 mm under explicit assumptions.
Explain that RSS is not an automatic yield prediction.

## Beat 7 — Measurement adequacy
Claim: EP09-C06.
Observed variation may include measurement variation.

## Beat 8 — Redesign for margin
Use architecture/datum/interface change before tightening everything reflexively.

## Listener tools
Functional Tolerance Chain.
Variation Evidence Review.

## Misconceptions
- tighter tolerance always means better quality;
- one working prototype represents the population;
- worst-case predicts expected yield;
- RSS is valid without assumptions;
- ASME and ISO GPS are interchangeable.

## Closing action
For one critical interface, identify the functional envelope, each contributor, measurement method and analysis assumption before changing any tolerance.

## Handoff
EP09 adds population variation.
EP10 adds time, environment, wear and field evidence.
