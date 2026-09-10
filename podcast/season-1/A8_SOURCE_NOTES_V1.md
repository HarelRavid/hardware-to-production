# A8 Source Notes V1 — Configuration Management from Prototype #1

status: SOURCE NOTES COMPLETE — READY FOR PODCAST READY GATE
episode: A8
checked: 2026-09-10
script: `A8_SCRIPT_DRAFT_V1.md`
script_review: `A8_SCRIPT_REVIEW_V1.md`
source_lock: `evidence/source-lock/wave-01/W1_SHARED_SOURCE_REGISTER.md`
claim_lock: `evidence/source-lock/wave-01/W1_A1_A7_A8_CLAIM_LOCK.md`

## Source-use statement

A8 uses NASA configuration-management, requirements-management and product-verification guidance for the underlying engineering premises. The episode's lightweight startup implementation, `Definition / As-built-As-run / Evidence` model, Change Impact Check and rework-history wording remain Hardware-to-Production synthesis.

## Primary source

### A8-S01 — NASA Systems Engineering Handbook, Section 6.5 Configuration Management
Owner: NASA
Evidence class: V2
URL: https://www.nasa.gov/reference/6-0-crosscutting-technical-management/

Relevant support:
- CM as a life-cycle discipline for visibility/control of product characteristics and changes;
- five elements: planning/management, identification, change management, status accounting and verification;
- configuration identification and baselines;
- systematic change proposal/evaluation, incorporation and verification of implementation;
- current/historical configuration status accounting.

Applicability:
NASA systems-engineering guidance. A8 transfers reconstructability/change-control mechanisms; it does not prescribe NASA program governance to commercial startups.

## Supporting sources

### A8-S02 — NASA SEH Section 5.3 Product Verification
URL: https://www.nasa.gov/reference/5-0-product-realization/
Use: product/requirements/tool/procedure/version context and discrepancy/corrective-action history in verification records.

### A8-S03 — NASA SEH Section 6.2 Requirements Management
URL: https://www.nasa.gov/reference/6-0-crosscutting-technical-management/
Use: requirement traceability/change impact and preservation of controlled relationships.

## Standards context

### ISO 10007:2017
Title: `Quality management — Guidelines for configuration management`
Edition: 3
Publication: 2017-03
Official ISO record: https://www.iso.org/standard/70400.html
Status checked: 2026-09-10.

Use in A8:
- standard identity/current-status/scope-level context only;
- public ISO summary may corroborate the high-level CM process family.

Not used:
- no detailed clause-level requirement/guideline is spoken;
- no claim that every startup must implement ISO 10007 formally.

Revision watch:
Edition 4 draft/revision project is active in 2026:
https://www.iso.org/standard/92170.html

## Claim-to-source map

| Episode premise | Source | Class | Spoken use | Guard |
|---|---|---|---|---|
| CM includes identification, change, status/history and verification rather than only revision control | A8-S01 | V2 | yes | NASA guidance, not commercial mandate |
| evidence should remain connected to product/configuration context | A8-S01/A8-S02 | V2 + V6 | yes | exact three-object model is ours |
| approved change requires implementation/control and applicable verification | A8-S01 | V2 | yes | specific startup sequence is synthesis |
| consequential rework/deviation history should remain visible | A8-S02 + V6 | V2 premise + synthesis | yes | not every minor touch-up requires formal NCR |
| revision vs effectivity | V6 | synthesis | yes | do not attribute exact definition to ISO/NASA |
| supplier alternate can affect prior evidence | P2.06 dependency | synthesis preview | yes | no universal requalification requirement |

## Internal synthesis/tools

Original Hardware-to-Production constructs:
- `Definition → As-built/As-programmed/As-run → Evidence` model;
- Minimum Prototype Configuration Record;
- Change Impact Check;
- `rework adds history` invariant wording;
- practitioner `revision vs effectivity` explanation;
- Five-Build Reconstruction Challenge;
- DEV/LVP/SVP configuration maturity framing.

## Illustrative content

Opening two-prototype scenario: fictional.
Sentinel Node sensor substitution: fictional canonical worked example.

## Quantitative declaration

No factual engineering threshold is used.
The five-build challenge is an editorial exercise quantity, not a statistical threshold.

## Applicability / transfer limits

A8 is general hardware configuration/evidence guidance.
Formal CM, traceability, release, change approval and record-retention requirements vary by industry, customer, contract and jurisdiction.

Supplier-specific approval/requalification requirements are intentionally deferred to P2.06 and the supplier episodes.

## Publication re-check

Before publication:
1. confirm ISO 10007 edition/current status if named in public show notes;
2. ensure no late edit presents the three-object model as NASA/ISO terminology;
3. ensure `revision vs effectivity` remains practitioner synthesis unless separately locked;
4. ensure supplier-alternate wording remains impact-based rather than universal requalification;
5. preserve the statement that record depth is risk/evidence dependent.

## Gate

Source evidence: LOCKED.
Applicability: CONTROLLED.
Standards wording: CONTROLLED.
Quantitative burden: NONE at current scope.
Script/source alignment: PASS.

**A8 SOURCE NOTES V1: COMPLETE — READY FOR PODCAST READY GATE**
