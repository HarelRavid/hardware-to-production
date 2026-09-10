# Wave 01 Shared Source Register

status: VERIFIED SOURCE REGISTER
checked: 2026-09-10
supports: A1, A7, A8, P2.02 and downstream reuse where claim/applicability match

## S-W1-01 — NASA Systems Engineering Handbook, Section 4.0 System Design Processes

Owner: NASA
Evidence class: V2 authoritative technical guidance
URL: https://www.nasa.gov/reference/4-0-system-design-processes/

### Exact support used
**Section 4.1 / Stakeholder Expectations Definition**
NASA guidance identifies constraints as conditions that must be met and notes that constraints may arise from external interfaces, regulatory restrictions, technology state and other factors.

**Section 4.2 / Technical Requirements Definition**
NASA describes technical requirements as a recursive/iterative translation of stakeholder expectations into validated technical requirements used to define the design solution.

**Section 4.2.1.2.2 / Define Requirements**
NASA identifies requirement families including functional, performance, interface and crosscutting requirements. The crosscutting examples include environmental, safety and human-factor requirements.

**Section 4.2.1.2.3 / Define Requirements in Acceptable Statements**
NASA guidance states that requirements should be sufficiently defined to be verifiable and points to guidance/checklists for well-written requirements.

### Claims supported
- A1-C01 premise: intent must be translated into explicit engineering requirements/constraints before coordinated design.
- A1-C02 premise: requirements should support a determination of whether they are satisfied.
- A1-C04 support: interfaces are explicit technical-requirement objects and need controlled definition.
- A1-C06 premise: environmental/safety/regulatory constraints can be architecture/design inputs.

### Applicability
NASA systems-engineering guidance. Used here as authoritative engineering support, not as a legal or contractual requirement for commercial hardware teams.

---

## S-W1-02 — NASA Systems Engineering Handbook, Section 6.2 Requirements Management

Owner: NASA
Evidence class: V2
URL: https://www.nasa.gov/reference/6-0-crosscutting-technical-management/

### Exact support used
**Section 6.2 opening / Requirements Management Process**
NASA states that requirements management is used to identify/control/decompose/allocate requirements, provide bidirectional traceability, and manage changes to established requirement baselines over the product life cycle.

**Section 6.2.1.2.2 / Conduct Requirements Management**
NASA describes maintaining traceability among stakeholder/customer/product/component requirements, design documents and test plans/procedures; evaluating change requests; and maintaining consistency with architecture/design.

**Section 6.2.1.2.3 / Conduct Expectations and Requirements Traceability**
NASA states that each documented requirement should have traceability to a parent/source requirement or be identified as self-derived with appropriate concurrence.

**Section 6.2.1.2.4 / Managing Expectations and Requirement Changes**
NASA states that changes should be evaluated for impacts across cost, schedule, architecture, design, interfaces, ConOps and requirements, and subjected to review/approval to preserve traceability and impact assessment.

### Claims supported
- A1-C03: source/requirement/downstream traceability premise.
- A1-C08: once requirements are baselined and dependent engineering decisions exist, change should be treated as a controlled impact-assessment event rather than invisible editing.
- A7-C02: verification/requirements linkage should be considered while requirements are managed, not invented only at the end.
- A8-C05 premise: change requires impact assessment against affected dependencies.
- P2.02 change-impact backbone.

### Applicability
NASA process guidance; commercial implementation may be lighter. The transferable engineering mechanism is traceability + impact-aware change control.

---

## S-W1-03 — NASA Systems Engineering Handbook, Section 5.3 Product Verification

Owner: NASA
Evidence class: V2
URL: https://www.nasa.gov/reference/5-0-product-realization/

### Exact support used
**Section 5.3.1.2 / verification execution and analysis**
NASA describes verification against specified product requirements using planned procedures and appropriate enabling products/instrumentation.

**Section 5.3.1.2.4 / Capture Product Verification Work Products**
NASA guidance states that verification records should capture method, procedures, environments, outcomes, decisions, assumptions, corrective actions and lessons learned.

The verification report content described by NASA includes:
- version of the specified requirements used;
- version of the product verified;
- version/standard for tools, data and equipment used;
- pass/fail results;
- discrepancies.

**Section 5.3.1.3 / Outputs**
NASA describes verification reports as linking requirement, traceability, verification method, equipment/conditions/procedures, results and anomalies/corrective actions.

**Section 5.3.2 / Product Verification Guidance**
NASA distinguishes verification (objective evidence that specified requirements were met) from validation (the product meets intended customer/user expectations in intended use/environment).

### Claims supported
- A1-C02 verification-path premise.
- A1-C09 support for verification as an evidence activity distinct from broader validation/production acceptance synthesis.
- A7-C01: evidence meaning depends on defined claim/configuration/conditions/method.
- A7-C02: verification is planned against requirements.
- A7-C08: verification evidence should preserve product/configuration/procedure identity.
- A8-C01/C02/C06: evidence must remain connected to product/version/tool/procedure context.

### Reverification support
NASA states that when mitigation of a nonconformance changes the product, verification may need to be planned/performed again. Hardware-to-Production's **impact-based targeted reverification rule** remains internal synthesis; NASA is not cited as saying every affected dependency should be treated exactly by our algorithm.

### Applicability
Authoritative NASA guidance. The commercial podcast extracts evidence architecture, not NASA program governance.

---

## S-W1-04 — NASA Systems Engineering Handbook, Section 6.5 Configuration Management

Owner: NASA
Evidence class: V2
URL: https://www.nasa.gov/reference/6-0-crosscutting-technical-management/

### Exact support used
**Section 6.5 opening**
NASA describes configuration management as a life-cycle discipline for visibility/control of functional and physical characteristics and changes, keeping product/documentation/configuration information consistent.

**Section 6.5.1.2**
NASA identifies five CM elements:
1. configuration planning and management;
2. configuration identification;
3. configuration change management;
4. configuration status accounting;
5. configuration verification.

**Section 6.5.1.2.2 / Identify Baseline to be Under Configuration Control**
NASA describes configuration identification as selecting/organizing/stating product attributes and using unique identifiers. A baseline is described as an agreed product description at a point in time against which changes are addressed.

**Section 6.5.1.2.3 / Manage Configuration Change Control**
NASA describes change management as systematic proposal, justification and evaluation, followed by incorporation of approved changes and verification of implementation.

NASA also distinguishes engineering changes from waivers within its program terminology.

**Section 6.5.1.2.4 / Maintain the Status of Configuration Documentation**
NASA describes configuration status accounting as recording/reporting the configuration data required to manage configuration items and preserve current/historical status.

### Claims supported
- A8-C01: evidence/configuration linkage premise.
- A8-C02: product definition and actual/versioned evidence must remain traceably consistent.
- A8-C05 premise: change is impact-controlled and implementation verified.
- P2-C-CM-001 support.
- P2-C-CM-003 strong support.
- P2-C-CM-005 NASA-specific terminology support.

### Important synthesis boundaries
NASA is **not** being cited as the source of:
- our `Definition → As-built/As-run → Evidence` three-object model;
- `rework adds history` wording;
- startup spreadsheet/Git implementation;
- our exact Change Impact Check;
- our targeted evidence-invalidation algorithm.

Those remain V6 synthesis informed by the source family.

---

## S-W1-05 — NASA Systems Engineering Handbook Appendix C/D

Owner: NASA
Evidence class: V2
URL: https://www.nasa.gov/reference/system-engineering-handbook-appendix/

### Exact support used
**Appendix C — How to Write a Good Requirement**
NASA provides requirement quality and validation guidance.

**Appendix D — Requirements Verification Matrix**
NASA provides a matrix structure connecting requirements, source and verification approach/method.

### Claims supported
- A1-C02 and A1-C03.
- A7 verification-planning structure.

### Applicability
Guidance/template evidence only; Hardware-to-Production listener tools are separately authored and should not be presented as NASA templates.

---

## S-W1-06 — NPR 7123.1D, NASA Systems Engineering Processes and Requirements

Owner: NASA Office of the Chief Engineer
Evidence class: V1 **only within NASA applicability**; V2/contextual support for our public commercial podcast
Current record checked: 2026-09-10
Effective date: 2023-07-05
Expiration date shown by NASA: 2028-07-05
URL: https://nodis3.gsfc.nasa.gov/displayDir.cfm?Internal_ID=N_PR_7123_001D_&page_name=main

### Use
This source is used mainly to lock the **applicability boundary**: NASA procedural requirements are mandatory within their stated NASA scope. They are not silently generalized into obligations for commercial startups.

### Rule
If a future script says `NASA requires`, the exact NPR section and applicability must be verified. If the script says `hardware teams generally must`, NASA procedural language alone is insufficient.

---

## S-W1-07 — ISO/IEC/IEEE 29148:2018 official record

Owner: ISO/IEC/IEEE
Evidence class: V1 metadata/status; normative clauses NOT LOCKED in this repository
Reference: ISO/IEC/IEEE 29148:2018
Title: Systems and software engineering — Life cycle processes — Requirements engineering
Edition: 2
Publication: 2018-11
URL: https://www.iso.org/standard/72089.html
OBP overview: https://www.iso.org/obp/ui#iso:std:iso-iec-ieee:29148:ed-2:v1:en

### Status checked 2026-09-10
- 2018 Edition 2 remains the published standard.
- ISO lifecycle shows active revision work.
- Edition 3 DIS is under development: https://www.iso.org/standard/94091.html

### Locked use
- title/edition/status/scope-level description;
- confirmation that the standard addresses requirements engineering for systems/software and related products/services.

### Not locked
No clause-level SHALL claim is verified by this record alone.

---

## S-W1-08 — ISO 10007:2017 official record

Owner: ISO
Evidence class: V1 metadata/status; clause-level normative/guidance text NOT LOCKED
Reference: ISO 10007:2017
Title: Quality management — Guidelines for configuration management
Edition: 3
Publication: 2017-03
URL: https://www.iso.org/standard/70400.html
ISO committee summary: https://committee.iso.org/sites/tc176/home/projects/published/iso-10007-2017.html

### Status checked 2026-09-10
- ISO 10007:2017 remains the published edition.
- revision work is active.
- Edition 4 working-draft project is under development: https://www.iso.org/standard/92170.html

### Public committee-summary support
The ISO committee summary identifies a configuration-management process including planning, configuration identification, change control, configuration status accounting and configuration audit.

### Locked use
- title/edition/status/scope;
- high-level process-family corroboration.

### Not locked
No detailed clause-level requirement/guideline is treated as verified without controlled full-text access.

---

## S-W1-09 — NASA Technology Readiness Levels current public page

Owner: NASA
Evidence class: V2
URL: https://www.nasa.gov/directorates/somd/space-communications-navigation-program/technology-readiness-levels/
Page last updated by NASA: 2026-06-25 (as checked 2026-09-10)

### Use
Supports P2.01's distinction that TRL is a technology-maturity scale. It does **not** support manufacturing-readiness, supplier, rate, quality or cost conclusions.

### Boundary
The Hardware Evolution Ladder and DEV/LVP/SVP are not NASA TRLs and must not be mapped one-to-one.

---

# Source hierarchy decision

For Wave 01 claims, use this order:
1. exact NASA handbook section for the engineering premise;
2. current NASA procedural document only when a NASA-specific requirement is actually relevant;
3. official ISO record for standard identity/current-status/scope;
4. licensed standard text only if exact ISO normative wording is needed;
5. internal V6 synthesis for listener tools and DEV/LVP/SVP implementation.

No secondary blog/source is needed to support the locked core.
