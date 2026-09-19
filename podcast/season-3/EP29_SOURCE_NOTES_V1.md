# EP29 Source Notes V1 — Capacity, Bottlenecks, Takt Time and Line Balance

status: SOURCE NOTES COMPLETE — READY FOR WAVE 03 PUBLICATION GATE
checked: 2026-09-19
script: EP29_SCRIPT_DRAFT_V1.md
script_review: EP29_SCRIPT_REVIEW_V1.md
source_lock: evidence/source-lock/SOURCE_LOCK_WAVE_03_RAMP_ECONOMICS_REGISTER.md

## Primary sources
### EP29-S01 — Lean Enterprise Institute, Takt Time
https://www.lean.org/lexicon-terms/takt-time/
Supports available production time / customer demand.

### EP29-S02 — Lean Enterprise Institute, Cycle Time
https://www.lean.org/lexicon-terms/cycle-time/
Supports cycle time as actual measured process/part time.

### EP29-S03 — NIST Manufacturing Analytical Services
https://tsapps.nist.gov/publication/get_pdf.cfm?pub_id=920909
Supports WIP/throughput/cycle-time relationships, Little's Law usage and utilization/queue effects.

### EP29-S04 — NIST TN 1890
https://www.nist.gov/publications/inventory-and-flow-time-us-manufacturing-industry

### EP29-S05 — NIST capital-investment sources
https://www.nist.gov/el/applied-economics-office/manufacturing/capital-investment-analysis
https://www.nist.gov/publications/efficiency-improvements-us-manufacturing-return-investment-small-and-medium

## Quantitative declaration
All numbers are illustrative and independently checked:
- 80 accepted / 420 min → 315 s takt.
- 25,200/360 → 70 theoretical cycles.
- 90% availability → 63 cycles.
- 92% FPY → 57.96 first-pass accepted.
- 360+0.08×240 → 379.2 s first-order burden.
- 80/7 h → 11.4286 arrivals/h.
- 9 cycles/h simplified service → ≈2.43/h queue growth before rework.

## Guardrails
420 min is example time basis, not a standard.
Longest nominal cycle is not always system bottleneck.
Little's Law is not a transient queue predictor or reason to add WIP.
No universal Run-at-Rate duration or capacity margin.

## Internal synthesis
RATE 8, Capacity Reality Sheet, accepted-throughput priority and moving-constraint loop are Hardware-to-Production frameworks.

**EP29 SOURCE NOTES V1: COMPLETE**
