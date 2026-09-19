# EP32 Script Outline V1 — Process Capability, SPC and Knowing Whether Production Is Stable

status: SCRIPT OUTLINE COMPLETE
season: Season 4 — Quality, Suppliers and the Reality of Scale
audience: quality / manufacturing / NPI / operations
lifecycle: LVP → SVP
source_lock: evidence/source-lock/wave-02/W2_EP23_EP24_EP32_EP39_EP40_CLAIM_LOCK.md
technical_review: evidence/source-lock/wave-02/W2_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-4/EP32_PRODUCTION_BLUEPRINT.md
entry: with short EP24 measurement recap

## Listener promise
By the end, the listener can separate three questions:
1. can I trust the measurement?
2. is the process behaving consistently over time?
3. if stable, is its distribution acceptable relative to specifications?

## Cold open
[ILLUSTRATIVE]
A dashboard says Cpk = 1.67. The team celebrates. The time-ordered data show the process shifted halfway through the run.

Question: Is one capability number allowed to compress an unstable process into a reassuring answer?

## Beat 1 — Variation is time-ordered behavior
Tags: [AUTH-GUIDANCE] [SYNTHESIS]
Claims: EP32-C01/C03
Narrative: do not reduce the process to pass/fail counts. Look at behavior over time.

## Beat 2 — Specification limits vs process-behavior/control limits
Tags: [AUTH-GUIDANCE]
Claims: EP32-C01
Sources: W2-S10
Explain:
- specifications come from engineering/customer requirements;
- control limits characterize expected process behavior under the chosen chart/model.
Guard: do not teach one universal chart construction/rule set.

## Beat 3 — Stable does not mean capable
Tags: [AUTH-GUIDANCE]
Claims: EP32-C02
Source: W2-S10
Example: stable process centered too close to a limit or with excessive spread.

## Beat 4 — In-spec does not mean stable
Tags: [SYNTHESIS]
Claims: EP32-C03
Sentinel sequence: all units remain inside 4.80–5.20 spec while the time series moves beyond illustrative process-behavior limits.
Lesson: investigate the process change before conformance necessarily fails.

## Beat 5 — Measurement adequacy first
Tags: [AUTH-GUIDANCE]
Claims: EP32-C07
Sources: W2-S07/W2-S09
One-minute recap from EP24.

## Beat 6 — Cp and Cpk
Tags: [AUTH-GUIDANCE] [ILLUSTRATIVE]
Claims: EP32-C05
Source: W2-S10
Formula:
Cp=(USL-LSL)/(6s)
Cpk=min[(USL-xbar)/(3s),(xbar-LSL)/(3s)]
Example:
LSL 4.80, USL 5.20, s 0.04.
mean 5.00 → Cp/Cpk ≈1.67.
mean 5.10 → Cp≈1.67, Cpk≈0.83.
Arithmetic: independently checked.
Guard: no universal threshold such as “1.33 is always good enough.”

## Beat 7 — Assumptions
Tags: [AUTH-GUIDANCE]
Claims: EP32-C04
Keep at practitioner level:
stable process evidence; suitable sampling; model/distribution fit; enough data for the conclusion; measurement adequacy.

## Beat 8 — Reaction plan
Tags: [SYNTHESIS]
Use fixture wear example:
signal → contain → verify measurement → inspect fixture/setup → find last-known-good → correct → verify restored behavior → disposition → update controls.

## Listener tool execution
Stability vs Capability Review:
CTQ → measurement adequate? → time order visible? → stable? → specification relation → centering/spread → capability calculation justified? → reaction.

## DEV / LVP / SVP
DEV: learn variation; avoid premature indices.
LVP: time-order data and detect process changes.
SVP: sustain statistical control/capability where justified, with explicit reaction plans and change control.

## Misconceptions
- high Cpk proves future quality.
- all in-spec = in control.
- stable = capable.
- control limits = tolerances.
- one capability threshold works for all customers.
- more decimals = more confidence.

## Closing action
Take one CTQ dashboard. If it shows only yield/Cpk and hides the time sequence, pull the raw chronological data before making the next process decision.

## Handoff
EP33 starts when the signal is real: how do we contain, disposition and correct without confusing closure of one unit with systemic correction?
