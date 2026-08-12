# P2.05 — Process Economics / Scaling Worked Example

**Status:** ACTIVE — FIRST WORKED EXAMPLE CAPTURED  
**Canonical example:** Sentinel Node  
**Purpose:** teach teams to compare manufacturing routes using lifecycle economics rather than purchase price or nominal labor savings alone.

## 1. Core claim

A lower nominal unit processing cost does not automatically make a manufacturing route economically superior. The decision depends on demand, utilization, yield/rework, labor, consumables, maintenance, tooling/NRE, qualification/change cost, downtime, working capital and the time value of money.

This pack treats payback, NPV and IRR as decision aids rather than universal pass/fail thresholds. The appropriate hurdle rate and decision rule are organization-specific.

## 2. Sentinel Node decision

The production team is considering three assembly/test architectures for a mounting-and-test operation:

| Route | Architecture | Up-front NRE / CapEx | Variable conversion cost / accepted unit | Practical annual capacity |
|---|---|---:|---:|---:|
| M | Manual fixture + bench test | $8,000 | $14.00 | 6,000 |
| S | Semi-automatic fixture + guided test | $45,000 | $7.50 | 18,000 |
| A | Automated cell | $180,000 | $4.80 | 45,000 |

Illustrative values only. They are deliberately simple enough for a listener to reproduce.

## 3. Break-even is pairwise

Manual versus semi-auto:

Incremental fixed cost = 45,000 - 8,000 = $37,000  
Savings per accepted unit = 14.00 - 7.50 = $6.50

Break-even volume = 37,000 / 6.50 ≈ **5,692 accepted units**.

Semi-auto versus automation:

Incremental fixed cost = 180,000 - 45,000 = $135,000  
Savings per accepted unit = 7.50 - 4.80 = $2.70

Break-even volume = 135,000 / 2.70 = **50,000 accepted units**.

This immediately exposes a common error: the automated cell has the lowest nominal variable cost, but that alone does not make it the best choice at LVP volumes.

## 4. Utilization trap

The $4.80 automated-cell estimate assumes sufficient utilization to spread fixed ownership and support cost over substantial output. If demand is only 8,000 accepted units/year, unused capacity does not disappear economically.

For a simple teaching model, suppose annual ownership/support cost attributable to the automated route is $54,000/year in addition to the $4.80 variable cost. At 40,000 units/year this adds $1.35/unit. At 8,000 units/year it adds $6.75/unit.

So the same equipment can appear economically attractive or unattractive depending on utilization.

## 5. Yield trap

Cost must ultimately be related to accepted output, not merely launched units.

If a route has a direct launched-unit conversion cost C and first-pass yield FPY, the simplistic C/FPY calculation can be useful as a warning signal, but it is not a complete cost model because failed units may be reworked, scrapped, retested, delayed, or consume bottleneck capacity differently.

Example:

- automated nominal conversion cost = $4.80/launched unit
- FPY = 90%

$4.80 / 0.90 = $5.33 per first-pass-equivalent accepted unit before explicitly accounting for rework/scrap consequences.

If semi-auto achieves 99% FPY:

$7.50 / 0.99 = $7.58.

Automation may still win, but the gap is no longer the headline $7.50 versus $4.80, and the correct model must include the actual disposition path.

## 6. Hidden cost categories

Before comparing routes, capture at minimum:

1. equipment/tooling purchase;
2. design/integration/NRE;
3. installation and facilities;
4. qualification/FAT/SAT/production validation;
5. operator labor;
6. technician/engineering support;
7. consumables and energy;
8. preventive and corrective maintenance;
9. spares;
10. downtime and recovery;
11. yield, scrap, rework and retest;
12. changeover and product-mix loss;
13. software/licensing/data infrastructure;
14. training;
15. floor space / utilities where material;
16. working capital and WIP consequences;
17. future product-change/requalification cost;
18. residual value / disposal where material.

## 7. NRE amortization is a communication choice, not cash-flow analysis

Teams often divide NRE by forecast volume and call the result 'unit cost.' That can be useful for quoting or comparison, but it must not be confused with an investment cash-flow model.

Example: $180,000 CapEx divided by 100,000 forecast units = $1.80/unit. This arithmetic says nothing by itself about when the cash is spent, when savings arrive, uncertainty in demand, cost of capital, or whether the equipment becomes obsolete before the volume is realized.

## 8. Investment decision layer

For material investments, compare cash flows over time using appropriate methods such as:

- payback period;
- net present value (NPV);
- internal rate of return (IRR);
- sensitivity/scenario analysis.

NIST manufacturing investment guidance explicitly covers NPV and IRR and frames technology adoption as an investment-analysis problem. The hurdle rate and required payback period remain company decisions.

## 9. Sensitivity before precision

A useful model identifies which assumptions dominate the decision. For Sentinel Node, test at least:

- annual demand;
- product life;
- labor rate;
- FPY/rework;
- uptime;
- utilization;
- engineering support burden;
- maintenance/spares;
- product-mix/changeover;
- CapEx/NRE;
- discount rate;
- ramp delay.

A spreadsheet with six decimal places is not a better decision model if demand and yield are guesses.

## 10. Worked scenario

Suppose expected annual accepted demand is 10,000 units.

Ignoring financing for the first screening:

Manual annual conversion cost = 10,000 × $14 = **$140,000**.

Semi-auto annual conversion cost = 10,000 × $7.50 = **$75,000**.

Semi-auto therefore saves $65,000/year in nominal conversion cost relative to manual. Against the $37,000 incremental fixed investment, simple payback is roughly **0.57 years** if the assumptions are realized.

Automation versus semi-auto saves only 10,000 × ($7.50-$4.80) = **$27,000/year** before ownership/support differences. Against $135,000 incremental fixed investment, simple payback is **5 years** even before accounting for financing, maintenance, qualification, utilization risk or product change.

This is why 'automate because volume is growing' is not yet a business case.

## 11. Economics must connect back to engineering

Economic inputs are not independent of the technical system:

- PFMEA/control plan affect expected failure/rework cost;
- P2.03 measurement/yield evidence determines whether cost assumptions are credible;
- P2.04 constraint and uptime evidence determines achievable volume;
- P2.02 change control affects future requalification/change cost;
- supplier capability affects price, lead time and disruption risk;
- automation qualification affects launch timing and ramp risk.

The economic model should therefore consume evidence from the manufacturing system rather than invent optimistic inputs in isolation.

## 12. Listener tool — ECON 10

Before approving a manufacturing investment, ask:

1. **Demand** — what accepted volume and product mix are we actually planning for?
2. **Fixed** — what CapEx, tooling and NRE must be paid?
3. **Variable** — what changes per launched and per accepted unit?
4. **Yield** — how do scrap/rework/retest alter cost and capacity?
5. **Utilization** — how much of installed capacity will actually be used?
6. **Reliability** — what do downtime, maintenance, spares and recovery cost?
7. **Change** — what happens economically when the product changes?
8. **Time** — when are cash outflows and benefits realized?
9. **Uncertainty** — which assumptions can reverse the decision?
10. **Alternative** — what is the cheapest simpler architecture that solves the actual constraint?

## 13. Podcast guardrails

Do not teach:

- lowest labor content = lowest total cost;
- lowest variable cost = best process;
- NRE/forecast volume = complete unit economics;
- payback alone = complete investment analysis;
- automation savings without utilization/yield/maintenance assumptions;
- forecast volume as though it were guaranteed demand.

Prefer:

> Compare alternatives using the same system boundary, state the assumptions, connect economics to manufacturing evidence, and test the assumptions that can change the decision.

## 14. Evidence backbone

Primary external anchors for this pack:

- NIST Manufacturing Economics — manufacturing technology decisions include costs, losses, benefits and investment analysis.
- NIST AMS 200-5, *Investment Analysis Methods* — manufacturing investment methods including NPV and IRR.
- NIST AMS 200-9, *Manufacturing Cost Guide* — structured manufacturing cost estimation and potential-return analysis.
- NIST AMS 100-50 — empirical manufacturing investment study showing returns are unevenly distributed across investment types; bottleneck reduction and scheduling can be high-return interventions.

## 15. Next depth increment

Build a 5-year cash-flow comparison for Manual vs Semi-auto vs Automation with demand ramp, discount rate, maintenance, yield and downside scenarios. Then create a listener-facing process-selection decision tree linking economics to DEV/LVP/SVP maturity.
