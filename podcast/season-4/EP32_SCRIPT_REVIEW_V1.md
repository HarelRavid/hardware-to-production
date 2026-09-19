# EP32 Script Review V1 — Process Capability, SPC and Knowing Whether Production Is Stable

status: PASS TO SOURCE NOTES
review_date: 2026-09-19
script_reviewed: EP32_SCRIPT_DRAFT_V1.md
source_lock: evidence/source-lock/wave-02/
reviewer_type: internal technical/editorial review; independent external human review not claimed

## Decision
The script is statistically sound at the intended practitioner level and preserves the required assumptions/threshold guardrails.

**PASS TO SOURCE-NOTE PACKAGING.**

## Technical findings
- Specification limits vs control/process-behavior limits: PASS.
- Stable vs capable distinction: PASS.
- In-spec vs stable distinction: PASS.
- Measurement adequacy prerequisite: PASS.
- Cp formula: VERIFIED against NIST.
- Cpk formula: VERIFIED against NIST.
- Sentinel arithmetic: independently checked and correct.
- Normality/model/sample-size caveat: present at appropriate level.
- No universal Cpk acceptance threshold: PASS.
- 2026 AIAG/VDA SPC manual used only as current automotive method context: PASS.

## Quantitative audit
Illustrative inputs:
LSL 4.80 mm; USL 5.20 mm; s=0.04 mm.
Centered mean 5.00 mm: Cp=Cpk≈1.67.
Shifted mean 5.10 mm: Cp≈1.67; Cpk≈0.83.
Arithmetic: PASS.
Data status: fictional/pedagogical.

## Recording-lock guards
- Do not add “Cpk 1.33 = capable” or any generic threshold.
- Do not present illustrative 3-sigma process limits as a universal control-chart construction method.
- Do not add universal Western Electric/AIAG/VDA signal rules without source lock.
- Preserve model/distribution/sample assumptions.

## Gate
Architecture change: NO.
New source required for current script: NO.
Source notes can be generated: YES.

**EP32 SCRIPT REVIEW V1: PASS TO SOURCE NOTES**
