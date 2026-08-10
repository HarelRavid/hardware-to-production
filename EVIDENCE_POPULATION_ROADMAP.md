# Phase 2 — Evidence Population & Verification Roadmap

status: ACTIVE
version: 1.1
started_on: 2026-08-09
updated_on: 2026-08-10

## Objective
Move from architecture-defined knowledge structure to source-backed, scoped and Podcast-Ready engineering knowledge.

## Architecture maturity terminology
- **DEFINED** — coherent conceptual architecture exists.
- **EVIDENCE VALIDATED** — important architecture/engineering claims have been checked against authoritative evidence with applicability limits.
- **IMPLEMENTATION VALIDATED** — architecture has been exercised against a representative implementation/reference dataset and conflict/failure cases.

Architecture V1.0 closure records that the canonical structure is DEFINED; it does not imply evidence or implementation validation.

## Prioritization model
Each work package should be ranked by:
- podcast/editorial value
- engineering decision importance
- risk of misleading guidance if wrong
- current evidence gap
- standards/regulatory relevance
- cross-domain leverage
- availability of strong primary sources

## Priority A — Foundational cross-domain evidence
1. Early hardware development / Opening Arc
2. Product development / NPI / EVT-DVT-PVT / production readiness
3. DFM / DFA / DFT foundational methods
4. Process-selection frameworks and lifecycle economics
5. Quality foundations: PFMEA/control plans/MSA/SPC/capability
6. Pilot/PVT/ramp/yield/capacity definitions and evidence
7. Supplier industrialization / qualification / change control
8. Automation business case / qualification / OEE boundaries
9. Manufacturing Data Hub semantic and integration standards
10. OT/ICS cybersecurity for connected manufacturing environments

## Priority B — Manufacturing-process standards and evidence
For each process family in Section 3:
- applicable standards/specifications
- primary handbooks/books
- peer-reviewed research
- manufacturer/industry guidance
- quantitative design/process windows
- defect/failure evidence
- inspection/qualification methods
- automation/cost evidence
- case studies

Recommended population order for podcast leverage:
1. Machining & Material Removal
2. Joining
3. Injection Molding
4. Metal Casting
5. Metal Forming
6. Additive Manufacturing
7. Heat Treatment
8. Surface Engineering
9. Cleaning/Contamination Control
10. Composites
11. Polymer Forming Beyond Injection
12. Rubber/Elastomers
13. Ceramics/Powder-Based Manufacturing
14. Process Integration

## Priority C — Standards extraction & applicability
Create/maintain clause-level Standard Objects for standards that materially support episode-critical claims or engineering decisions.

Minimum metadata:
- standard ID/title
- issuing body
- edition/revision/date
- status/current/superseded
- scope/applicability
- relevant clauses
- normative/informative role
- claims/decisions supported or bounded
- supersession/history

### Applicability Statement reference implementations
Build at least two worked examples during Phase 2:
1. **Process/requirement example:** ISO 21307 or another suitably bounded manufacturing standard, demonstrating Standard -> Clause/Evidence -> Claim -> Applicability Statement -> Decision linkage.
2. **System/integration example:** ISA-95/IEC 62264 or IEC 62443, demonstrating applicability across system boundary, role, context and architecture decision.

The purpose is to validate the Applicability Statement object and workflow, not to imply that these standards apply universally.

## Priority D — Claim verification campaign
For each domain:
1. enumerate GNR claims;
2. rank by importance/risk;
3. search for suitable sources;
4. attach evidence and applicability;
5. preserve conflicts;
6. update evidence maturity;
7. leave unsupported claims visibly open rather than smoothing them into prose.

## Priority E — Case studies
Target case studies that teach transferable decisions rather than only famous stories:
- hardware launch failures
- manufacturing debt in startups
- tolerance/capability failures
- supplier scale failures
- automation-too-early failures
- design-for-assembly/test successes
- yield/ramp recoveries
- process-change failures
- traceability/quality escapes
- OT/ICS integration/security failures where lessons are relevant to connected production systems

## Priority F — Podcast Research Packs
Use PODCAST_MAP.md as editorial priority, but do not promote an episode to Podcast Ready until:
- critical claims have suitable evidence;
- standards applicability is checked where relevant;
- conflicts/assumptions are explicit;
- quantitative examples are scoped;
- at least one useful case/example is included where appropriate;
- show-note sources are assembled.

## Dedicated OT/ICS evidence package
Before the Manufacturing Data/AI/Security podcast arc is Podcast Ready, create an evidence package covering as applicable:
- IEC 62443 family structure and applicability;
- zones/conduits and segmentation;
- identity/access for users, machines and services;
- remote/vendor access;
- IT/OT boundary design;
- secure write-back to operational systems;
- patch/change/configuration constraints;
- logging/monitoring/incident response;
- safety/security interaction;
- applicability to startups/LVP versus larger SVP environments.

## Phase 2 operating rhythm
### Pass 1 — Breadth
Populate high-authority source maps and identify episode-critical claims across all major domains.

### Pass 2 — Depth
Perform clause-level standards extraction, quantitative evidence and case-study research for highest-priority decisions.

### Pass 3 — Synthesis
Build decision frameworks, Research Packs and scripts; promote mature Objects to Podcast Ready.

## Evidence quality rule
Do not maximize source count. Prefer the smallest sufficient set of strong, applicable sources that supports the engineering claim and makes limitations visible.

## Completion criteria for Phase 2
Phase 2 is substantially complete when the priority podcast sequence can be produced from Research Packs whose critical engineering claims meet the Knowledge OS Podcast Ready gate.