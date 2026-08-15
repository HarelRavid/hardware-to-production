# Episode 8 Research Pack — Design for Test, Calibration and Traceability

status: RESEARCH PACK OPEN
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: electronics, embedded, mechanical, NPI, manufacturing, quality, test
lifecycle: DEV → LVP → SVP
entry_point: DESIGNING FOR PRODUCTION
technical_depth: practitioner

## 1. Episode promise
Teach teams to design the product and production flow so every unit can be programmed, calibrated, tested, identified and released without depending on engineering-only access or unreconstructable evidence.

Canonical listener question:
> How do we design today so production can prove tomorrow that each unit was built, configured, calibrated and tested correctly?

## 2. Navigation card
**You are here:** DFM/DFA → test/calibration/traceability → tolerance/variation.
**Best for:** teams preparing repeated builds, custom PCBs, calibration, production test fixtures or serial traceability.
**Prerequisite:** Episode 7 helpful, not mandatory.
**You will leave with:** Production Test Architecture Map + Unit Evidence Chain + Test-Debt Scan.
**Next:** Episode 9 Tolerance/GD&T/Variation → Episode 10 Reliability/Service/Repair.

## 3. Core thesis
Design for Test is not an end-of-line tester project. It starts with product architecture, access, signals, firmware states, calibration strategy, serial identity and the claim each test is meant to support.

A production test system should create useful evidence for release while remaining compatible with production rate, measurement capability, configuration control and traceability.

## 4. Draft claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP08-C01 | Production testability is partly a product-design property because access, interfaces, states and observability are created by the design. | P0 | BACKBONE-SUPPORTED |
| EP08-C02 | Engineering debug access can accelerate DEV while hiding dependencies that are unsuitable for repeated production test. | P0 | BACKBONE-STABLE / A6 |
| EP08-C03 | A production test should be tied to a defined release/quality claim rather than exist only because “we always test this.” | P0 | BACKBONE-STABLE |
| EP08-C04 | Measurement adequacy must precede strong pass/fail or capability conclusions. | P0 | GLOBAL INVARIANT / P2.03 |
| EP08-C05 | Calibration is part of configuration/product evidence when its values materially affect product behavior. | P0 | BACKBONE-STABLE / A8 |
| EP08-C06 | Serial/lot/unit identity should link relevant build, programming, calibration, test and deviation/rework evidence where those records matter to release or field learning. | P0 | BACKBONE-STABLE |
| EP08-C07 | More tests do not automatically create better quality; test coverage should target meaningful failure modes/claims and be evaluated against cost, escape risk and false reject burden. | P1 | SYNTHESIS/BACKBONE |
| EP08-C08 | Production-test architecture must evolve with DEV→LVP→SVP rate, automation, traceability and recovery needs rather than be treated as a one-time fixture decision. | P1 | BACKBONE-SUPPORTED |

## 5. Production Test Architecture Map
For each significant test/calibration step capture:
| Field | Question |
|---|---|
| Claim protected | What requirement/CTQ/failure mode does the step address? |
| Unit identity | What serial/lot/configuration is under test? |
| Product state | What HW/FW/configuration/operating state is required? |
| Access/interface | Test points, connector, optical/mechanical access, network/debug path? |
| Stimulus | What input/load/environment/reference is applied? |
| Measurement | What is measured and with what adequacy? |
| Criterion | What is pass/fail/calibration acceptance logic? |
| Data captured | Raw data, summary, calibration constants, trace? |
| Reaction | What happens on fail/abort/fixture fault? |
| Rework/retest | How is original fail history preserved? |
| Cycle/rate burden | Does the step fit intended production flow? |
| Change trigger | What product/process/test change requires review? |

## 6. Unit Evidence Chain
Internal framework:
`Unit/lot identity → product definition/configuration → programming/configuration → calibration → test procedure/version → result/raw evidence → deviations/rework → disposition/release`.

The chain can be implemented in lightweight tools in early LVP; enterprise MES is not required to establish the discipline.

## 7. Test-Debt Scan
Flag any of these:
- test requires engineering laptop or hidden debug command;
- test access disappears after enclosure/assembly change;
- unit identity is assigned after test rather than before relevant evidence;
- calibration constants live only on a technician's computer;
- test procedure/version is not tied to result;
- fail/retest leaves only final PASS;
- fixture self-check/reference method is undefined;
- criterion is tighter than credible measurement capability;
- test adds cycle time but protects no explicit claim;
- software/HW change can invalidate test meaning without impact review.

## 8. Worked example — Sentinel Node programming/calibration/final test
DEV flow:
- engineer flashes firmware over USB/debug;
- calibration script writes constants locally;
- laptop log confirms function;
- no persistent unit identity.

LVP-ready direction:
- unit ID assigned before relevant programming/test;
- controlled HW/BOM/FW/configuration identity;
- repeatable programming interface;
- calibration procedure/version and constants linked to unit;
- functional test tied to explicit acceptance claims;
- fail/rework/retest preserved;
- result stored with traceable procedure/configuration.

The episode must not prescribe one database or tester architecture; the evidence chain is the requirement.

## 9. DEV/LVP/SVP lens
**DEV:** optimize observability/debug speed; label engineering-only dependencies and calibration shortcuts.
**LVP:** introduce repeatable programming/calibration/test, unit identity, controlled criteria and traceable fail/rework history.
**SVP:** support rate, automated data capture where justified, measurement-system control, fixture recovery, version/effectivity and field-population reconstruction.

## 10. Boundary discipline
Episode 7 owns assembly architecture/mistake prevention. Episode 8 owns product testability, calibration and traceability architecture. Episode 9 owns tolerance/GD&T/variation. Episode 24 owns deeper MSA/production-testing methods. P2.08 owns full Manufacturing Atlas/data architecture.

## 11. Standards/source burden
Potential source families depend on final script claims: AIAG MSA for measurement-system methodology where applicable; IPC/J-STD/industry product test standards for electronics-specific acceptance; calibration/metrology standards; product-specific safety/compliance test standards.

No numeric MSA threshold, sampling plan, test coverage target, calibration interval or regulated record requirement enters the script without exact source/applicability verification.

## 12. Applicability statement
General hardware DFT/calibration/traceability framework. Actual production-test requirements vary by product risk, measurement needs, customer/regulatory obligations, software architecture, rate and economic trade-offs.

## 13. What this episode must NOT claim
- every unit needs every possible test;
- 100% functional test proves process capability;
- final test replaces upstream process control;
- calibration is always required;
- serial traceability automatically requires MES;
- a final PASS erases prior fail/rework;
- test data are trustworthy without measurement-system consideration.

## 14. Research backlog before CLAIM SET STABLE
1. Cross-check P2.03, P2.08 and A6/A8 boundaries.
2. Build authoritative DFT/calibration/traceability source map.
3. Select representative mechanical/electrical/software test examples.
4. Verify any MSA/calibration/regulated claims before external attribution.
5. Technical review: test + manufacturing/NPI + quality/metrology.

## 15. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: MEDIUM-HIGH
Quantitative burden: MEDIUM in later examples
Backbone risk: LOW
Source verification: OPEN

Next status target: `RESEARCH PACK OPEN → CLAIM SET STABLE`
