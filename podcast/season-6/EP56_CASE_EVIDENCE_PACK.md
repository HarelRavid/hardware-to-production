# EP56 Case Evidence Pack — Lessons from Automotive Manufacturing

status: EVIDENCE PACK V1 — CASE SET SELECTED, APPLICABILITY REVIEW ACTIVE
season: Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies
canonical_episode: EP56 — Lessons from Automotive Manufacturing
primary_mode: industry-practice + regulator/manufacturer case analysis
opened: 2026-09-08

## 1. Episode job

EP56 must answer:

> Which automotive manufacturing disciplines are genuinely useful outside automotive, and which depend on automotive/customer-specific volume, supply-chain and approval context?

This episode must not become an APQP/PPAP vocabulary lecture.

The stronger structure is:
1. show real process/supplier failures;
2. show what evidence objects automotive methods are designed to control;
3. state exact transfer limits.

Required separation:

`CASE FACT → AUTOMOTIVE METHOD CONTEXT → TRANSFERABLE MECHANISM → NON-TRANSFERABLE REQUIREMENT/ECONOMICS`

## 2. Selected case set

1. Chevrolet Bolt EV/EUV battery recall — interacting supplier manufacturing defects + changed manufacturing/QA process.
2. Toyota RAV4 seat-bracket weld recall — narrow genealogy by supplier tier, production line, time window and equipment condition.
3. AIAG Quality Core Tools — official method context, not a case.
4. IATF 16949 current-publication status — applicability/current-revision control, not a case.

---

# CASE 56-01 — Chevrolet Bolt battery: interacting manufacturing defects at supplier

## A. Case identity
- Product: 2017–2022 Chevrolet Bolt EV/EUV battery population addressed by recall communications
- Supplier context: LG battery cell/module production
- Lifecycle: field recall → supplier/process remediation → replacement production
- Primary lens: supplier process evidence, interacting defects, release after process change
- Evidence source: GM communication hosted in NHTSA recall record

## B. Source-status rule
The NHTSA-hosted document is a **GM manufacturer communication**, not an independent NHTSA engineering finding. Root-cause language must therefore remain attributed to GM.

Source:
https://static.nhtsa.gov/odi/rcl/2021/RCMN-21V650-0383.pdf

## C. Documented fact set

### F56-01-01 — two manufacturing defects
GM states that the root cause of the rare circumstances that could cause a battery fire was the simultaneous presence in the same battery cell of two manufacturing defects: a torn anode and folded separator.

Locator:
page 1, `New Battery Production` section.

### F56-01-02 — interaction condition
GM explicitly states that both defects needed to be present in the same battery cell.

Same locator.

### F56-01-03 — changed supplier production process
GM states that LG implemented new manufacturing processes and worked with GM to review/enhance quality-assurance programs before/with resumed production.

Same source/locator.

### F56-01-04 — process-change deployment across facilities
GM states that LG would institute the new processes in other facilities supplying cells to GM.

Same source/locator.

### F56-01-05 — population/time linkage
GM states that replacement prioritization considered specific battery build timeframes where it believed defects appeared clustered.

Same source, `Prioritized Battery Replacement`.

## D. Source-supported interpretation
This is unusually useful because the public communication identifies an **interaction condition**: neither defect is presented as sufficient alone in the cited root-cause statement; the field hazard was associated with their co-occurrence in one cell.

The corrective response also explicitly changed the manufacturing/QA system rather than treating replacement alone as sufficient.

## E. Framework lesson
- Automotive supplier evidence is product evidence when the component's process state creates the product hazard.
- PFMEA/control logic must consider consequential **interactions**, not only independent failure-mode rows.
- Supplier corrective action changes the process evidence envelope and should trigger reassessment/release logic.
- Genealogy by build timeframe can support prioritization/containment when defect occurrence is not uniform.
- FIELD EVIDENCE → SUPPLIER PROCESS INVESTIGATION → PROCESS CHANGE → EFFECTIVENESS/RELEASE evidence.

## F. Automotive-method connection
Possible method lenses:
- PFMEA: process failure modes and interaction awareness;
- Control Plan: controls tied to identified process risks;
- MSA/SPC: trustworthy process/inspection signals where applicable;
- PPAP/re-approval: changed production process evidence if customer-specific requirements trigger it.

Do **not** claim from this case alone which exact Core Tool failed or which PPAP submission level was required/used.

## G. What EP56 must NOT claim
- NHTSA independently determined the exact torn-anode/folded-separator root cause in this document;
- both defects were common across all batteries;
- any one Core Tool would necessarily have prevented the recall;
- every supplier process change universally requires automotive PPAP outside its customer/industry context.

## H. Case readiness
Failure mechanism specificity: STRONG
Source independence: MANUFACTURER-ATTRIBUTED
Interaction-claim value: EXCELLENT
Episode use: FLAGSHIP

---

# CASE 56-02 — Toyota RAV4 seat brackets: genealogy, supplier tiers and shared-equipment propagation

## A. Case identity
- Product: 2025 Toyota RAV4
- Recall: NHTSA 26V256 / Toyota 26TB09 / 26TA09
- Submission date: 22 April 2026
- Potential U.S. population: 4 vehicles
- Supplier component: seat-rail attachment brackets
- Tier: Tier 2 component manufacturer identified as Concord Tool and Manufacturing
- Lifecycle: supplier manufacturing → routine inspection → process investigation → safety assessment/recall
- Primary lens: genealogy/effectivity; equipment condition; supplier-tier investigation

Source:
https://static.nhtsa.gov/odi/rcl/2026/RCLRPT-26V256-6965.pdf

## B. Documented fact set

### F56-02-01 — narrow affected envelope
Toyota's Part 573 report states that the issue affected vehicles manufactured with seat brackets welded during a specific production period on a specific production line at a certain supplier.

Locator:
page 1, `Descriptive Information`.

### F56-02-02 — equipment condition matters
The report states that depending on welding-equipment condition, some brackets could have missing and/or cold welds in different patterns.

Locator:
page 1, `Defect / Noncompliance Description`.

### F56-02-03 — detection upstream of field complaints
The chronology states that during routine inspection at the Tier 1 supplier in late November 2025, missing welds were identified and the Tier 1 notified the Tier 2 and Toyota.

Locator:
page 3 of the PDF / chronology section.

### F56-02-04 — shared-equipment propagation mechanism
Toyota/suppliers found that a shim installed on a passenger-side welding jig caused mechanical interference and damage to a weld robot, causing missing welds. Damage subsequently affected shared tip-dressing equipment used with the driver-side weld robot, producing inadequate tip condition and intermittent missing/cold weld patterns.

Locator:
chronology, page 3.

### F56-02-05 — product-risk analysis followed process investigation
Toyota then analyzed possible missing/cold-weld patterns against crash/restraint conditions and decided on a voluntary safety recall.

Same chronology.

### F56-02-06 — no related U.S. field reports/warranty claims at decision date
Toyota reported that as of 15 April 2026 its record review found no related U.S. Field Technical Reports or warranty claims.

Same chronology.

## C. Source-supported interpretation
This case demonstrates how detailed process genealogy and supplier investigation can bound a potential affected population very narrowly—even when the exact defect presence in individual units is not known before inspection.

It also demonstrates a cross-equipment interaction: damage originating from one jig/robot path propagated through shared tip-dressing equipment into another welding path.

## D. Framework lesson
- Genealogy is not only serial number → supplier; useful genealogy can include supplier tier, line, equipment, tooling, process window and time/effectivity.
- Shared support equipment can create **interaction claims** across nominally separate stations/process paths.
- Equipment/tooling condition belongs to the demonstrated process envelope.
- Detection during supplier inspection can trigger containment before field signals exist.
- A narrow affected population is possible only if enough production identity/history survives.

## E. Automotive-method connection
- Control Plan/reaction plan: routine inspection and response to abnormal weld condition;
- PFMEA: tooling/equipment failure and shared-resource interactions;
- traceability/effectivity: line/time/equipment-based population scoping;
- supplier-quality escalation: Tier 1 → Tier 2 → OEM investigation;
- PPAP/requalification: discuss only if exact customer/process-change requirement is independently sourced.

## F. What EP56 must NOT claim
- all four potentially involved vehicles definitely contain bad welds;
- the report's portal `1%` means Toyota estimated one percent actual defect rate—the report explicitly explains that portal value `1` represented `unknown` in this submission;
- the supplier's routine inspection was necessarily an APQP/Control Plan requirement unless sourced;
- the exact Toyota supplier-quality process is universal.

## G. Case readiness
Regulator-hosted manufacturer report: STRONG
Process mechanism: EXCELLENT
Genealogy lesson: EXCELLENT
Episode use: FLAGSHIP

---

# SUPPORT 56-03 — AIAG Quality Core Tools

## A. Official method context
AIAG identifies the automotive Quality Core Tools as:
- Advanced Product Quality Planning (APQP)
- Control Plan (CP)
- Production Part Approval Process (PPAP)
- Failure Mode and Effects Analysis (FMEA)
- Statistical Process Control (SPC)
- Measurement System Analysis (MSA)

AIAG states that most automotive manufacturers and suppliers require use of one or more Core Tools.

Source:
https://www.aiag.org/expertise-areas/quality/quality-core-tools

AIAG's current page also shows:
- APQP 3rd Edition (2024);
- standalone Control Plan structure;
- AIAG & VDA SPC Manual released July 2026.

## B. Episode use
Teach the chain as connected evidence objects, not paperwork:

`planning/requirements → risk → control → measurement trust → process behavior → production approval`

This maps cleanly to the canonical Hardware-to-Production Quality Chain without claiming the internal framework equals the AIAG manuals.

## C. Transfer guardrail
AIAG itself notes adoption/use beyond automotive, but that does not make automotive customer-specific submission requirements universal.

Extract mechanisms; preserve exact customer/sector applicability.

---

# SUPPORT 56-04 — IATF 16949 current-status control

## A. Current publication status as of 2026-09-08
IATF's official publication register lists `IATF 16949:2016` as 1st Edition, 1 October 2016.

Source:
https://www.iatfglobaloversight.org/iatf-publications/

The IATF published a 30 July 2026 Stakeholder Communiqué specifically updating stakeholders on the status of the revision toward a 2nd Edition.

Source:
https://www.iatfglobaloversight.org/news/30-july-2026-iatf-stakeholder-communique-iatf-16949-2nd-edition-update-information/

## B. Episode rule
Do not describe a draft/upcoming second edition as already replacing the published 2016 edition until official publication/transition information says so.

Do not imply IATF 16949 certification is a universal prerequisite to manufacture automotive-related hardware; applicability depends on supply-chain/customer/certification scope.

---

# 3. Cross-case matrix

| Automotive lesson | Bolt | RAV4 | Core Tool connection | Transferable mechanism |
|---|---|---|---|---|
| supplier process state affects product claim | very strong | very strong | APQP/PFMEA/CP/PPAP context | supplier evidence envelope |
| interacting failure mechanisms | two defects in same cell | shared tip-dresser/equipment propagation | PFMEA/system response | INTERACTION CLAIM |
| traceability/effectivity | build-time clustering | supplier line/time/equipment | APQP/Control Plan/traceability context | affected-population scoping |
| process change → renewed evidence | LG process/QA changes | correction/inspection after investigation | PPAP/reapproval where applicable | evidence invalidation/requalification |
| measurement/inspection before field failure | secondary | routine supplier inspection discovered issue | MSA/CP context | measurement adequacy + reaction |

## 4. Episode-level synthesis claim candidates

### EP56-C01
The most transferable automotive lesson is not “use automotive paperwork”; it is to connect requirement/risk/process control/measurement/approval into one traceable evidence chain.

Status: STRONG INTERNAL SYNTHESIS.

### EP56-C02
Supplier approval is evidence inside a demonstrated process/configuration envelope, not permanent approval of a supplier name.

Status: CANONICAL BACKBONE, strongly illustrated by both cases.

### EP56-C03
Automotive genealogy can be valuable because it supports process-specific population scoping across supplier, line, tooling/equipment and time—not merely VIN traceability.

Status: STRONG, RAV4 case.

### EP56-C04
Core Tools are connected methods whose value comes from the links between risk, control, measurement and production approval; isolated documents can exist without controlling the actual process.

Status: SYNTHESIS + AIAG contextual support.

### EP56-C05
High-volume automotive methods should be transferred by mechanism and risk, not copied wholesale into DEV/LVP hardware with different economics and customer obligations.

Status: REQUIRED TRANSFER GUARDRAIL.

## 5. Recommended narrative order

1. **RAV4 cold open:** four vehicles, but a deep supplier/equipment history tells a much bigger process story.
2. Reconstruct the shim → robot damage → shared tip dresser → second weld path chain.
3. Ask: what information allowed Toyota to scope the population?
4. Introduce Core Tools as the automotive industry's connected risk/control/evidence machinery.
5. **Chevrolet Bolt:** interaction of two manufacturing defects and process/QA changes across supplier plants.
6. Explain supplier approval as an evidence envelope, not a badge.
7. Close with “borrow the mechanism, not the bureaucracy” and a transfer matrix for startup/LVP/SVP contexts.

## 6. Listener tool — Automotive Practice Transfer Matrix

For any automotive method:

`Method → problem it controls → evidence object → customer/standard requirement? → volume assumption → supplier-network assumption → high-consequence assumption → what DEV needs → what LVP needs → what SVP/customer contract requires → transferable core → non-transferable overhead`

Internal synthesis only.

## 7. Remaining evidence gaps before episode lock

1. If exact APQP/PPAP requirements are spoken, source them to the current manuals/customer-specific requirements rather than summaries.
2. Verify whether any selected OEM/customer-specific requirements materially affect the illustrative claims; otherwise keep PPAP discussion generic/contextual.
3. Recheck IATF 2nd Edition status immediately before publication because the revision is active in 2026.
4. Preserve the Bolt root-cause attribution as GM's statement.
5. Use Toyota report wording carefully around potentially involved vs confirmed defective units.

## 8. Gate

Flagship case evidence: STRONG
Industry-method context: STRONG
Applicability burden: HIGH / controlled
Cross-industry transfer discipline: DEFINED

Current status:

**EP56 CASE EVIDENCE PACK V1: COMPLETE — CURRENT-STANDARD/APPLICABILITY CHECK REQUIRED AT SCRIPT GATE**
