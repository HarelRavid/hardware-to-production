# A7 Source Notes V1 — Verification Planning Before DVT/PVT Thinking

status: SOURCE NOTES COMPLETE — READY FOR PODCAST READY GATE
episode: A7
checked: 2026-09-10
script: `A7_SCRIPT_DRAFT_V1.md`
script_review: `A7_SCRIPT_REVIEW_V1.md`
source_lock: `evidence/source-lock/wave-01/W1_SHARED_SOURCE_REGISTER.md`
claim_lock: `evidence/source-lock/wave-01/W1_A1_A7_A8_CLAIM_LOCK.md`

## Source-use statement

A7 uses NASA systems-engineering guidance to support the evidence architecture of product verification. The Verification Intent Sheet, exploratory-vs-release framing, claim-specific representativeness reuse and impact-based re-verification logic remain Hardware-to-Production synthesis unless explicitly sourced otherwise.

## Primary source

### A7-S01 — NASA Systems Engineering Handbook, Section 5.3 Product Verification
Owner: NASA
Evidence class: V2
URL: https://www.nasa.gov/reference/5-0-product-realization/

Episode-supported premises:
- verification is performed against specified product requirements;
- verification uses planned methods/procedures/conditions and enabling products/instrumentation;
- verification records preserve requirement version, product version, tools/equipment/data context, procedures/environments, results and discrepancies;
- verification and validation answer different questions.

Applicability:
NASA authoritative systems-engineering guidance. The podcast transfers the evidence discipline; it does not impose NASA program governance on commercial hardware teams.

## Supporting sources

### A7-S02 — NASA SEH Section 4.2 Technical Requirements Definition
URL: https://www.nasa.gov/reference/4-0-system-design-processes/
Use: requirements should be sufficiently defined/verifiable; verification intent can influence requirement quality.

### A7-S03 — NASA SEH Section 6.2 Requirements Management
URL: https://www.nasa.gov/reference/6-0-crosscutting-technical-management/
Use: traceability, managed requirement change and impact assessment.

### A7-S04 — NASA SEH Appendix D Requirements Verification Matrix
URL: https://www.nasa.gov/reference/system-engineering-handbook-appendix/
Use: requirement/source/verification-method linkage.

## Claim-to-source map

| Episode premise | Source | Evidence class | Spoken use | Guard |
|---|---|---|---|---|
| verification evidence is meaningful only with defined requirement/product/method/context records | A7-S01 | V2 + V6 | yes | compact wording is synthesis |
| verification planning connects to requirements before late-stage test | A7-S02/A7-S04 | V2 | yes | no claim that every DEV requirement needs formal procedure |
| verification and validation are distinct | A7-S01 | V2 | yes | do not use validation as `more serious test` |
| change can require new verification where affected | A7-S01/A7-S03 | V2 + V6 | yes | exact dependency algorithm is ours |
| measurement adequacy precedes strong conclusions | P2.03 dependency | V6 preview | yes, principle only | no MSA numeric thresholds |
| one passing unit does not automatically prove process capability/population behavior | V6/P2.03 dependency | synthesis | yes | do not claim one unit can never verify anything |

## Standards context

ISO/IEC/IEEE 29148:2018 may be listed in show notes as current requirements-engineering context as checked 2026-09-10. No clause-level ISO requirement is used in A7 narration.

## Internal synthesis/tools

Not external standards:
- Verification Intent Sheet;
- Evidence-to-Claim Review;
- exploration vs release-evidence practical framing;
- claim-specific applicability wording;
- dependency-based re-verification rule;
- DEV/LVP/SVP implementation.

## Illustrative content

Opening environmental-test scenario: fictional.
Sentinel Node sealing/connector verification example: fictional canonical worked example.

## Quantitative declaration

No evidence-derived quantitative threshold is used.
No sample-size, GR&R, capability or reliability criterion is taught.

## Publication re-check

Before publication:
1. confirm NASA source pages/handbook reference remains available;
2. verify no late edit converts internal re-verification logic into a NASA/ISO requirement;
3. verify no late edit adds MSA/sample-size thresholds without P2.03 source lock;
4. preserve verification-vs-validation wording.

## Gate

Source evidence: LOCKED.
Applicability: CONTROLLED.
Quantitative burden: NONE at current scope.
Script/source alignment: PASS.

**A7 SOURCE NOTES V1: COMPLETE — READY FOR PODCAST READY GATE**
