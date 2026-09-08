# Episode 50 Production Blueprint — The Manufacturing Atlas: Turning Knowledge into Decisions

status: PRODUCTION BLUEPRINT COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
lifecycle: CROSS-STAGE
maps_to: MASTER_WBS 9.9, 9.10

## Listener transformation
Before: treats the knowledge base as a place to search for answers.
After: uses context, alternatives, applicability, evidence and prior decisions to build repeatable manufacturing decision support without hiding uncertainty.

## Narrative hook
Two engineers ask, “Should we injection mold this part?” and receive different answers because one is building 50 units next month and the other 200,000 units over three years. A useful knowledge system must understand the decision context, not merely retrieve facts about molding.

## Teaching flow
1. Search answers facts; engineering decisions require context and alternatives.
2. Capture decision question, lifecycle stage and product/process envelope.
3. Identify relevant requirements/CTQs and constraints.
4. Retrieve applicable process/material/supplier/quality knowledge.
5. Compare alternatives with evidence and uncertainty visible.
6. Reuse canonical decision frameworks rather than ad-hoc scoring.
7. Record decision, rationale, assumptions and rejected alternatives.
8. Link later outcomes/field evidence back to the decision.
9. Make updates affect dependent decisions selectively.
10. AI can assist navigation/synthesis but must expose sources, scope and uncertainty.

## Core framework — ATLAS 10 Decision Path
`Question → context → requirements/CTQs → applicable knowledge → alternatives → evidence → trade-offs → decision → rationale/effectivity → outcome/learning`.

## Listener tools
- Manufacturing Atlas Decision Card.
- Decision Replay: could another engineer reproduce why this choice was made using the preserved assumptions, evidence and alternatives?

## DEV / LVP / SVP
DEV: Atlas helps preserve fast decisions and assumptions. LVP: it connects manufacturing route/supplier/process decisions to evidence. SVP: it supports controlled, auditable cross-functional decisions and change-impact analysis.

## Common mistakes
- knowledge graph with no decision workflow;
- one score hiding non-compensable constraints;
- AI recommendation without source/applicability path;
- old decision reused after volume/configuration changed;
- decision outcome never fed back into knowledge;
- Atlas becoming a second PLM/QMS/MES instead of linking authoritative systems.

## Source/evidence backlog
The Atlas is an internal synthesis framework, not an industry standard. Any embedded technical rule inherits the source/applicability burden of its underlying claim; AI-generated synthesis remains marked until externally verified.

## Closing handoff
Episode 51 addresses the plumbing needed to connect production systems without losing meaning: semantic context, ISA-95 and OPC UA without buzzwords.
