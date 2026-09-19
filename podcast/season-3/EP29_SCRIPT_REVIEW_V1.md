# EP29 Script Review V1 — Capacity, Bottlenecks, Takt Time and Line Balance

status: PASS TO SOURCE NOTES
review_date: 2026-09-19
script_reviewed: EP29_SCRIPT_DRAFT_V1.md
source_lock: evidence/source-lock/wave-03/
reviewer_type: internal technical/editorial + quantitative review; independent external human review not claimed

## Decision
The script is quantitatively coherent and preserves the required distinction among demand pace, process time, throughput and sustainable capacity.

PASS TO SOURCE-NOTE PACKAGING.

## Technical findings
- takt definition: PASS against LEI.
- cycle-time definition: PASS.
- candidate bottleneck vs true constraint: PASS.
- availability/yield/rework modeling: PASS as illustrative model.
- WIP/queue interpretation: PASS.
- Little's Law boundary: PASS; script explicitly avoids transient-prediction misuse.
- moving constraint: PASS as synthesis.
- capacity-before-CapEx: PASS.

## Quantitative audit
80 accepted units / 420 min:
takt = 315 s/unit — PASS.

25,200/360:
70 theoretical cycles — PASS.

90% availability:
22,680 s / 360 = 63 cycles — PASS.

92% FPY:
63×0.92 = 57.96 first-pass accepted — PASS.

First-order rework burden:
360 + 0.08×240 = 379.2 s — PASS.

Demand arrival:
80/7 h = 11.4286/h.
Illustrative service:
10/h×0.90 = 9/h.
Difference:
≈2.43/h queue growth before rework — PASS.

## Recording-lock guards
- 420 min is an illustrative planned-time basis, not a standard;
- longest nominal cycle is not automatically system bottleneck;
- queue arithmetic is simplified deterministic illustration;
- no universal run-at-rate duration;
- no universal capacity margin;
- do not let Little's Law imply WIP creates throughput.

## Gate
Quantitative blockers: 0.
New P0 source required: NO.
Source notes: YES.

EP29 SCRIPT REVIEW V1: PASS TO SOURCE NOTES.
