# Episode 11 Research Pack — How to Select a Manufacturing Process

status: RESEARCH PACK OPEN
season: Season 2 — How Hardware Is Actually Made
primary_audience: Audience A + Audience B
secondary_audience: mechanical, materials, NPI, manufacturing, sourcing, quality, finance/operations
lifecycle: DEV → LVP → SVP
entry_point: PROCESS-SELECTION FOUNDATION
technical_depth: practitioner

## 1. Episode promise
Teach teams to choose a manufacturing route by function, material, geometry, tolerance, surface, volume, tooling, capability, inspection, supplier maturity and cost per accepted good part — rather than by familiarity, prototype convenience or headline unit price.

Canonical listener question:
> Given this part and this production stage, what manufacturing process should we actually use — and when should we switch routes as volume and evidence mature?

## 2. Navigation card
**You are here:** product/readiness/design-for-production → manufacturing process selection → process-family deep dives.
**Best for:** teams choosing between machining, molding, casting, forming, additive, composites, joining/process chains or bridge routes.
**Prerequisite:** Episode 6 DFM helpful, not mandatory.
**You will leave with:** Process Selection Decision Grid + Bridge-Process Exit Check.
**Next:** Episode 12 Polymer Parts → Episode 13 Metal Parts → later joining/composites/ceramics/AM/process-chain episodes.

## 3. Core thesis
There is no universally “best” manufacturing process for a geometry. The right route depends on the product claim, material state, geometry, tolerance/surface, volume, tooling/NRE, process capability, supplier/equipment maturity, inspection/qualification burden, lead time, automation and economics.

The process decision can also change across DEV → LVP → SVP. A bridge route can be the correct production route for one stage and the wrong route later.

## 4. Draft claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP11-C01 | Manufacturing-process selection is a multi-constraint decision, not a geometry-only or unit-price-only choice. | P0 | BACKBONE-SUPPORTED |
| EP11-C02 | The same part may rationally use different processes across DEV, LVP and SVP as volume, evidence and economics change. | P0 | BACKBONE-SUPPORTED |
| EP11-C03 | Material condition, tolerance, surface, joining/post-process and inspection requirements can make two nominally similar routes non-equivalent. | P0 | BACKBONE-SUPPORTED |
| EP11-C04 | Cost comparisons should include tooling/NRE, scrap/rework, inspection, secondary operations and accepted good-unit economics where material. | P0 | ECON/BACKBONE-STABLE |
| EP11-C05 | Supplier capability/maturity is part of process selection because nominal process capability in theory does not prove a specific source can repeatedly meet the claim. | P0 | SUPPLIER/BACKBONE-STABLE |
| EP11-C06 | Prototype convenience can create false confidence if the prototype route hides failure/variation mechanisms that matter in production. | P0 | A4/A5/A6/BACKBONE-STABLE |
| EP11-C07 | A bridge process should have explicit expiration triggers based on volume, evidence, cost, capability, lead time or risk. | P1 | SYNTHESIS/BACKBONE |
| EP11-C08 | Process chains should be evaluated as sequences because heat treatment, cleaning, coating, joining and finishing can change geometry/material/surface and evidence. | P1 | BACKBONE-SUPPORTED |

## 5. Listener tool — Process Selection Decision Grid
For each candidate route score/describe:
| Dimension | Question |
|---|---|
| Function | What product requirement/CTQ is served? |
| Material/state | What material, temper, composition or state is required? |
| Geometry | Size, wall, undercut, section, aspect, internal features? |
| Tolerance/geometric control | What limits truly matter? |
| Surface | Finish, texture, coating, cleanliness, cosmetic, sealing/friction? |
| Volume/stage | DEV, LVP, SVP quantity/rate? |
| Tooling/NRE | What irreversible investment is required? |
| Unit economics | Material, cycle, labor, yield, secondary ops, inspection? |
| Capability evidence | What real source/process evidence exists? |
| Supplier/equipment availability | How many credible sources/equipment options exist? |
| Lead time/change flexibility | How costly is design/process iteration? |
| Inspection/qualification | How will the part/process be accepted? |
| Automation | What level is justified at this stage? |
| Post-process chain | Heat treat, machining, cleaning, coating, joining, finishing? |
| Risk/exit trigger | What would force a different route? |

## 6. Bridge-Process Exit Check
A bridge process remains justified only while its advantages outweigh its debt.

Ask:
1. Is the route still economically competitive at current/forecast volume?
2. Is it masking production-relevant material/process behavior?
3. Does it create manual rescue, inspection or supplier dependence that will not scale?
4. Is lead time becoming the constraint?
5. Is quality/capability evidence weaker than a serial-intent route could provide?
6. Would switching now force redesign/tolerance/interface changes?
7. What evidence must be generated before committing to new tooling/process?

## 7. Worked example — Sentinel Node enclosure route
DEV candidate: FDM printed enclosure for packaging/interface learning.
LVP candidates: CNC machined polymer/aluminum, urethane casting, low-volume molding or high-quality AM depending on claim/volume/economics.
SVP candidate: injection molding if geometry/material/volume/tooling economics/capability justify it.

The decision is not “injection molding is more professional.” It is whether the route supports the required product/process/economic envelope at that stage.

## 8. Process-family handoff map
Episode 11 owns selection logic; later episodes own depth:
- Ep12 polymers;
- Ep13 metals;
- Ep14 joining;
- Ep15 composites;
- Ep16 ceramics/powders/sintering;
- Ep17 additive;
- Ep18 surface/cleaning/heat treatment;
- Ep19 process chains.

## 9. DEV/LVP/SVP lens
**DEV:** maximize learning and iteration speed while recording which production-relevant dimensions are unrepresented.
**LVP:** choose bridge/low-volume routes deliberately, with controlled supplier/process evidence and expiration triggers.
**SVP:** commit to a demonstrated route whose capability, rate, quality, supply and economics match the commercial envelope.

## 10. Standards/source boundary
Process-specific design rules, material specifications, qualification methods and acceptance criteria belong to the relevant process/material standards and later source packs. Episode 11 can teach the decision dimensions without inventing universal numerical thresholds.

## 11. Applicability statement
The Process Selection Decision Grid is an internal framework. The correct route is product-, material-, supplier-, volume-, geography-, equipment- and standards-dependent.

## 12. What this episode must NOT claim
- higher-volume processes are always better;
- lowest quoted piece price is the lowest total cost;
- prototype success proves production-process capability;
- one process family is universally more precise/strong/reliable than another;
- automation level determines maturity;
- a bridge process must always be abandoned at a fixed quantity.

## 13. Research backlog before CLAIM SET STABLE
1. Cross-check process-selection and economics backbone.
2. Build authoritative source support for selection dimensions without universalizing process limits.
3. Confirm handoff boundaries with Episodes 12–19.
4. Add one comparative numerical economics example only after assumptions/arithmetic are audited.
5. Technical review: design/materials + manufacturing/process + sourcing/quality + economics.

## 14. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: MEDIUM at foundation level; HIGH in process-family follow-ons
Quantitative burden: MEDIUM
Backbone risk: LOW
Source verification: OPEN

Next status target: `RESEARCH PACK OPEN → CLAIM SET STABLE`
