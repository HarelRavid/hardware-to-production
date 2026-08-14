# A1 Source Verification Note — Requirements Engineering

status: SOURCE VERIFICATION STARTED
supports: `podcast/pilot/A1_RESEARCH_PACK.md`
date_checked: 2026-08-14

## 1. Purpose

Stabilize the A1 claim set using authoritative requirements-engineering sources without turning the episode into a standards lecture.

The episode remains a lightweight startup-facing synthesis. External sources support the underlying engineering premises; the listener tools and DEV/LVP/SVP framing remain internal synthesis.

## 2. Primary sources located

### S-A1-01 — NASA Systems Engineering Handbook / Appendix D: Requirements Verification Matrix

Source owner: NASA
Source type: authoritative government systems-engineering guidance
Evidence class: V2
Status: SOURCE LOCATED / usable for technical support

Relevant support:
- NASA states that when developing requirements, an approach for verifying the requirements should be identified.
- NASA's example verification matrix identifies each requirement, its source and how it will be verified.
- NASA's V&V-plan guidance distinguishes verification methods including test, analysis, inspection and demonstration.

A1 use:
- supports A1-C02: requirements should be expressed/managed so satisfaction can be determined by a verification approach;
- supports A1-C03 in part: requirement identity/source and verification linkage are useful controlled records;
- supports A1-C09 boundary: verification evidence must be planned and is not equivalent to every later production-acceptance activity.

Guardrail:
NASA guidance is not presented as a contractual requirement for all commercial hardware startups.

### S-A1-02 — ISO/IEC/IEEE 29148:2018

Official title: `Systems and software engineering — Life cycle processes — Requirements engineering`
Edition: 2
Publication: 2018-11
Official status checked: Published/current edition; ISO states it was reviewed and confirmed in 2024.
ISO lifecycle status: `To be revised`.
Evidence class: V1 for any normative claim; V2-style discovery support until licensed/full text is available.

Official ISO abstract states that the document specifies requirements-engineering processes and related information items and provides guidance for applying requirements-related life-cycle processes. Its stated applicability includes systems, software-intensive systems, software and hardware products and related services.

A1 use:
- candidate authoritative source for exact terminology/characteristics of requirements;
- candidate source for traceability/information-item claims;
- not necessary for the episode's lightweight one-page listener tool unless an exact normative statement is made.

Acquisition note:
Full licensed text should be added to the controlled standards acquisition workflow before clause-level P0 claims are marked VERIFIED.

### S-A1-03 — ISO/IEC/IEEE DIS 29148, Edition 3 draft

Official status checked: under development / Draft International Standard.
Edition: 3 draft
ISO project status checked 2026-08-14: DIS registered; ISO shows the revision project active in 2026.

A1 use:
- standards-library/change-watch only;
- must NOT be cited as the current published normative edition while it remains a draft.

## 3. Claim mapping after first verification pass

| Claim | Previous status | New evidence state | Decision |
|---|---|---|---|
| A1-C01 | UNVERIFIED | SUPPORTED, not yet clause-level | Keep as synthesis supported by systems-engineering guidance; do not make it sound normative. |
| A1-C02 | UNVERIFIED | STRONGLY SUPPORTED | NASA directly supports planning a verification approach while developing requirements. Exact universal wording still avoided. |
| A1-C03 | UNVERIFIED | PARTIALLY SUPPORTED | NASA verification-matrix/source linkage supports controlled identity/source/verification linkage. Broader bidirectional traceability awaits full source packaging. |
| A1-C04 | UNVERIFIED | OPEN | Keep as engineering synthesis until interface-focused primary/academic support is packaged. |
| A1-C05 | SYNTHESIS | SYNTHESIS | No need to force external normative support; retain as DEV guidance. |
| A1-C06 | UNVERIFIED | OPEN | Product-neutral principle is plausible, but safety/regulatory source should be selected by episode use; avoid generic legal claims. |
| A1-C07 | UNVERIFIED | BACKBONE-SUPPORTED | Keep mapped to P2.03; episode should preview CTQ concept rather than normatively define it. |
| A1-C08 | UNVERIFIED | BACKBONE-SUPPORTED | Keep mapped to P2.02 configuration/change logic; exact CM source packaging can occur before script-ready. |
| A1-C09 | UNVERIFIED | PARTIALLY SUPPORTED | NASA V&V structure supports distinct verification activities; production-acceptance distinction remains our lifecycle synthesis. |
| A1-C10 | SYNTHESIS | SYNTHESIS | Internal Hardware Evolution Ladder framing. |

## 4. Standards-status finding that must remain visible

As of 2026-08-14:

- `ISO/IEC/IEEE 29148:2018` remains the current published edition according to ISO and was confirmed in 2024.
- ISO also lists it as `to be revised`.
- an Edition 3 DIS is under development in 2026.

Therefore any future standards library should retain both:
1. the licensed/current 2018 edition for normative verification while it remains current; and
2. a revision-watch record for Edition 3.

Do not silently replace the current standard with the draft.

## 5. A1 source-vs-synthesis boundary

Externally supportable engineering premises:
- requirements engineering is a lifecycle activity;
- verification approach should be considered while requirements are developed;
- requirements can be uniquely identified and linked to verification/source records;
- verification may use test, analysis, inspection or demonstration depending on the requirement.

Internal podcast synthesis:
- Minimum Useful Requirements Sheet;
- Requirement Quality Check;
- bounded DEV assumptions/TBDs with explicit expiration;
- DEV → LVP → SVP maturity framing;
- shortcut-expiration rules;
- startup-scale implementation guidance.

## 6. Remaining P0 work before EVIDENCE VERIFIED

1. Obtain/licence the full current ISO/IEC/IEEE 29148 text if exact normative claims will be used.
2. Add exact clause/page references for any 29148 claim that reaches the final script.
3. Select source support for early safety/regulatory/environmental constraint awareness only if the script makes a consequential claim beyond common engineering framing.
4. Reuse P2.02/P2.03 verified source packs for configuration-change and CTQ boundaries instead of duplicating standards research.
5. Technical systems-engineering review.

## 7. Status recommendation

A1 is now suitable for:

`RESEARCH PACK OPEN → CLAIM SET STABLE`

Reason:
- core episode thesis is supported;
- source-vs-synthesis boundary is explicit;
- standards status is controlled;
- remaining verification work is visible and does not require claim-set redesign.

It is NOT yet EVIDENCE VERIFIED or SCRIPT READY.
