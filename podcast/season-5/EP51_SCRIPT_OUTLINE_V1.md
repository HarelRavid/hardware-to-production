# EP51 Script Outline V1 — OPC UA, ISA-95 and Semantic Integration Without the Buzzwords

status: SCRIPT OUTLINE COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
audience: controls / manufacturing data / automation / IT-OT / systems
lifecycle: LVP → SVP
source_lock: Wave 05
technical_review: evidence/source-lock/wave-05/W5_INTERNAL_TECHNICAL_REVIEW.md

## Listener promise
Connect systems while preserving engineering meaning: identity, hierarchy, units, states, operation/product/recipe context and model version.

## Cold open
[ILLUSTRATIVE] Data platform receives Temp_07 = 83.4. Nobody knows what it measures, which unit, operation, recipe or units.

## Beat 1 — Connectivity vs syntax vs semantics
Claim EP51-C01.

## Beat 2 — ISA-95 scoped context
Claim EP51-C02.
Source W5-S01/S02.
Guard: not mandatory stack or cyber zones.

## Beat 3 — OPC UA infrastructure/information models
Claim EP51-C03.
Source W5-S03.

## Beat 4 — Companion Specifications
Claim EP51-C05.
Evaluate applicable models before proprietary reinvention; not universal mandate.

## Beat 5 — Stable/durable identity
Claims EP51-C04/C06.
NodeId/tag/source key not automatically cross-system identity.

## Beat 6 — Context-to-data mapping
Engineering object → identifier → hierarchy → signal/attribute → units/state → owner → product/operation/recipe → consumer.

## Beat 7 — Version/effectivity
Semantic mappings/models change too; control them.

## Beat 8 — Offline/latency/security consequence
Keep security preview only; EP52 owns OT risk.

## Listener tool — Meaning-Preservation Test
Can a consumer interpret the datum correctly without tribal knowledge about the source tag/database?

## Misconceptions
- OPC UA endpoint = semantic architecture;
- ISA-95 = Purdue security model;
- tag name = global identity;
- connectivity solves data ownership;
- protocol security solves OT cybersecurity.

## Closing action
Pick ten important machine tags and see whether a new engineer can interpret them with product/operation/units/state context.

## Handoff
EP52 asks which connected data is fit for engineering decisions and how to access OT without creating unsafe pathways.
