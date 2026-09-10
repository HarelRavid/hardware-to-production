# A1 Source Notes V1 — From an Idea to Engineering Requirements

status: SOURCE NOTES COMPLETE — READY FOR PODCAST READY GATE AFTER ONE SCRIPT WORDING PATCH
episode: A1 — From an Idea to Engineering Requirements
season: Season 1 — Build the Right Hardware Before Production Finds Your Mistakes
checked: 2026-09-10
script: `A1_SCRIPT_DRAFT_V1.md`
script_review: `A1_SCRIPT_REVIEW_V1.md`
source_lock: `evidence/source-lock/wave-01/W1_SHARED_SOURCE_REGISTER.md`
claim_lock: `evidence/source-lock/wave-01/W1_A1_A7_A8_CLAIM_LOCK.md`
source_notes_contract: `podcast/SOURCE_NOTES_CONTRACT.md`

## 1. Source-use statement

A1 is intentionally a practical early-hardware episode, not a standards lecture.

The spoken script relies on authoritative NASA systems-engineering guidance for the underlying engineering premises around requirements definition, traceability/change management and verification planning. The episode's listener tools, `Minimum Useful Requirements` language, uncertainty/TBD-expiration model and DEV/LVP/SVP framing are Hardware-to-Production synthesis.

ISO/IEC/IEEE 29148 is retained as standards context/current-status metadata only. No ISO clause-level normative statement is used in the spoken script.

## 2. Primary authoritative sources used

### A1-S01 — NASA Systems Engineering Handbook, Section 4.0 System Design Processes
Owner: NASA
Type: authoritative government technical guidance
Evidence class: V2
URL: https://www.nasa.gov/reference/4-0-system-design-processes/

Relevant areas:
- Stakeholder Expectations Definition;
- Technical Requirements Definition;
- requirement categories including functional, performance, interface and crosscutting constraints;
- requirement quality/verifiability guidance.

Episode use:
- supports the move from product intent to explicit technical requirements/constraints;
- supports discussion of interfaces, environment and safety-style constraints as engineering inputs;
- supports the premise that requirements need sufficient definition to permit determination of satisfaction.

Applicability:
NASA systems-engineering guidance. It is used as strong engineering support, not as a mandatory process imposed on commercial startups.

### A1-S02 — NASA Systems Engineering Handbook, Section 6.2 Requirements Management
Owner: NASA
Type: authoritative government technical guidance
Evidence class: V2
URL: https://www.nasa.gov/reference/6-0-crosscutting-technical-management/

Relevant areas:
- requirements identification/control/decomposition/allocation;
- bidirectional traceability;
- relationship among requirements, design and test plans/procedures;
- evaluation and control of requirement changes;
- impact assessment when baselined requirements change.

Episode use:
- supports the `Why/source/rationale` and traceability premise;
- supports the idea that once dependent engineering decisions exist, requirement changes should be visible and impact-assessed rather than silently edited.

Applicability:
The episode uses the engineering mechanism, not NASA program governance.

### A1-S03 — NASA Systems Engineering Handbook, Section 5.3 Product Verification
Owner: NASA
Type: authoritative government technical guidance
Evidence class: V2
URL: https://www.nasa.gov/reference/5-0-product-realization/

Relevant areas:
- verification against specified product requirements;
- planned procedures/conditions and appropriate enabling products/instrumentation;
- verification records linking requirements, product version/configuration, tools/equipment, procedures, conditions, results and discrepancies.

Episode use:
- supports adding a `verification idea` while requirements are still being developed;
- supports the general connection from requirement to future evidence.

Boundary:
A1 does not teach the full verification method. A7 owns that topic.

### A1-S04 — NASA Systems Engineering Handbook Appendix C/D
Owner: NASA
Type: authoritative guidance/templates
Evidence class: V2
URL: https://www.nasa.gov/reference/system-engineering-handbook-appendix/

Relevant areas:
- Appendix C: good-requirement guidance;
- Appendix D: Requirements Verification Matrix.

Episode use:
- supports the requirement-quality/verifiability premise;
- supports the usefulness of linking requirements to source and verification approach.

Boundary:
The `Requirement Quality Check` and `Minimum Useful Requirements Sheet` in A1 are not NASA forms and must be presented as Hardware-to-Production listener tools.

## 3. Standards context / revision watch

### ISO/IEC/IEEE 29148:2018
Title: `Systems and software engineering — Life cycle processes — Requirements engineering`
Edition: 2
Publication: 2018-11
Official ISO record: https://www.iso.org/standard/72089.html

Status checked: 2026-09-10.

Locked publication use:
- standard identity/title/edition/status/scope-level context only.

Not used:
- no exact clause-level SHALL statement;
- no claim that ISO/IEC/IEEE 29148 is contractually applicable to every hardware startup;
- no claim that A1's listener tools are ISO-defined.

Revision watch:
An Edition 3 DIS project is active in 2026. Draft record:
https://www.iso.org/standard/94091.html

Publication rule:
The draft must not be described as having replaced the published 2018 edition until official publication/transition information confirms that change.

## 4. Claim-to-source map

| Episode premise | Source | Class | Support location | Spoken use | Applicability guard |
|---|---|---|---|---|---|
| product/stakeholder intent must be translated into explicit technical requirements/constraints for coordinated engineering | A1-S01 | V2 + V6 | NASA SEH §4.1/§4.2 | yes | episode wording is practical synthesis, not NASA mandate |
| useful requirements should be sufficiently defined to permit verification/determination of satisfaction | A1-S01 + A1-S04 | V2 | NASA §4.2 + Appendix C/D | yes | no universal `shall`-syntax requirement |
| functional/performance/interface/environmental/safety-style constraints are legitimate requirement dimensions | A1-S01 | V2 | NASA §4.2 | yes | exact product/legal obligations remain product specific |
| traceability/source linkage and controlled change are useful when requirements drive dependent engineering | A1-S02 | V2 + V6 | NASA §6.2 | yes | lightweight implementation is ours |
| verification intent can be considered while requirements are developed | A1-S03 + A1-S04 | V2 | NASA §5.3 + Appendix D | yes | full verification ownership deferred to A7 |
| every startup should use our seven buckets/eight-question tool | none | V6 | internal | yes as our tool | explicitly not an external standard |

## 5. Internal synthesis / listener tools

The following are original/internal Hardware-to-Production packaging and are not attributed to NASA or ISO:
- `Minimum Useful Requirements` framing;
- seven-bucket practical organization;
- `CONFIRMED / TARGET / ASSUMPTION / TBD` implementation labels;
- assumption/TBD expiration trigger;
- Minimum Useful Requirements Sheet;
- eight-question Requirement Quality Check;
- `DEV → LVP → SVP` maturity framing;
- the rule that uncertainty is acceptable when visible/owned and dangerous when silently embedded in architecture.

These are V6 synthesis. Their embedded premises are source-supported where consequential, but the frameworks themselves remain ours.

## 6. Illustrative/fictional content declaration

### Opening scenario
The six-week hardware-team integration story is fictional/illustrative. It is not based on a named real company and must not be introduced as a documented case study.

### Sentinel Node
Sentinel Node is the repository's fictional recurring hardware product.
Its 24 VDC architecture, environmental assumptions, connector uncertainty and other example requirements are pedagogical design choices, not field data or universal product requirements.

## 7. Quantitative declaration

No engineering-significant factual number drives the A1 recommendation.

Numbers in the script are editorial/illustrative:
- `six weeks` — fictional opening;
- `seven buckets` — internal organization;
- `eight questions` — internal tool;
- `10–20 requirements` — practical exercise guidance;
- `20 minutes` — practical exercise guidance;
- `24 VDC` — Sentinel Node fictional architecture assumption.

These must not be described as validated thresholds.

## 8. Safety/regulatory applicability note

A1 says that possible safety/regulatory/environmental constraints should be surfaced early when they can alter architecture, materials, electrical design, enclosure, test or manufacturing choices.

This is an engineering-planning statement.

A1 does **not** determine:
- what regulation applies;
- what standard is mandatory;
- what certification is required;
- what specific safety test or acceptance criterion is correct.

Those claims require product, market, jurisdiction and role-specific source verification in later work.

## 9. Source-vs-synthesis language examples for final edit

Safe:
- `A useful requirement needs enough clarity that you can imagine how you would eventually know whether it is satisfied.`
- `NASA systems-engineering guidance treats requirements, traceability and verification as connected activities.` — only if NASA is explicitly named in a final optional source callout.
- `For this series, we will use a lightweight Minimum Useful Requirements Sheet.`

Avoid unless separately V1 locked:
- `ISO 29148 requires every startup to...`
- `The standard says every requirement must use this eight-question structure.`
- `All products must identify the following seven requirement categories.`

## 10. Publication re-check list

Before final publication:
1. confirm the official ISO 29148 record still identifies the 2018 edition as current, or update the status note if Edition 3 has been published;
2. confirm NASA source pages remain reachable or preserve stable handbook citation metadata;
3. verify no late script edit introduced a clause-level ISO claim;
4. verify no late script edit converted the safety/compliance watchlist into a generic legal requirement;
5. verify the one terminology patch from `A1_SCRIPT_REVIEW_V1.md` is incorporated in the recording/final script.

## 11. Remaining blockers

Technical/source blocker: NONE for current non-normative A1 script scope.

Editorial recording-lock blocker:
- replace `requirements baseline may contain targets...` with `working requirements set may contain targets...` in the DEV section.

Independent external human review:
- not claimed as completed; add one if the production policy later requires independent domain signoff before publication.

## 12. Gate

Primary authoritative evidence: LOCKED.
Source-vs-synthesis boundaries: EXPLICIT.
Standards revision watch: ACTIVE.
Quantitative claims: CONTROLLED.
Applicability: CONTROLLED.
Script/source-note alignment: PASS.

**A1 SOURCE NOTES V1: COMPLETE — READY FOR PODCAST READY GATE AFTER RECORDING WORDING PATCH**
