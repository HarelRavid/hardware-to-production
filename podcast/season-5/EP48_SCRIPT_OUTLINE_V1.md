# EP48 Script Outline V1 — Product Genealogy, Recipes, Parameters and Measurements

status: SCRIPT OUTLINE COMPLETE
season: Season 5 — Automation, Data and the Connected Factory
audience: manufacturing / quality / data / NPI / field engineering
lifecycle: LVP → SVP → FIELD
source_lock: Wave 05
technical_review: evidence/source-lock/wave-05/W5_INTERNAL_TECHNICAL_REVIEW.md

## Listener promise
Design a reconstructable Unit Evidence Thread linking configuration, materials, operations, equipment, recipes, measurements, rework and release.

## Cold open
[ILLUSTRATIVE] Serial 1847 fails in the field. Test result exists, but material lot, recipe revision and rework history cannot be linked.

## Beat 1 — Serial is identity, not genealogy
Claim EP48-C01.
Source: W5-S06.

## Beat 2 — Build the Unit Evidence Thread
Claim EP48-C02.
Product config → materials → routing → equipment → recipe/software → parameters → measurements → deviation/rework → disposition → field linkage.

## Beat 3 — Historical truth vs current master data
Claim EP48-C03.
Revision/effectivity/history dependency.

## Beat 4 — Durable identity
Claims EP48-C04/C05.
Sources W5-S04/S05.
Guard: UUID helps identity; it does not create authority/provenance alone.

## Beat 5 — Recipe/parameter context
Values need operation, unit, equipment, recipe version, unit of measure and time context.

## Beat 6 — Measurements/test and measurement-system identity
Dependency: Wave 02.

## Beat 7 — Rework adds history
Claim EP48-C06.
Never overwrite original failure/state.

## Beat 8 — Time/event ordering
Claim EP48-C07.
No universal sync precision.

## Listener tool — RECONSTRUCT 8
What built? From what? Where? How? Which recipe/config? What measured? What failed/changed? What population shares dependency?

## Misconceptions
- serial number = genealogy;
- latest BOM reconstructs old unit;
- store every tag and genealogy appears;
- UUID = provenance;
- final PASS erases rework.

## Closing action
Pick one shipped serial and try to reconstruct it without asking the original builder.

## Handoff
EP49 links physical evidence to engineering claims and sources.
