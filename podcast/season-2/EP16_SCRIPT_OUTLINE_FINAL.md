# EP16 Final Script Outline — Ceramics, Powder Processing and Sintering

status: FINAL SCRIPT OUTLINE COMPLETE — SEASON CONTINUITY PENDING
season: Season 2 — How Hardware Is Actually Made
audience: design / NPI / manufacturing / quality / materials
lifecycle: DEV → LVP → SVP
source_lock: evidence/source-lock/wave-06/W6F_EP16_CLAIM_LOCK.md
technical_review: evidence/source-lock/wave-06/W6F_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-2/EP16_PRODUCTION_BLUEPRINT.md

## Listener transformation

Before:
“Powder parts are shaped, heated, and then they come out smaller.”

After:
“I can treat powder/feedstock, green state, debinding and sintering as linked manufacturing states, and I know what evidence must survive through the transformation.”

## Two-character opportunity

Speaker B:
“If I know my shrink factor and final furnace recipe, why do I need all this intermediate data?”

Speaker A:
Because the final geometry and properties can depend on green state, load, fixture, atmosphere and thermal history—not only one scalar or recipe line.

## Cold open

[ILLUSTRATIVE]
A green ceramic part is dimensionally correct. After sintering, one furnace location produces more distortion and another lot becomes fragile. Same CAD, same nominal recipe, different process state.

## Beat 1 — Powder/feedstock is the first product state

Claims: EP16-C01.
Sources: NIST powder/green-body characterization.

Discuss:
- particle/feedstock state;
- binder/moisture/dispersion where relevant;
- packing/flow/formability.

No generic numeric ranges.

## Beat 2 — Green body is an engineering object

Claim: EP16-C02.

Teach:
green density, strength, uniformity and geometry can matter before sintering.

Use NIST green-body density work.

## Beat 3 — Debinding/drying is not housekeeping

Claim: EP16-C03.

Explain:
mass transport + thermal history + binder removal can create cracks/voids/distortion.

Guard:
no universal debind schedule.

## Beat 4 — Sintering changes material state

Claim: EP16-C04.

Sources:
ISO 21821 / ISO 18754 / ASTM B962 / ISO 2738 context.

Teach:
densification, microstructure and dimensions evolve together.

## Beat 5 — One shrink factor is a dangerous shortcut

Claims: EP16-C05/C10.

Use worked example:
oversize design based on one scalar vs evidence map by feature/orientation/location.

No universal percentage.

## Beat 6 — Furnace/load/fixture/atmosphere can matter

Claims: EP16-C06/C11.

Explain:
recipe text is necessary but may not be sufficient to reconstruct actual part exposure.

## Beat 7 — Density/porosity is useful, but bounded

Claims: EP16-C07/C08.

Teach:
density/porosity can be process/quality evidence;
method applicability matters;
density alone does not prove all final properties.

## Beat 8 — Genealogy through transformation

Claim: EP16-C09.

Powder lot
→ mix/binder
→ forming
→ green-body evidence
→ debind
→ furnace/load/atmosphere
→ sintered density/microstructure
→ geometry
→ post-process
→ final evidence.

## Beat 9 — Prototype-to-production transfer

Claim: EP16-C12.

Small furnace / sparse load / expert handling may not represent loaded production conditions.

## Listener tool — Powder-to-Part Traveler

Powder lot/state
→ mix/binder
→ forming method
→ green body
→ debind
→ furnace/load/atmosphere
→ sintered density/microstructure
→ dimensions
→ post-process
→ release evidence.

## Listener tool — Shrinkage / Distortion Evidence Map

Feature/location/orientation
→ green dimension
→ final dimension
→ shrink/distortion
→ lot
→ fixture
→ furnace position/load
→ density/property evidence.

## DEV / LVP / SVP

DEV:
learn material/process sensitivities quickly; capture green/fired relationships.

LVP:
repeatable feedstock/forming/debind/sinter records and loaded-furnace evidence.

SVP:
controlled lots, fixtures, furnaces, atmospheres, thermal records, density/geometry/inspection and change/effectivity.

## Misconceptions

- one shrink factor works everywhere;
- final inspection is enough;
- furnace recipe text is complete process evidence;
- density proves all properties;
- green-body state does not matter once the part is sintered;
- small-batch success proves loaded-furnace production.

## Closing action

For one powder/sintered part, write the complete state chain from feedstock to final inspection and identify the first stage where current evidence becomes weak.

## Handoff

EP16 shows process-created geometry and material state through densification.
EP17 turns to additive manufacturing, where build orientation, machine state, powder/feedstock, post-processing and inspection again determine what the printed geometry actually means.
