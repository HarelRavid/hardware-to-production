# P2.05 — Five-Year Cash-Flow, NPV and Downside Worked Example

Status: IN PROGRESS — CASH-FLOW / NPV / DOWNSIDE LAYER CAPTURED

## Purpose

Extend the Sentinel Node process-selection example beyond unit cost and simple break-even. The objective is to show why a manufacturing investment must be evaluated across time, utilization, yield, maintenance, ramp risk and uncertainty.

This is a worked teaching model, not a universal cost standard. Values are illustrative and must be replaced with project-specific quotations, labor rates, financing assumptions, tax treatment, depreciation, working-capital effects and verified production evidence before a real investment decision.

## 1. Candidate process architectures

| Parameter | Manual | Semi-automatic | Full automation |
|---|---:|---:|---:|
| Initial CapEx + NRE | $5,000 | $45,000 | $180,000 |
| Variable conversion cost / launched unit | $9.50 | $5.75 | $3.05 |
| Annual fixed support / maintenance | $2,000 | $7,000 | $22,000 |
| Planning FPY assumption | 94% | 97% | 98% |
| Practical annual capacity assumption | 12,000 | 32,000 | 55,000 |

Guardrail: FPY, uptime and capacity assumptions are not allowed to outrun the evidence generated in P2.03 and P2.04.

## 2. Five-year demand scenario

Base demand forecast:

- Y1: 6,000 accepted units
- Y2: 12,000
- Y3: 20,000
- Y4: 30,000
- Y5: 40,000

This immediately exposes an important issue: the manual process is not a five-year solution and the semi-automatic architecture becomes capacity constrained late in the horizon. Economic comparison therefore has to include the cost and timing of the next capacity step rather than pretend every alternative can serve every forecast point.

## 3. Accepted-unit economics

Approximate launched units required = accepted demand / FPY.

Illustrative Y2 comparison at 12,000 accepted units:

- Manual launches ≈ 12,766 units at 94% FPY.
- Semi-auto launches ≈ 12,371 units at 97% FPY.
- Automation launches ≈ 12,245 units at 98% FPY.

Variable conversion spend therefore depends on yield as well as nominal cost per launch.

This is why `$ / operation` is not the same as `$ / accepted product`.

## 4. Cash-flow logic

For each year, model at minimum:

`Net manufacturing cash benefit versus baseline = avoided baseline conversion cost - alternative conversion cost - incremental fixed support - incremental requalification/change cost - incremental working-capital/other relevant costs`

Then discount future cash flows:

`NPV = -Initial Investment + Σ(CFt / (1+r)^t)`

where `r` is the decision-specific discount/hurdle rate.

For the teaching example use 10% only as an illustrative hurdle rate. It is not a recommended universal manufacturing discount rate.

## 5. Base-case interpretation

The key lesson is deliberately not a single winning number.

At low volume, semi-automation can dominate because it removes expensive manual content with modest fixed investment. Full automation has the lowest nominal variable cost but must recover a much larger up-front investment and recurring support burden.

As demand grows, the decision changes again because capacity enters the model. If semi-automation cannot sustainably supply Y5 demand, the comparison must include:

- second fixture/cell or parallel station,
- additional operators,
- floor-space and utilities,
- duplicate test/calibration resources,
- additional maintenance/spares,
- or a later migration to automation.

Therefore a static break-even graph is useful but incomplete.

## 6. Downside scenario

Now stress the automated option rather than accepting the sales-case assumptions.

Illustrative downside changes:

- demand is 25% below base forecast,
- ramp is delayed six months,
- actual FPY during early ramp is 94% rather than 98%,
- annual maintenance/support is $30,000 rather than $22,000,
- unplanned downtime reduces usable capacity,
- product Rev D arrives in Y3 and requires $25,000 of tooling/software/requalification work.

The automation may still show the lowest theoretical steady-state unit conversion cost while losing much of its NPV advantage — or becoming economically inferior — because fewer accepted units absorb the fixed investment and because support/change costs arrive earlier than the expected benefits.

Podcast claim:

> Lowest steady-state unit cost does not necessarily produce the best investment.

## 7. Why maintenance belongs inside the investment model

Maintenance is not merely an operations KPI after the machine is purchased. It changes:

- cash cost,
- uptime,
- effective capacity,
- schedule risk,
- defect/recovery exposure,
- spare-parts inventory,
- technical staffing needs.

A process architecture that is inexpensive only when it never fails is not an economically complete architecture.

## 8. Why uncertainty belongs inside the model

A single forecast produces false precision. At minimum, sensitivity should test:

- demand / product mix,
- labor rate,
- FPY / scrap / rework,
- uptime,
- maintenance cost,
- CapEx overrun,
- ramp delay,
- engineering-change frequency,
- discount rate,
- residual value / redeployability where relevant.

For higher-stakes decisions, scenario or Monte Carlo analysis can be used instead of a single-point forecast.

## 9. Process Selection Gate

Before approving a manufacturing-process investment, ask:

1. What production problem are we solving?
2. What is the minimum viable intervention — WI/fixture/poka-yoke/semi-auto/full automation?
3. What demand and product-mix envelope must it serve?
4. Is that demand committed, forecast, or aspirational?
5. What FPY, uptime and rate assumptions are used, and what evidence supports them?
6. What CapEx and NRE occur before benefit starts?
7. What recurring maintenance, software, spares and specialist-support costs remain?
8. What happens when the product changes?
9. What is the NPV/payback under base and downside cases?
10. What option value do we lose by committing now?

Decision outputs:

- INVEST NOW
- STAGE / SEMI-AUTOMATE FIRST
- DEFER UNTIL EVIDENCE IMPROVES
- REJECT / SELECT ALTERNATIVE

## 10. DEV / LVP / SVP interpretation

### DEV
Optimize learning and avoid irreversible CapEx before the process and product architecture are understood.

### LVP
Invest where the evidence identifies a real constraint, quality mechanism, ergonomics/safety need or labor-content problem. Preserve flexibility because configuration and demand can still move quickly.

### SVP
Use sustained production evidence, maintenance history, actual product mix and verified demand to justify larger capital commitments and optimization.

This creates a strong link to the Hardware Evolution Ladder: process economics matures with the evidence maturity of the production system.

## 11. Source-backed backbone

NIST manufacturing-economics work treats manufacturing investment decisions as multi-period economic decisions and provides guidance using NPV, IRR, payback and related methods. NIST also treats maintenance costs/losses as economically material in manufacturing and provides evidence that maintenance strategy can affect downtime, defects, delays and inventory. NIST investment-analysis guidance also supports sensitivity/uncertainty analysis rather than reliance on one deterministic forecast.

Source anchors for episode packaging:

- NIST AMS 200-5 — Investment Analysis Methods: NPV, IRR and manufacturing investment decision principles.
- NIST AMS 200-11 / ASTM E3200-based guide — NPV, IRR, payback, hurdle rate and sensitivity/Monte Carlo techniques.
- NIST AMS 100-18 and AMS 100-34 — economics of machinery maintenance and losses.
- NIST AMS 100-50 — observed manufacturing investment returns; high-return categories include bottleneck reduction and scheduling, reinforcing the need to compare automation with simpler alternatives.

## 12. Guardrails

Do not claim:

- that 10% is a standard discount rate;
- that the illustrative costs represent industry averages;
- that automation always wins above a fixed volume;
- that payback alone is sufficient for investment selection;
- that forecast demand equals demonstrated demand;
- that nominal machine capacity equals sustainable accepted-output capacity.

## 13. Podcast-ready takeaways

1. Unit cost is a snapshot; investment value is a time series.
2. Yield converts launched-unit economics into accepted-unit economics.
3. Utilization determines how much output absorbs fixed cost.
4. Maintenance is part of economics, not an afterthought.
5. Product changes can create a second NRE event after automation is installed.
6. A downside case is mandatory when the decision is hard to reverse.
7. The best process at DEV may intentionally be different from the best process at SVP.

Canonical line:

> Do not automate the forecast. Automate the constraint after the evidence earns the investment.
