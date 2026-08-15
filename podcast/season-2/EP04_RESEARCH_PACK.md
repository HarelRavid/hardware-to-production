# Episode 4 Research Pack — Product Readiness vs Manufacturing Readiness

status: RESEARCH PACK OPEN
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: NPI, manufacturing, quality, engineering leads, operations, supply chain
lifecycle: DEV → LVP → SVP
entry_point: READINESS DECISION FOUNDATION
technical_depth: foundation-practitioner

## 1. Episode promise
Give hardware teams a practical way to separate evidence that the product design is ready for its intended use from evidence that the production system can repeatedly build and accept it.

Canonical listener question:
> Can the product be technically ready while manufacturing is not — or manufacturing look stable while the product itself is still changing?

## 2. Navigation card
**You are here:** build maturity/NPI ownership → readiness evidence → lifecycle gates.

**Best for:** teams preparing pilot/LVP commitments, design releases, supplier/tooling decisions or readiness reviews.

**Prerequisite:** none mandatory. Episodes 1–3 recommended.

**You will leave with:** Product-vs-Manufacturing Readiness Matrix + Readiness Evidence Review.

**Next:** Episode 5 EVT/DVT/PVT/Pilot/Ramp → Episode 6 DFM.

## 3. Core thesis
Product readiness and manufacturing readiness are coupled but not identical.

A design may satisfy important functional/verification claims while process, supplier, test, measurement, yield or capacity evidence remains immature. Conversely, a factory may execute a stable process for a product configuration that is still changing or insufficiently verified.

The release decision must therefore inspect multiple evidence dimensions rather than compressing readiness into one label or percentage.

## 4. Draft claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP04-C01 | Product readiness and manufacturing readiness are distinct but interacting evidence domains. | P0 | BACKBONE-SUPPORTED |
| EP04-C02 | A successful product verification result does not by itself prove manufacturing capability. | P0 | BACKBONE-STABLE |
| EP04-C03 | A stable production process does not prove the underlying product configuration satisfies all intended product claims. | P0 | BACKBONE-STABLE |
| EP04-C04 | Readiness should be assessed across dimensions rather than collapsed into one maturity score. | P0 | BACKBONE-SUPPORTED |
| EP04-C05 | Supplier, measurement/test, process capability, configuration, rate and economics may mature independently. | P1 | BACKBONE-SUPPORTED |
| EP04-C06 | Readiness evidence must be tied to a defined configuration/process/applicability envelope. | P0 | BACKBONE-STABLE |
| EP04-C07 | The evidence threshold depends on the next commitment: another DEV build, LVP release, customer qualification, ramp or SVP. | P0 | SYNTHESIS/BACKBONE |
| EP04-C08 | Readiness gaps should generate owned closure actions rather than a cosmetic red/yellow/green score. | P1 | SYNTHESIS |

## 5. Hardware Manufacturing Readiness Matrix
Keep two major columns visible rather than merging them.

### Product evidence dimensions
- requirements/CTQs;
- architecture/interfaces;
- released configuration;
- functional/performance verification;
- reliability/environment;
- safety/compliance applicability;
- service/repair where relevant.

### Manufacturing evidence dimensions
- process route/window;
- supplier/source readiness;
- tooling/fixtures/equipment;
- work method/training;
- measurement/inspection/test/calibration;
- traceability/configuration execution;
- yield/rework/defect learning;
- capacity/rate;
- cost per good unit/economics;
- change/effectivity/recovery.

For each dimension record:
`Claim → Current evidence → Gap → Owner → Next decision → Required closure evidence`.

Do not average the matrix into a single readiness percentage.

## 6. Readiness Evidence Review
Ask:
1. What is the exact next commitment?
2. Which product claims must be demonstrated before it?
3. Which manufacturing claims must be demonstrated before it?
4. Which dimensions may legitimately remain provisional?
5. Are product and manufacturing evidence tied to the same configuration?
6. What supplier/process/test changes are still expected?
7. Which gap has the highest consequence if carried into the next stage?
8. Who owns closure and what evidence closes it?

## 7. Worked example — Sentinel Node
Product side may be strong: sensing performance, firmware behavior and enclosure function verified on a bounded configuration.

Manufacturing side may remain weak: connector insertion variation, calibration station repeatability, supplier lot traceability, yield/rework learning and rate evidence.

Decision: the product may be ready for a controlled LVP learning build without being ready for unrestricted serial ramp.

The opposite can also occur: a repeatable assembly line may exist while a late firmware/thermal/interface change invalidates product evidence.

## 8. DEV/LVP/SVP lens
### DEV
Readiness means enough evidence to justify the next learning investment.

### LVP
Readiness increasingly means bounded/released configuration plus controlled process/test/supplier learning across a population.

### SVP
Readiness requires product and manufacturing evidence to coexist inside a controlled commercial operating envelope, including change/recovery discipline.

## 9. Applicability statement
The Hardware Manufacturing Readiness Matrix is an internal podcast framework, not a claimed external maturity standard. Industry/customer readiness systems may impose named levels, gates or mandatory evidence and must be handled through explicit applicability/source verification.

## 10. What this episode must NOT claim
- one readiness score can prove launch readiness;
- product verification equals process capability;
- process capability equals product compliance;
- every dimension must reach the same maturity simultaneously;
- a pilot or phase label proves readiness;
- our matrix is an ISO/industry standard.

## 11. Research backlog before CLAIM SET STABLE
1. Cross-check P2.01/P2.04 readiness architecture.
2. Verify no overlap with Episode 2 build maturity and Episode 5 lifecycle gates.
3. Add authoritative readiness/manufacturing evidence sources only where externally attributed.
4. Technical review: product/systems + NPI/manufacturing + quality.

## 12. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: LOW-MEDIUM
Quantitative burden: LOW
Backbone risk: LOW
Source verification: OPEN

Next status target:
`RESEARCH PACK OPEN → CLAIM SET STABLE`
