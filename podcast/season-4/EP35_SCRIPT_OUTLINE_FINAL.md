# EP35 Final Script Outline — Traceability, Genealogy and Evidence Retention

status: FINAL SCRIPT OUTLINE COMPLETE — SEASON CONTINUITY PENDING
season: Season 4 — Quality, Suppliers and the Reality of Scale
audience: quality / manufacturing / NPI / field / data / supply chain
lifecycle: LVP → SVP → FIELD
source_lock: evidence/source-lock/season-4/S4A_EP35_CLAIM_LOCK.md
technical_review: evidence/source-lock/season-4/S4A_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-4/EP35_PRODUCTION_BLUEPRINT.md

## Listener transformation

Before:
“Traceability means serial numbers.”

After:
“I can define the genealogy needed to reconstruct affected populations without collecting meaningless data.”

## Two-character opportunity

Speaker B:
“We already serialize every product. Isn’t that traceability?”

Speaker A:
Identity tells you which unit; genealogy tells you how it became what it is.

## Cold open

[ILLUSTRATIVE]
Serial 1847 fails in field. Nobody can link it to supplier lot, firmware, calibration station, coating batch or rework history.

## Beat 1 — Identity vs genealogy
Claim: EP35-C01.

## Beat 2 — Genealogy chain
Claim: EP35-C02.
configuration/effectivity → material/supplier → route/equipment/recipe → measurement/test → deviation/rework → release/service.

## Beat 3 — Granularity by consequence
Claim: EP35-C03.
Not every tag/event belongs in permanent genealogy.

## Beat 4 — Historical truth vs current master
Claim: EP35-C04.
Today’s BOM/recipe is not proof of yesterday’s build.

## Beat 5 — Retention
Claim: EP35-C05.
Sector/customer/legal specific.

## Beat 6 — Affected-population query
Claim: EP35-C06.
Start with changed/failing dependency and identify exposed vs unexposed units/lots.

## Beat 7 — Rework adds history
Claim: EP35-C07.

## Beat 8 — Architecture is implementation-neutral
Claim: EP35-C08.
One database not required.

## Listener tool — Genealogy Evidence Chain
unit/lot → config/effectivity → material/supplier → process route → equipment/tool/recipe → measurement/test → deviation/rework → release → field/service.

## Listener tool — Affected-Population Query
what changed? when effective? what dependency? which units/lots passed through it? what evidence separates exposed from unexposed?

## Misconceptions
- serial = genealogy;
- current BOM reconstructs history;
- more data always means better traceability;
- final PASS erases rework;
- one database is required;
- retention period can be copied from another industry.

## Closing action
Pick one field failure and try to isolate the affected population without asking the original builder.

## Handoff
EP35 tells us what evidence must be reconstructable.
EP36 asks which external/internal requirements actually govern what evidence we need.
