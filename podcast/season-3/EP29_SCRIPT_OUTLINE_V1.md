# EP29 Script Outline V1 — Capacity, Bottlenecks, Takt Time and Line Balance

status: SCRIPT OUTLINE COMPLETE
season: Season 3 — Build the Factory Before You Need the Factory
audience: NPI / manufacturing / operations / automation / finance
lifecycle: Production Validation → Ramp
source_lock: evidence/source-lock/wave-03/W3_EP26_EP27_EP28_EP29_EP30_EP31_CLAIM_LOCK.md
technical_review: evidence/source-lock/wave-03/W3_INTERNAL_TECHNICAL_REVIEW.md
blueprint: podcast/season-3/EP29_PRODUCTION_BLUEPRINT.md

## Listener promise
Calculate demand pace, identify the real current constraint, include downtime/yield/rework/WIP, and distinguish burst speed from sustainable accepted throughput.

## Cold open
[ILLUSTRATIVE] Every station looks fast enough on the stopwatch, yet calibration queues grow and customer demand is missed.

## Beat 1 — Takt starts with demand
Claims: EP29-C01
Source: W3-S04.
Example: 80 accepted units / 420 min → 315 s/unit.
Guard: time basis explicit.

## Beat 2 — Cycle time is observed process time
Source: W3-S05.
Do not confuse takt and cycle time.

## Beat 3 — Candidate bottleneck vs true system constraint
Claims: EP29-C02/C04
Sources: W3-S06/S07.
Longest nominal cycle is a candidate, not automatic truth.

## Beat 4 — Sentinel nominal capacity
360 s constraint → 70 theoretical cycles/shift.
At 90% availability → 63 cycles.
At 92% FPY → 57.96 first-pass accepted.
Tags: [ILLUSTRATIVE] arithmetic verified.

## Beat 5 — Rework loads the constraint
Claims: EP29-C06
First-order burden 360 + 0.08×240 = 379.2 s launched-unit-equivalent before repeat loops.

## Beat 6 — WIP and queue growth
Claims: EP29-C07
Source: W3-S06.
Demand arrival ≈11.43/h; simplified service ≈9/h → +2.43/h queue before rework.
Guard: simplified deterministic illustration, not transient queue prediction.

## Beat 7 — Little's Law guard
Use average stable-system relationship only; do not teach WIP as a capacity lever.

## Beat 8 — Moving constraint
Claims: EP29-C05
After improving test, re-measure; constraint may move to assembly/material/test-data upload.

## Beat 9 — Capacity before CapEx
Claims: EP29-C09
Sources: W3-S10/S11/S14.
Compare flow improvement, shifts/labor, parallelization and automation; do not automate a forecast.

## Listener tool — Capacity Reality Sheet / RATE 8
Demand → time → constraint → availability → yield/rework → queues → representativeness → duration.

## Misconceptions
- takt = cycle time;
- longest nominal cycle always bottleneck;
- fastest observed cycle = capacity;
- WIP raises capacity;
- final good output makes rework free;
- 30-minute target-rate burst proves run-at-rate.

## Closing action
At your current bottleneck, calculate accepted units per hour after downtime and rework—not nominal cycles per hour.

## Handoff
EP30 asks whether suppliers and contract manufacturers can support the same rate/evidence envelope.