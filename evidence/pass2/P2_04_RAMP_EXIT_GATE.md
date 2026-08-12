# P2.04 — Pilot / PVT / Run-at-Rate / Ramp Exit Gate

**Status:** NEAR PODCAST READY — canonical gate drafted
**Purpose:** Convert pilot and run-at-rate evidence into a disciplined decision on whether a production system is ready to ramp.

## 1. Core distinction

A successful pilot batch is not the same as demonstrated rate. Demonstrated rate is not the same as sustainable capacity. Sustainable capacity is not the same as readiness to ramp.

The decision chain is:

**Pilot/PVT learning → representative run-at-rate → sustained capacity evidence → ramp exit decision**

## 2. Evidence boundary

A ramp decision should state the operating envelope actually demonstrated:
- product/configuration and revision,
- supplier/material state,
- production route and tooling,
- staffing and skill assumptions,
- shift pattern and available production time,
- demand/rate target,
- product mix and changeovers,
- inspection/test content,
- rework routing,
- maintenance assumptions,
- duration of demonstrated operation.

Evidence outside this envelope is not automatically transferable.

## 3. Canonical Ramp Exit Gate

### Gate A — Product definition is sufficiently controlled
PASS evidence:
- production-intent configuration is released,
- known deviations are dispositioned and visible,
- effectivity/cut-in is controlled,
- as-built genealogy can identify what was actually produced.

### Gate B — Production process is representative
PASS evidence:
- production-intent equipment/tooling/fixtures are used or differences are explicitly bounded,
- normal operators perform the work,
- controlled work instructions are used,
- normal inspection/test route is active,
- normal material presentation and logistics are represented.

### Gate C — Measurement and quality controls are trustworthy
PASS evidence:
- CTQs and acceptance criteria are defined,
- measurement systems are adequate for their decisions,
- control/reaction plans exist for critical characteristics and failure modes,
- yield, scrap and rework are measured consistently,
- unresolved quality escapes do not invalidate the run.

### Gate D — Rate is demonstrated at the system constraint
PASS evidence:
- demand and available time define takt,
- constraint is identified from observed flow rather than assumed station design rates,
- accepted throughput at the system boundary meets the required rate,
- rework load on constrained resources is included,
- the result is not created by hidden engineering intervention or pre-staging.

### Gate E — Flow is sustainable
PASS evidence:
- WIP/queue does not grow without bound during the demonstrated window,
- downstream operations consume upstream output at sustainable rates,
- rework backlog remains controlled,
- changeovers and replenishment do not create accumulating production debt.

### Gate F — Availability and recovery are represented
PASS evidence:
- realistic minor stops and downtime are included,
- failure/restart/recovery behavior is understood,
- maintenance and spare assumptions are defined,
- recovery does not depend on extraordinary expert support that will not exist in serial production.

### Gate G — Supply can support the demonstrated envelope
PASS evidence:
- critical suppliers/materials are qualified for the configuration used,
- lead-time and replenishment assumptions are credible,
- shortages are not being hidden by one-time pilot inventory,
- substitutions are under change control.

### Gate H — Economics are visible
PASS evidence:
- labor content is measured rather than estimated only from routing standards,
- scrap/rework/inspection burden is included,
- bottleneck and overtime assumptions are visible,
- current unit economics and the expected ramp trajectory are separated.

### Gate I — Learning loop is closing
PASS evidence:
- pilot/run findings create owned corrective actions,
- PFMEA/control plan/work instructions/tooling/training are updated where appropriate,
- effectiveness is verified,
- known production debt is explicitly accepted or scheduled.

### Gate J — Duration is sufficient for the claim
PASS evidence:
- the duration is long enough to expose the failure modes relevant to the decision,
- replenishment, breaks, operator rotation, rework and routine disturbances are represented where material,
- the team states what the run did *not* demonstrate.

## 4. Decision outcomes

Do not reduce the gate to PASS/FAIL only.

**GREEN — Ready to ramp inside demonstrated envelope**
Evidence supports controlled ramp at the defined configuration, rate and operating assumptions.

**AMBER — Conditional ramp**
Specific gaps remain, but risk is bounded. Define owner, containment, due date, monitoring metric and explicit stop condition.

**RED — Not ready to ramp**
A critical gate is unproven or contradicted by evidence: e.g. unstable queue growth, untrusted measurement, uncontrolled configuration, insufficient constraint capacity, unresolved critical quality issue, or supply incapable of supporting rate.

## 5. Sentinel Node worked decision

Target: 80 accepted units / 420 net production minutes.
Takt: 315 s/unit.
Observed Calibration + Functional Test cycle: 360 s/unit.
Illustrative availability: 90%.
Observed upstream launch rate: ~11.43 units/hour.
Effective test cycles at 90% availability: ~9 units/hour.
Queue growth before rework: ~2.43 units/hour.

Decision: **RED for ramp to 80 accepted units/shift** even if a short interval reached target launch rate.

Reason:
- the system constraint cannot sustainably consume upstream flow,
- WIP grows during the run,
- rework further consumes constraint capacity,
- short-burst rate therefore overstates sustainable system capacity.

Possible routes to GREEN are not prescribed by the gate; engineering may reduce test cycle, add validated parallel capacity, improve FPY/rework load, change demand/shift assumptions, or redesign the test strategy. Each option must be re-evaluated against quality, economics and representativeness.

## 6. Listener tool — RAMP 10

Before approving ramp, ask:
1. What exact rate and accepted-output target are we claiming?
2. What configuration and production envelope produced the evidence?
3. Where is the actual system constraint?
4. Does accepted throughput meet demand after availability and quality losses?
5. Is WIP stable, falling, or growing?
6. How much constraint capacity is consumed by rework?
7. Were normal operators, tooling, instructions, logistics and inspection used?
8. What downtime, changeovers and replenishment occurred during the run?
9. Which production risks remain open, and what stops the ramp if they worsen?
10. Was the run long enough to justify the claim we are making?

## 7. Podcast guardrails

Never equate:
- one good batch with process capability,
- launch rate with accepted throughput,
- station cycle time with system capacity,
- peak rate with sustained rate,
- completed run-at-rate with unrestricted production readiness,
- zero visible queue at the end of a staged demo with stable flow.

Use wording such as **“demonstrated within this operating envelope”** rather than universal claims.

## 8. Evidence anchors

- NASA NPR 7123.1C PRR: production readiness concerns efficiently producing the required number of systems and includes production plans, critical process controls, resources, BOM/critical parts, inspection/test readiness and manufacturability.
- Prior P2.04 worked examples: takt/constraint/capacity model; WIP/queue and rework recursion; run-at-rate scorecard.

## 9. P2.04 readiness assessment

P2.04 now contains:
- quantitative takt/constraint/capacity worked example,
- availability/yield/rework treatment,
- queue/WIP growth example,
- rework recursion concept,
- run-at-rate scorecard,
- canonical Ramp Exit Gate,
- Sentinel Node decision example,
- listener-facing RAMP 10 tool.

**Assessment: NEAR PODCAST READY.**
Remaining work before episode packaging: technical review, source-note normalization, and mapping the canonical claims/tools to the relevant episode IDs.