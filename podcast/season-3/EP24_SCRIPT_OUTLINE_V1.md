# EP24 Script Outline V1 — Production Testing and Measurement-System Capability

status: SCRIPT OUTLINE COMPLETE
season: Season 3 — Build the Factory Before You Need the Factory
audience: manufacturing / quality / test / NPI
lifecycle: LVP → Production Validation → Ramp
source_lock: evidence/source-lock/wave-02/W2_EP23_EP24_EP32_EP39_EP40_CLAIM_LOCK.md
technical_review: evidence/source-lock/wave-02/W2_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-3/EP24_PRODUCTION_BLUEPRINT.md
entry: standalone with measurement-language recap

## Listener promise
By the end, the listener can ask whether a production measurement or PASS/FAIL test is actually capable of supporting the decision it is being used to make.

## Cold open
[ILLUSTRATIVE]
Two stations measure the same connector seating depth and disagree. The process team starts adjusting the assembly fixture—but the dominant variation is fixture contact geometry, operator setup and the measurement method itself.

Question: Are we controlling the process—or reacting to the gauge?

## Beat 1 — Measurement system is more than the instrument
Tags: [AUTH-GUIDANCE]
Claims: EP24-C01
Sources: W2-S07/W2-S09
Narrative: NIST measurement-process characterization includes repeatability, reproducibility, stability and other conditions around the measurement process.
Teach: instrument + fixture + method + operator + environment + software/algorithm + reference state.

## Beat 2 — Repeatability and reproducibility
Tags: [AUTH-GUIDANCE]
Claims: EP24-C02
Source: W2-S08
Explain:
- repeatability: same conditions;
- reproducibility: changed conditions, and specify what changed.
Example: same operator repeated reads vs different operator/fixture orientation.

## Beat 3 — Calibration is necessary, but not the whole question
Tags: [AUTH-GUIDANCE] [SYNTHESIS]
Claims: EP24-C03
Sources: W2-S07/W2-S09
Guard: never say calibration is unimportant.
Example: calibrated gauge + poor contact datum + operator angle = decision variation.

## Beat 4 — Adequacy is decision-specific
Tags: [SYNTHESIS]
Claims: EP24-C04
Example: 0.1 mm resolution may be fine for rough screening and inadequate for a tighter discrimination decision.
No universal ratio/threshold.
Question: What wrong decision could this measurement cause?

## Beat 5 — Reference/golden units
Tags: [SYNTHESIS]
Guard: EP24-G03
Explain: a controlled reference unit can detect drift/change in a station, but it is not automatically a calibration standard.
Need identity, storage, expected response and change control.

## Beat 6 — Retest and history
Tags: [SYNTHESIS]
Claims: EP24-C05/C07
Wave 01 dependency: measurement/test software, fixture or acceptance-rule change can alter historical comparability.
A final PASS must not erase an earlier fail/retest path when that history matters.

## Beat 7 — Sentinel connector-depth worked example
Tags: [ILLUSTRATIVE]
Study pattern: representative parts, multiple operators, repeated readings.
Teach only the pattern: repeat differences + operator offset expose measurement contribution.
No GR&R acceptance percentage.
Improvement: hard datum, controlled orientation, constant force, work instruction, training, check standard, repeat study.

## Listener tool execution — Measurement Decision Chain
Claim/CTQ → method → instrument/fixture → reference/calibration → repeatability/reproducibility/stability → acceptance rule → reaction → data identity → change trigger.

## DEV / LVP / SVP
DEV: engineering measurement may be sufficient for learning if limits are visible.
LVP: repeatable fixture/method/identity becomes necessary.
SVP: maintenance, calibration, software/effectivity and ongoing measurement control must scale with rate/risk.

## Misconceptions
- calibrated = capable.
- digital display = objective truth.
- golden unit = calibration standard.
- one GR&R percentage works everywhere.
- tighter test limit always improves quality.
- retest PASS makes initial FAIL irrelevant.

## Closing action
Choose one production measurement that drives accept/reject. Ask three people to explain exactly how it is made and what could move the result. If the answers differ, the measurement system is not just the instrument.

## Handoff
EP32 later asks: once the measurement is trustworthy, is the process actually stable—and is it capable relative to the specification?
