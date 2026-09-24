# A3 Final Script Outline — System Architecture & Interfaces

status: FINAL SCRIPT OUTLINE COMPLETE — SEASON CONTINUITY PENDING
season: Season 1
audience: founders / systems / mechanical / electronics / embedded / NPI
lifecycle: DEV-first / cross-stage
source_lock: evidence/source-lock/season-1/S1A_A3_CLAIM_LOCK.md
technical_review: evidence/source-lock/season-1/S1A_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-1/A3_PRODUCTION_BLUEPRINT.md
research: podcast/season-1/A3_RESEARCH_PACK.md

## Listener transformation
Before:
“Each subsystem owner can optimize their own part.”

After:
“I can identify risky interfaces, define a lightweight contract, assign responsibility and plan evidence before integration failure forces redesign.”

## Two-character opportunity
Rona begins from:
“If the connector, PCB and enclosure all meet their own specs, why isn’t the interface proven?”
Oz separates component evidence from interaction evidence.

## Cold open
[ILLUSTRATIVE]
Mechanical, electronics and firmware each meet their local goal, but the assembled product resets when the cable bends and service access requires removing the heatsink.

## Beat 1 — Interfaces are where local success meets system behavior
Claim: A3-C01.
Sources: S1A-S04/S05.

## Beat 2 — Lightweight architecture decomposition
Product function → subsystem → interface → owners → dependency → failure consequence.
Tag: V6 SYNTHESIS.

## Beat 3 — Interface families
Claim: A3-C02.
Examples:
mechanical / electrical / data / thermal / fluidic / user-service / manufacturing-test.
Guard:
taxonomy is ours.

## Beat 4 — Ownership and change authority
Claim: A3-C03.
Source: NASA Appendix L.

## Beat 5 — Interface Contract Sheet
Fields:
purpose → owners → definition → limits/tolerance → states → abnormal states → verification → change authority.
Guard:
lightweight internal tool, not required formal IRD.

## Beat 6 — Interaction claim
Claims: A3-C04/A3-C07.
Component ratings do not automatically prove assembled interaction.

## Beat 7 — Temporary interfaces are legitimate
Claim: A3-C08.
Show jumper / oversized connector / provisional protocol.
Expiration occurs when another decision depends on it.

## Beat 8 — Change impact
Claim: A3-C06.
One side changes → reassess affected interaction evidence.

## Beat 9 — DEV / LVP / SVP
DEV: visible assumptions.
LVP: released interfaces that drive supplier/build/test.
SVP: cross-supplier/effectivity/change evidence.

## Listener tool execution
Use Sentinel Node connector-to-enclosure interface:
position / sealing / strain / pinout / grounding / service / test access / owner / verification.

## Misconceptions
- CAD assembly is the full interface definition;
- connector part number defines the interface;
- if both components meet spec, interaction is proven;
- systems engineering must be heavy;
- shared ownership means covered ownership.

## Closing action
Pick the five interfaces whose failure would cause the most redesign and write owners, limits, states and evidence for each.

## Handoff
A3 defines what must connect.
A4 asks which prototype can actually prove those interface claims.
