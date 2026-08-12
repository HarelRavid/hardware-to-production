# P2.05 — Process Economics: Sensitivity, Uncertainty & Canonical Decision Pack

Status: NEAR PODCAST READY

## Purpose
Turn manufacturing economics from a single-point spreadsheet into an evidence-linked decision system for DEV → LVP → SVP.

Canonical rule:
> A precise NPV built on weak production assumptions is not a precise decision.

## 1. Economics chain
Demand hypothesis → process alternative → fixed investment → variable conversion cost → yield/rework → utilization/capacity → maintenance/downtime → change/requalification → cash flow → NPV / payback / break-even → uncertainty/sensitivity → decision gate → post-investment verification.

The manufacturing evidence created in P2.02–P2.04 is upstream evidence for this model. Economics must not silently overwrite it with optimistic assumptions.

## 2. Sentinel Node alternatives
Use the established three alternatives:
- Manual
- Semi-automatic
- Full automation

The model shall separate:
- CapEx
- NRE/integration/qualification
- labor and consumables
- scrap/rework
- maintenance/spares/service
- downtime/capacity loss
- floor-space/utilities where material
- product-change/requalification cost
- working-capital/WIP effects where material
- residual value where justified

## 3. Sensitivity matrix
Every investment recommendation must test at least these drivers:

| Driver | Downside | Base | Upside | Why it matters |
|---|---:|---:|---:|---|
| Annual demand | -25% | forecast | +20% | spreads fixed cost and drives utilization |
| Ramp timing | +6 months delay | plan | -3 months | delays savings/revenue |
| FPY | -5 pp | demonstrated/assumed base | +2 pp | changes accepted output and rework burden |
| Availability | -10 pp | demonstrated/assumed base | +3 pp | changes practical capacity |
| Maintenance/support | +50% | base | -20% | affects ownership cost and downtime |
| Labor rate | -10% | base | +20% | changes automation savings |
| Product life | -2 years | base | +2 years | changes time available to recover fixed investment |
| Engineering change | major requalification | expected case | none | can strand tooling/software/integration investment |
| Discount rate | higher | base | lower | changes present value of delayed benefits |

Do not interpret this as a universal mandated range. These are project-model scenarios and must be replaced by defensible ranges when project evidence exists.

## 4. Uncertainty classes
Tag important inputs as:
- E1 — directly demonstrated by representative production evidence
- E2 — supported by supplier quote, historical data or comparable process
- E3 — engineering estimate with explicit basis
- E4 — forecast/assumption with weak evidence

A decision dominated by E4 inputs must not be presented with false precision.

## 5. Tornado logic
Rank variables by their effect on the decision metric, not by how easy they are to edit in Excel.

Recommended metrics:
- ΔNPV versus next-best alternative
- break-even volume
- payback time
- capacity margin
- cost per accepted unit at representative utilization

If demand and utilization dominate the result, the next action may be market/ramp evidence rather than a more detailed machine quote.

If FPY and downtime dominate, the next action is production learning/maintenance evidence rather than finance-model refinement.

## 6. Sentinel Node decision example
Base-case result may favor full automation at high sustained volume because of lower variable conversion cost.

But test a downside combination:
- demand -25%
- ramp delayed six months
- early FPY below plan
- availability below plan
- maintenance/support above plan
- Year-3 product change requiring tooling/software/requalification

Possible outcome:
- full automation still has the lowest theoretical steady-state unit conversion cost;
- semi-automation has better risk-adjusted economics over the actual planning horizon;
- therefore the rational decision can be STAGE/SEMI-AUTOMATE FIRST.

This is not a claim that semi-automation is universally superior. It demonstrates why unit cost and investment value are different questions.

## 7. ECON 10 — canonical listener tool
1. Demand — what volume/ramp is actually supported?
2. Fixed — what CapEx + NRE + qualification is required?
3. Variable — what changes per accepted unit?
4. Yield — what scrap/rework assumptions are used?
5. Utilization — what realistic loading supports the unit-cost claim?
6. Reliability — what downtime, maintenance, spares and recovery burden exists?
7. Change — what happens when product/process configuration changes?
8. Time — when do costs occur and benefits arrive?
9. Uncertainty — which assumptions dominate the decision and how strong is their evidence?
10. Alternative — can fixture, poka-yoke, balancing, outsourcing or semi-automation solve the real constraint with less irreversible investment?

## 8. Process Selection Gate
### INVEST NOW
Use when the constraint/problem is demonstrated, demand and utilization are sufficiently supported, economics remain attractive under reasonable downside, qualification path is understood, and the investment does not create unacceptable inflexibility.

### STAGE / SEMI-AUTOMATE FIRST
Use when the problem is real but demand, product architecture or process learning remains uncertain; a smaller investment can generate evidence while improving quality/rate.

### DEFER UNTIL EVIDENCE IMPROVES
Use when economics are dominated by weak assumptions, representative production evidence is missing, or the investment solves a forecast rather than a demonstrated constraint.

### REJECT / SELECT ALTERNATIVE
Use when a lower-risk process architecture provides better system economics or the proposed investment fails the required return/capacity/quality envelope.

## 9. DEV / LVP / SVP applicability
### DEV
Optimize learning economics. Avoid locking an immature product/process into expensive dedicated equipment unless the equipment itself is required to retire a critical risk.

### LVP
Invest against demonstrated constraints and failure mechanisms. Semi-automation, fixtures and poka-yoke may maximize learning per dollar while preserving flexibility.

### SVP
Use sustained evidence for demand, FPY, availability, maintenance, product mix and change frequency. Larger irreversible CapEx becomes more defensible when the production system and market envelope are demonstrated.

## 10. Evidence guardrails
- Break-even volume is not NPV.
- Lowest unit cost is not automatically best investment.
- Rated machine speed is not demonstrated capacity.
- Supplier uptime claim is not site availability evidence.
- NRE divided by forecast volume is allocation, not investment analysis.
- Sensitivity analysis does not repair bad assumptions; it exposes their importance.
- Use ranges/scenarios where evidence is uncertain; do not hide uncertainty behind decimals.
- Re-run the economics after representative production evidence changes FPY, availability, constraint, maintenance or demand assumptions.

## 11. Evidence basis
NIST manufacturing-economics work supports life-cycle/investment analysis approaches and the use of economic metrics such as NPV/IRR/payback in manufacturing decisions. NIST maintenance research also shows that maintenance strategy can materially affect downtime, defects, delays and inventory, supporting explicit maintenance/reliability treatment in the economic model.

This document's ECON 10, evidence classes, scenario ranges and Process Selection Gate are project synthesis, not claimed requirements of NIST or any standard.

## 12. Podcast-ready messages
> Do not automate the forecast. Automate the constraint after the evidence earns the investment.

> Lowest unit cost and best investment are not the same question.

> The economics spreadsheet is downstream of the factory evidence.

> If one uncertain assumption can reverse the decision, that assumption is part of the engineering work.

## 13. P2.05 readiness
Captured:
- process alternatives
- break-even logic
- five-year cash-flow / NPV logic
- downside scenario
- maintenance and utilization treatment
- sensitivity matrix
- uncertainty/evidence classes
- ECON 10 listener tool
- DEV/LVP/SVP applicability
- Process Selection Gate

Remaining before PODCAST READY:
- episode-level source-note packaging
- technical/economic review of numerical assumptions
- final worked spreadsheet/table if used in show notes

Current status: **NEAR PODCAST READY**.
