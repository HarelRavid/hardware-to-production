# EP58 Case Evidence Pack — Lessons from Aerospace Manufacturing

status: EVIDENCE PACK V1 — CASE SET SELECTED, STANDARDS/APPLICABILITY REVIEW ACTIVE
season: Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies
canonical_episode: EP58 — Lessons from Aerospace Manufacturing
primary_mode: NTSB case analysis + IAQG method context
opened: 2026-09-08

## 1. Episode job

EP58 must answer:

> What can other hardware teams learn from aerospace manufacturing about configuration, supplier oversight, first-article/change evidence, special/critical processes and lifecycle inspection—without copying aerospace assurance burden where it is not justified?

This episode should show why aerospace is evidence-heavy by examining cases where:
- supplier/process approval existed but did not cover the critical mechanism;
- rework history/documentation failed to close an as-built configuration;
- manufacturing-created features later became fatigue/reliability mechanisms.

Required separation:

`NTSB FACT/FINDING → AEROSPACE METHOD CONTEXT → TRANSFERABLE MECHANISM → APPLICABILITY LIMIT`

## 2. Selected case set

1. Boeing 787 APU battery / GS Yuasa — supplier audits/FAI existed, yet relevant manufacturing defects/process features were not adequately controlled/detected.
2. Alaska Airlines 737-9 door plug — rework/removal/closure documentation and quality verification failure.
3. United Airlines Flight 328 PW4077 fan blade — manufacturing-created geometry/contamination + later inspection interpretation/lifecycle evidence.
4. IAQG 9102 FAI — official method context and applicability guardrail.

---

# CASE 58-01 — Boeing 787 battery: approval/audits did not cover the consequential process features

## A. Case identity
- Event: Japan Airlines Boeing 787-8 APU battery fire, Boston, 7 January 2013
- NTSB report: NTSB/AIR-14/01
- Battery manufacturer: GS Yuasa
- System/supplier chain: Boeing → Thales → GS Yuasa
- Lifecycle: supplier industrialization/production → field incident → manufacturing/process investigation
- Primary lens: subtier oversight, process-control scope, inspection capability, FAI/audit evidence envelope

Primary source:
https://www.ntsb.gov/investigations/accidentreports/reports/air1401.pdf

## B. Scope/probable-cause discipline
NTSB's report addresses the incident and explicitly identifies safety issues involving cell manufacturing defects and oversight of cell-manufacturing processes among other certification/thermal-management issues.

Do not reduce the event to “supplier quality caused the fire” or imply one manufacturing issue was the sole probable cause.

## C. Documented fact set

### F58-01-01 — manufacturing concerns despite acceptance/FAI evidence
In the `Cell Manufacturing Concerns` analysis, NTSB states that GS Yuasa said the battery was manufactured according to provided drawing specifications and that GS Yuasa's and Boeing's FAI processes showed compliance with Boeing acceptance/quality-control requirements, **however** NTSB observations identified several manufacturing concerns.

Locator:
NTSB/AIR-14/01, section 2.3, printed page 58.

### F58-01-02 — process could create electrode perturbations
NTSB observed that manual winding flattening could create electrode-foil perturbations/buckling, visually consistent with wrinkles found in examined cells.

Locator:
section 2.3, pages 58–60.

### F58-01-03 — FOD generation near sensitive assembly
NTSB observed welding processes that could generate metallic FOD near open-cell/internal-component assembly and noted weaknesses in FOD shielding/control.

Locator:
section 2.3, printed page 59.

### F58-01-04 — CT inspection could not reliably see relevant features
NTSB found that GS Yuasa CT settings could not identify many internal features; perturbations, small FOD and burrs might not be recognized with the equipment/settings used.

Locator:
section 2.3, printed page 60.

### F58-01-05 — inspection/control gap
NTSB states that GS Yuasa did not have a process to inspect for some features found during the investigation; its FOD monitoring was not a formal standardized quality-control process, and much of the quality-control inspection occurred after cells were fully manufactured.

Locator:
section 2.3, printed pages 60–61.

### F58-01-06 — supplier audit scope missed the relevant features
NTSB states that Thales audited GS Yuasa in June 2011 and September 2012 and discrepancies were addressed, but none related to the perturbations/FOD features later identified. NTSB further states that Thales had not recognized that such features could result from the process or that GS Yuasa's controls were not established to detect them.

Locator:
section 2.3, printed page 61.

### F58-01-07 — Boeing/FAA direct audits before incident
NTSB states that Boeing and FAA personnel did not conduct audits of GS Yuasa before the incident; Boeing said it relied on Thales to audit its subtier suppliers.

Same locator.

## D. Source-supported interpretation
This case is a strong example of **approval evidence being narrower than the consequential process mechanism**. FAI, supplier-quality systems and audits existed, but the later investigation identified manufacturing features that the control/inspection/audit system had not been designed to recognize adequately.

## E. Framework lesson
- Supplier approval is an evidence envelope, not proof that every latent process mechanism is controlled.
- Audit completion is not equivalent to process understanding.
- FAI verifies defined characteristics/configuration; it cannot substitute for process-risk knowledge or capable ongoing controls.
- Inspection resolution/capability must match the defect/mechanism being claimed as controlled.
- Subtier oversight requires clear ownership of what evidence must flow through the chain.
- A low reject rate is weak reassurance if the inspection system cannot detect the consequential feature.

## F. Aerospace-method connection
Potential lenses:
- 9102 FAI: configuration-specific first-article verification;
- supplier-quality/flowdown;
- FOD prevention/control;
- special/key-characteristic process control where applicable;
- change/requalification when process/equipment/inspection capability changes.

Do not claim the incident proves noncompliance with a specific IAQG clause unless independently established.

## G. What EP58 must NOT claim
- FAI is ineffective in general;
- GS Yuasa had no quality system or audits;
- Boeing/FAA/Thales had no supplier oversight at all;
- any one manufacturing feature alone was the sole cause of the incident;
- aerospace supplier-control architecture should be copied unchanged into every hardware startup.

## H. Case readiness
NTSB evidence: EXCELLENT
Supplier-evidence lesson: EXCELLENT
Complexity: HIGH but manageable
Episode use: FLAGSHIP

---

# CASE 58-02 — Alaska Airlines 737-9 door plug: rework history and closure verification

## A. Case identity
- Event: Alaska Airlines Flight 1282, Boeing 737-9, in-flight separation of left mid-exit door plug, 5 January 2024
- NTSB final investigation/report context: AIR-25-04 and 2025 recommendation letters/press materials
- Lifecycle: aircraft manufacturing/rework → delivery → early field event
- Primary lens: rework/removal record, work instruction, training/ownership, quality closure

Sources:
- NTSB safety recommendation letter: https://www.ntsb.gov/safety/safety-recs/recletters/A-25-015-033.pdf
- NTSB press summary: https://www.ntsb.gov/news/press-releases/Pages/NR20250624.aspx

## B. Documented fact set

### F58-02-01 — incomplete closure after rework
NTSB identified incomplete closure of the airplane's left MED plug, with missing securing bolts/hardware, after the plug had been opened to facilitate rework during manufacturing.

Locator:
NTSB A-25-015 through -033 letter, page 5.

### F58-02-02 — plug was opened without required removal documentation
NTSB's 2025 press summary states that the door plug was opened in Boeing's Renton factory to perform rivet repair work and that the work lacked the required documentation/removal record.

Source:
https://www.ntsb.gov/news/press-releases/Pages/NR20250624.aspx

### F58-02-03 — missing documentation prevented quality inspection of closure
NTSB's press summary states that the absence of proper documentation meant no quality-assurance inspection of the plug closure occurred.

Same source.

### F58-02-04 — training/instruction/oversight issues
NTSB's recommendation material identifies safety issues involving clarity/ease of use of the part-removal instruction, undocumented/unstructured OJT, and management oversight/training for door-team personnel.

Locator:
A-25-015 through -033, pages 5 onward.

## C. Source-supported interpretation
The powerful manufacturing lesson is not merely “someone forgot bolts.” The event shows how **rework/removal is a configuration-state transition**: opening an assembly creates a new incomplete state that must be recorded, owned, verified and explicitly closed before release.

## D. Framework lesson
- Rework adds history; it cannot be handled as if the original successful assembly still exists.
- An open/incomplete configuration needs explicit status and closure criteria.
- Work documentation can be a control trigger: if the removal record does not exist, required downstream verification may never be invoked.
- Quality inspection is only useful if process routing/configuration history tells it **what changed and what must be reverified**.
- Training, work instruction and system design must work together; none alone is enough when a high-consequence incomplete state can escape.

## E. What EP58 must NOT claim
- the entire Boeing quality system can be inferred from this single event;
- operator error alone caused the event;
- every rework requires a full first-article inspection;
- NTSB findings directly define manufacturing requirements for non-aviation hardware.

## F. Case readiness
NTSB evidence: EXCELLENT
Rework/configuration lesson: EXCELLENT
Episode use: FLAGSHIP SECOND CASE

---

# CASE 58-03 — PW4077 fan blade: manufacturing feature → fatigue life → inspection interpretation

## A. Case identity
- Event: United Airlines Flight 328, Boeing 777-222, right-engine fan-blade separation, 20 February 2021
- Engine: Pratt & Whitney PW4077
- Primary source: NTSB Powerplant Group Factual Report DCA21FA085 + NTSB investigation page
- Lifecycle: original manufacturing → years in service/overhaul → repeated inspection → fracture
- Primary lens: manufacturing-state impact on reliability + lifecycle inspection/evidence

Sources:
- Investigation page: https://www.ntsb.gov/investigations/Pages/DCA21FA085.aspx
- Powerplant factual report: https://data.ntsb.gov/Docket/Document/docBLOB?FileExtension=pdf&FileName=DCA21FA085+PP+factual-Rel.pdf&ID=15168653

## B. Documented fact set

### F58-03-01 — incident/probable cause high-level
NTSB's investigation page states that it determined the probable cause to be fatigue failure of the right-engine fan blade.

### F58-03-02 — manufacturing-related factors reducing material life
The NTSB Powerplant Group factual report states that examination identified two significant contributing factors decreasing blade-material life in the relevant region:
1. a local geometric discontinuity;
2. carbon contamination of the internal cavity surface likely from contaminated argon used during manufacturing.

Locator:
Powerplant Factual Report, pages 4 and 24–26.

### F58-03-03 — geometric discontinuity mechanism
The factual report states that the local tight radius was caused by machining and exacerbated by forming operations. A P&W technical review estimated a local steady stress increase and reduced fatigue-life resistance at the location.

Locator:
page 24.

Attribution rule:
The exact 30% stress / 50% fatigue-resistance numerical estimate is a **P&W technical-review estimate reported by NTSB**, not an NTSB universal material law.

### F58-03-04 — contamination source timing
The report states that metallurgical analysis indicated carbon contamination introduced after diffusion bonding in manufacturing and that review identified the shop argon system as the most likely source for the event blade's manufacturing-era process.

Locator:
pages 24–26.

### F58-03-05 — earlier inspection indication was accepted
The report states that an indication visible in the April 2016 TAI data was identified as `grit/noise` and accepted; later review found it close to the initiating fatigue-fracture location.

Locator:
section 2.1.9, pages 21–22.

### F58-03-06 — procedure called for escalation/reinspection
The report states that the 2016 inspection procedure required either strip/repaint for a second TAI or elevation of the ambiguous indication for team review/other inspections, but no documentary evidence was found that either occurred.

Same locator.

## C. Source-supported interpretation
This case connects **manufacturing evidence to lifecycle reliability**. The blade's as-manufactured internal geometry/material surface state was not merely a production-quality detail; it altered fatigue resistance over years of service. Later inspection interpretation then became another evidence layer.

## D. Framework lesson
- Manufacturing-created material/geometry state can be a reliability mechanism long after production release.
- Production acceptance and field/lifecycle inspection are linked evidence systems.
- “Passed inspection” is meaningful only relative to inspection method capability, criteria and correct handling of ambiguous indications.
- Historical process changes can matter to installed populations; manufacturing date/process genealogy can drive lifecycle risk stratification.
- Reliability models should connect known process failure mechanisms to screening/inspection/maintenance controls where justified.

## E. What EP58 must NOT claim
- manufacturing discontinuity alone was the full probable cause without the final report context;
- the numerical stress/life estimate applies generally;
- all legacy blades manufactured before a process change had the same defect state;
- one inspection technology is inherently inadequate.

## F. Case readiness
Manufacturing/reliability connection: EXCELLENT
Source type: NTSB factual report + investigation page
Numerical attribution burden: CONTROLLED
Episode use: THIRD CASE / lifecycle bridge

---

# SUPPORT 58-04 — IAQG 9102 First Article Inspection

## A. Official scope
IAQG states that 9102 standardizes First Article Inspection process/documentation requirements for verification of aviation, space and defense product and can be used across supply-chain levels.

Source:
https://iaqg.org/standard/9102-first-article-inspection-requirement/

## B. Critical applicability guardrail
IAQG SCMH explicitly states that 9102 may be self-imposed or required by contract and **is not required by any other published standard**.

Source:
https://scmh.iaqg.org/scmh-make/

Therefore EP58 must not say “AS9100 means you must do 9102 FAI” as a universal rule.

## C. Transferable mechanism
FAI is useful as a standardized way to verify that the first production/configuration article matches defined engineering/product requirements after relevant new/change conditions.

It does not by itself prove ongoing process capability, lifetime reliability, or control of mechanisms not represented by the verification characteristics.

---

# 3. Cross-case matrix

| Lesson | 787 battery | 737-9 plug | PW4077 blade | Aerospace evidence object |
|---|---|---|---|---|
| approval is bounded | FAI/audits existed, mechanism escaped | release/QA route not triggered correctly | prior service/inspection acceptance existed | evidence envelope |
| supplier/process knowledge | subtier process critical | internal manufacturing/rework | manufacturing-era process state | flowdown/process control |
| rework/change history | secondary | central | overhaul/inspection history | configuration/effectivity |
| measurement/inspection adequacy | CT resolution/control gap | required closure inspection absent | ambiguous TAI handling | verification capability |
| manufacturing ↔ reliability | battery internal shorts | early structural escape | long-term fatigue mechanism | reliability-control bridge |

## 4. Episode-level synthesis claim candidates

### EP58-C01
Aerospace evidence disciplines are valuable because they force configuration-specific proof, but an approved first article/audit/certificate cannot prove a mechanism that the verification system was never designed to observe.

Status: STRONG INTERNAL SYNTHESIS, 787 case.

### EP58-C02
Rework should be treated as an explicit configuration-state transition with history, ownership, closure and re-verification—not as a temporary interruption that disappears after the part is put back.

Status: CANONICAL BACKBONE + 737-9 case.

### EP58-C03
Manufacturing process state can become a field reliability variable years later, so production genealogy and lifecycle inspection strategy should connect where failure physics justify it.

Status: STRONG, PW4077 case.

### EP58-C04
Transfer aerospace methods by the **risk/evidence mechanism**, not by copying aerospace paperwork/certification burden into unrelated products.

Status: REQUIRED GUARDRAIL.

## 5. Recommended narrative order

1. **787 battery:** “The battery had passed acceptance/FAI—but the later investigation found process features the controls were not built to catch.”
2. Distinguish conformance evidence from process-understanding/capability evidence.
3. **737-9 door plug:** rework is a configuration state; missing record → missing verification chain.
4. Introduce 9102 FAI as a real aerospace tool, with the explicit IAQG applicability caveat.
5. **PW4077:** decades-long consequence of as-manufactured internal state + inspection interpretation.
6. Close with three transferable aerospace habits: configuration identity, evidence-to-risk matching, and disciplined change/rework closure.

## 6. Listener tool — Aerospace Practice Transfer Check

`Aerospace method → exact scope/contract? → failure consequence it controls → configuration/change trigger → evidence produced → ongoing capability covered? → supplier/subtier dependence → cost/assurance burden → what high-risk hardware elsewhere should borrow → what low-risk/LVP hardware can simplify`

Internal synthesis only.

## 7. Remaining evidence gaps before episode lock

1. Use the final NTSB Flight 328 report, not only the factual report, for any final causal sentence beyond manufacturing-factor facts.
2. If using exact FAI reaccomplishment/change triggers, source current 9102 Rev C or contractual guidance rather than memory.
3. Avoid implying 9102 is mandated by 9100; IAQG SCMH explicitly warns against this simplification.
4. Keep PW4077 numerical stress/life estimates attributed to P&W technical analysis reported in the factual record.
5. Technical review should verify terms `special process`, `key characteristic`, `FAI` and `flowdown` wherever used normatively.

## 8. Gate

Flagship NTSB evidence: EXCELLENT
Supplier/configuration/reliability coverage: STRONG
Aerospace applicability burden: HIGH / controlled
Cross-industry transfer rule: DEFINED

Current status:

**EP58 CASE EVIDENCE PACK V1: COMPLETE — FINAL-REPORT/STANDARD-TRIGGER CHECK REQUIRED AT SCRIPT GATE**
