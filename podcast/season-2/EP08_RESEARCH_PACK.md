# Episode 8 Research Pack — Design for Test, Calibration and Traceability

status: CLAIM SET STABLE
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: electronics, embedded, mechanical, NPI, manufacturing, quality, test
lifecycle: DEV → LVP → SVP
entry_point: DESIGNING FOR PRODUCTION
technical_depth: practitioner

## 1. Episode promise
Teach teams to design the product and production flow so every relevant unit can be programmed, calibrated, tested, identified and released without depending on engineering-only access or unreconstructable evidence.

Canonical listener question:
> How do we design today so production can prove tomorrow that each relevant unit was built, configured, calibrated and tested correctly?

## 2. Navigation card
**You are here:** DFM/DFA → test/calibration/traceability → tolerance/variation.
**Best for:** teams preparing repeated builds, custom PCBs, calibration, production test fixtures or serial/lot traceability.
**Prerequisite:** Episode 7 helpful, not mandatory.
**You will leave with:** Production Test Architecture Map + Unit Evidence Chain + Test-Debt Scan.
**Next:** Episode 9 Tolerance/GD&T/Variation → Episode 10 Reliability/Service/Repair.

## 3. Core thesis
Design for Test is not an end-of-line tester project. It starts with product architecture, access, observable states, firmware/configuration control, calibration strategy, identity and the claim each test is meant to support.

Production test creates release evidence only inside a defined product/test/measurement/configuration envelope. A PASS result is not stronger than the measurement system, procedure, configuration identity and reaction logic behind it.

## 4. Stable claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP08-C01 | Production testability is partly a product-design property because access, interfaces, states and observability are created by the design. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP08-C02 | Engineering debug access can accelerate DEV while hiding dependencies unsuitable for repeated production test. | P0 | BACKBONE-STABLE / A6 |
| EP08-C03 | A production test should protect a defined requirement/CTQ/failure-mode/release claim rather than exist only by habit. | P0 | BACKBONE-STABLE |
| EP08-C04 | Measurement adequacy must be established before strong pass/fail, trend or capability conclusions are drawn from test data. | P0 | GLOBAL INVARIANT / P2.03 / STABLE |
| EP08-C05 | Calibration values/procedure/version are part of product/configuration evidence when they materially affect product behavior or acceptance. | P0 | BACKBONE-STABLE / A8 |
| EP08-C06 | Relevant unit/lot identity should link the build, configuration, programming, calibration, test and deviation/rework evidence needed for release or field learning. | P0 | BACKBONE-STABLE |
| EP08-C07 | More testing does not automatically mean better quality; coverage should address consequential claims/failure modes while considering escape, false-reject, cycle and economic burden. | P1 | SYNTHESIS/BACKBONE STABLE |
| EP08-C08 | Production-test architecture should evolve with DEV→LVP→SVP rate, automation, traceability, measurement and recovery needs. | P1 | BACKBONE-SUPPORTED / STABLE |

Publication guardrail: no numeric MSA threshold, sampling plan, test-coverage target, calibration interval or regulated retention requirement enters the script without exact source/applicability verification.

## 5. Production Test Architecture Map
For each significant test/calibration step capture:
`Claim protected → identity/configuration → product state → access/interface → stimulus/reference → measurement system → acceptance/calibration criterion → data captured → fail/abort/fixture reaction → rework/retest history → cycle/rate burden → change trigger`.

## 6. Unit Evidence Chain
Internal framework:
`Unit/lot identity → product definition/configuration → programming/configuration → calibration → procedure/version → result/raw evidence → deviation/rework/retest → disposition/release`.

The discipline can begin with lightweight controlled records in LVP; enterprise MES is not a prerequisite.

## 7. Test-Debt Scan
Flag when:
- test requires engineering-only laptop/debug knowledge;
- test access disappears after an assembly/enclosure change;
- identity is assigned too late to connect relevant evidence;
- calibration constants exist only on a technician computer;
- procedure/version is not linked to result;
- retest leaves only final PASS and destroys prior fail/rework history;
- fixture self-check/reference strategy is undefined;
- criterion is tighter than credible measurement capability;
- test consumes rate but protects no explicit claim;
- HW/FW/process change can invalidate test meaning without impact review.

## 8. Worked example — Sentinel Node
DEV: engineer flashes over debug/USB, calibration script writes local constants, laptop log shows function, persistent identity is weak.

LVP direction: identity before relevant evidence; controlled HW/BOM/FW/configuration; repeatable programming; calibration procedure/version and constants linked to identity; functional acceptance tied to explicit claims; fail/rework/retest preserved; result linked to procedure/configuration.

The evidence chain is the requirement; this episode does not prescribe one database, MES or tester architecture.

## 9. DEV/LVP/SVP lens
**DEV:** optimize observability/debug speed; label engineering-only dependencies and calibration shortcuts.
**LVP:** introduce repeatable programming/calibration/test, identity, controlled criteria and traceable failure/rework history.
**SVP:** support intended rate, measurement-system control, fixture/reference recovery, version/effectivity, controlled automation and field-population reconstruction where required.

## 10. Boundary discipline
Episode 7 owns assembly architecture/mistake prevention. Episode 8 owns product testability, calibration and traceability architecture. Episode 9 owns tolerance/GD&T/variation. Episode 24 owns deeper MSA/production-testing methods. P2.08 owns full Manufacturing Atlas/data architecture.

## 11. Standards/source boundary
Potential source families include AIAG MSA where applicable, calibration/metrology standards, electronics-specific acceptance/test standards, and product-specific safety/compliance requirements. These are applicability-controlled source families, not universal requirements.

## 12. Applicability statement
General hardware DFT/calibration/traceability framework. Actual requirements vary by product risk, measurement needs, customer/regulatory obligations, software architecture, production rate and economics.

## 13. What this episode must NOT claim
- every unit needs every possible test;
- 100% functional test proves process capability;
- final test replaces upstream process control;
- calibration is always required;
- serial traceability automatically requires MES;
- final PASS erases prior fail/rework;
- test data are trustworthy without measurement-system consideration.

## 14. Evidence backlog after claim stabilization
1. Build authoritative DFT/calibration/traceability source map.
2. Verify any MSA/calibration/regulated claim before attribution.
3. Add representative mechanical/electrical/software examples without turning examples into universal rules.
4. Technical review: test + manufacturing/NPI + quality/metrology.

## 15. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: MEDIUM-HIGH
Quantitative burden: MEDIUM in later examples
Backbone risk: LOW
Claim set: STABLE
Source verification: CONTROLLED BACKLOG

Next status target: `CLAIM SET STABLE → EVIDENCE VERIFIED`
