# Episode 4 Research Pack — Product Readiness vs Manufacturing Readiness

status: CLAIM SET STABLE
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: NPI, manufacturing, quality, engineering leads, operations, supply chain
lifecycle: DEV → LVP → SVP
entry_point: READINESS DECISION FOUNDATION
technical_depth: foundation-practitioner

## 1. Episode promise
Separate evidence that the product design is ready for its intended claim from evidence that the production system can repeatedly build, verify and release it.

Canonical listener question:
> Can the product be technically ready while manufacturing is not — or manufacturing look stable while the product itself is still changing?

## 2. Navigation card
**You are here:** build maturity/NPI ownership → readiness evidence → lifecycle gates.
**Best for:** teams preparing pilot/LVP commitments, design releases, supplier/tooling decisions or readiness reviews.
**Prerequisite:** none mandatory. Episodes 1–3 recommended.
**You will leave with:** Product-vs-Manufacturing Readiness Matrix + Readiness Evidence Review.
**Next:** Episode 5 lifecycle gates → Episode 6 DFM.

## 3. Core thesis
Product readiness and manufacturing readiness are coupled but not identical. A product claim can be well supported while process, supplier, measurement, yield or capacity evidence remains immature. Conversely, a repeatable process can build the wrong, changing or insufficiently verified configuration very consistently.

The decision therefore needs a multidimensional evidence view tied to the exact next commitment.

## 4. Stable claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP04-C01 | Product readiness and manufacturing readiness are distinct but interacting evidence domains. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP04-C02 | Product verification does not by itself establish repeatable manufacturing capability. | P0 | BACKBONE-STABLE |
| EP04-C03 | Stable manufacturing execution does not establish that the product configuration satisfies all intended product claims. | P0 | BACKBONE-STABLE |
| EP04-C04 | Readiness should remain multidimensional rather than being inferred from one maturity percentage. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP04-C05 | Supplier, measurement/test, process, configuration, rate and economics may mature at different speeds. | P1 | BACKBONE-SUPPORTED / STABLE |
| EP04-C06 | Readiness evidence must be tied to a defined product/process/configuration/applicability envelope. | P0 | BACKBONE-STABLE |
| EP04-C07 | Required evidence depends on the next commitment: learning build, LVP release, qualification, ramp or SVP. | P0 | SYNTHESIS/BACKBONE STABLE |
| EP04-C08 | Readiness gaps should create owned closure actions and evidence requirements rather than cosmetic status alone. | P1 | SYNTHESIS STABLE |

## 5. Hardware Manufacturing Readiness Matrix
This is an internal framework, not an external maturity standard.

**Product evidence:** requirements/CTQs; architecture/interfaces; configuration; functional/performance verification; reliability/environment; safety/compliance applicability; service/repair where relevant.

**Manufacturing evidence:** process route/window; supplier/source; tooling/equipment; work method/training; measurement/inspection/test/calibration; traceability/configuration execution; yield/rework; capacity/rate; cost per good unit; change/effectivity/recovery.

For every dimension record:
`Claim → Current evidence → Gap → Owner → Next decision → Required closure evidence`.

Never average the matrix into a single readiness percentage.

## 6. Readiness Evidence Review
1. What is the exact next commitment?
2. Which product claims must be demonstrated before it?
3. Which manufacturing claims must be demonstrated before it?
4. Which dimensions may legitimately remain provisional?
5. Are product and manufacturing evidence tied to the same configuration?
6. What supplier/process/test changes remain expected?
7. Which carried gap has the highest consequence?
8. Who owns closure and what evidence closes it?

## 7. Sentinel Node example
Sensing performance, firmware behavior and enclosure function may be verified on a bounded configuration while connector insertion variation, calibration-station repeatability, supplier traceability, yield/rework learning and rate evidence remain weak. That can justify a controlled LVP learning build without justifying unrestricted serial ramp.

The inverse is possible too: repeatable assembly can exist while a late firmware, thermal or interface change invalidates product evidence.

## 8. DEV/LVP/SVP lens
**DEV:** enough evidence to justify the next learning investment.
**LVP:** bounded/released configuration plus controlled process/test/supplier learning across a population.
**SVP:** product and manufacturing evidence coexist within a controlled commercial envelope, including change and recovery discipline.

## 9. Boundary discipline
Episode 2 owns build maturity/representativeness. Episode 3 owns industrialization responsibility. Episode 4 owns readiness dimensions and evidence gaps. Episode 5 owns phase/gate language. Later episodes own detailed capability, pilot and ramp methods.

## 10. Applicability statement
The Hardware Manufacturing Readiness Matrix is an internal podcast framework. Industry/customer readiness systems may impose named levels, gates or mandatory evidence; those require explicit source verification and applicability.

## 11. What this episode must NOT claim
- one readiness score proves launch readiness;
- product verification equals process capability;
- process capability equals product compliance;
- all dimensions must mature simultaneously;
- a pilot/phase label proves readiness;
- this matrix is an ISO or industry standard.

## 12. Evidence backlog after claim stabilization
1. Verify any external maturity/readiness framework before attribution.
2. Add source support for product/manufacturing evidence concepts where useful.
3. Technical review: product/systems + NPI/manufacturing + quality.
4. Keep detailed capability/ramp mathematics in their dedicated episodes.

## 13. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: LOW-MEDIUM
Quantitative burden: LOW
Backbone risk: LOW
Claim set: STABLE
Source verification: CONTROLLED BACKLOG

Next status target: `CLAIM SET STABLE → EVIDENCE VERIFIED`
