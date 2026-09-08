# Season 6 — Case Evidence Shortlist V1

status: ACTIVE — CANDIDATE SHORTLIST, NOT YET EPISODE-LOCKED
season: Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies
scope: EP53–EP59 candidate evidence + EP60 synthesis handoff
opened: 2026-09-08
method: primary/official-source-first

## 1. Purpose

Build a defensible case layer before producing Season 6 episode blueprints.

Season 6 is not a new foundations pass. Cases must apply the frozen Hardware-to-Production frameworks and preserve:

`FACT → SOURCE INTERPRETATION → OUR FRAMEWORK LESSON`

A compelling story is not sufficient. A candidate is promoted only when the source record supports the factual mechanism, timing, consequence and relevant applicability boundary.

## 2. Evidence classes used in this shortlist

- **A — Regulator / government investigation / official legal record.** Preferred for failure facts and causal statements.
- **B — Company primary technical / regulatory filing / official postmortem.** Strong for what the company itself documented; company interpretation must remain attributed.
- **C — Official industry body / standard owner.** Strong for method/applicability context, not proof that a specific company executed well.
- **D — Government-backed case study with company-reported outcomes.** Useful for operational examples; quantitative success claims remain case-reported rather than independent audit findings.

Promotion status:
- **PROMOTE** — strong candidate for a case evidence packet.
- **SUPPORT** — useful context or method source, not a standalone case.
- **HOLD** — potentially useful but needs stronger corroboration or clearer episode ownership.

---

# EP53 — Hardware Launch Failures and What Was Missed

Target: different failure classes, not multiple versions of one recall story.

## EP53-CAND-01 — Samsung Galaxy Note7: initial recall did not close the hazard
**Status:** PROMOTE
**Evidence class:** A + B
**Primary failure class:** product/supplier evidence + corrective-action effectiveness / containment

### Documented facts to use
- CPSC recalled about 1 million Galaxy Note7 phones on 15 September 2016 because lithium-ion batteries could overheat and catch fire.
- On 13 October 2016 CPSC expanded the recall to about 1.9 million units, explicitly including replacement Note7 devices from the first recall.
- Samsung later announced that its investigation and three independent organizations concluded that batteries were the cause and introduced enhanced battery quality/safety checks.

### Sources
- CPSC initial recall: https://www.cpsc.gov/Recalls/2016/Samsung-Recalls-Galaxy-Note7-Smartphones
- CPSC expanded recall: https://www.cpsc.gov/Recalls/2017/Samsung-Expands-Recall-of-Galaxy-Note7-Smartphones-Based-on-Additional-Incidents-with-Replacement-Phones
- Samsung investigation announcement: https://news.samsung.com/global/samsung-electronics-announces-cause-of-galaxy-note7-incidents-in-press-conference
- Samsung enhanced QA measures: https://news.samsung.com/global/samsung-announces-new-and-enhanced-quality-assurance-measures-to-improve-product-safety

### Canonical lesson candidates
- A remedy/replacement population needs its own evidence; it is not trustworthy merely because it is the corrective action.
- Containment and corrective-action effectiveness are separate gates.
- Supplier/component evidence must be connected to product-level risk and configuration identity.

### Guardrail
Do not infer a single root organizational cause beyond the published investigation. Keep Samsung technical conclusions attributed to Samsung/independent investigators and CPSC facts separate.

## EP53-CAND-02 — Tesla Model 3 ramp: automation introduced faster than some processes could mature
**Status:** PROMOTE
**Evidence class:** B — SEC filing
**Primary failure class:** automation / ramp / moving constraint

### Documented facts to use
Tesla's Q1 2018 Form 10-Q states that it added automation too quickly in certain Model 3 manufacturing processes, encountered ramp challenges in the battery-module line, materials flow and general assembly, temporarily reduced automation and introduced semi-automated/manual processes, and treated the battery-module line as the main production bottleneck for months.

### Source
- Tesla Form 10-Q, quarter ended 31 March 2018: https://www.sec.gov/Archives/edgar/data/1318605/000156459018011086/tsla-10q_20180331.htm

### Canonical lesson candidates
- Automation maturity is bounded by process maturity and failure/recovery capability.
- A manual/semi-automatic bridge can be a controlled production mode, not necessarily a regression.
- Constraints move as bottlenecks are relieved; one machine's peak speed is not system capacity.

### Guardrail
Do not frame this as “automation is bad.” Tesla explicitly remained committed to automation and described selective reduction while processes were stabilized.

## EP53-CAND-03 — Boeing 737 MAX JATR: invalid assumptions can survive formal development/certification
**Status:** PROMOTE
**Evidence class:** A
**Primary failure class:** architecture / system integration / assumption validation

### Documented facts to use
The FAA-chartered Joint Authorities Technical Review identified issues in the 737 MAX certification process and recommended questioning applicant assumptions, documenting compliance, and strengthening human-factors/system-integration treatment. The JATR specifically found that some assumptions about NG-to-MAX pilot experience and flightcrew response did not appear warranted.

### Sources
- FAA JATR landing page: https://www.faa.gov/newsroom/finaljatrsubmittaltofaaoct2019
- JATR report: https://www.faa.gov/sites/faa.gov/files/2022-08/Final_JATR_Submittal_to_FAA_Oct_2019.pdf

### Canonical lesson candidates
- Assumptions are part of the engineering definition and require evidence, especially across changed-product interfaces.
- Interface and human-system behavior cannot be hidden inside subsystem success.
- Formal review processes do not remove the need to challenge inherited assumptions.

### Guardrail
This is an aviation certification case, not a generic manufacturing rule. Use it to teach assumption/evidence discipline and system integration, not to universalize aviation regulatory mechanisms.

## EP53-CAND-04 — Peloton Tread+: field signal and hazard escalation
**Status:** PROMOTE / secondary case
**Evidence class:** A
**Primary failure class:** field evidence / hazard recognition / reporting

### Documented facts to use
CPSC's May 2021 recall documented one child death and 72 reports of people, pets or objects being pulled under the rear of the Tread+, including 29 reports of child injuries. A later CPSC settlement record states that Peloton had more than 150 reports by 4 March 2021 and addresses failure to immediately report the defect/risk as required by the Consumer Product Safety Act.

### Sources
- CPSC recall: https://www.cpsc.gov/Recalls/2021/Peloton-Recalls-Tread-Plus-Treadmills-After-One-Child-Died-and-More-than-70-Incidents-Reported
- CPSC settlement/order: https://www.cpsc.gov/s3fs-public/PelotonInteractiveIncProvSettlementAgreementandOrder23C0001p.pdf

### Canonical lesson candidates
- FIELD EVENT → SIGNAL AGGREGATION → containment/decision timing.
- Individual complaints become engineering evidence when aggregated and scoped to a population/configuration.

### Guardrail
Keep legal/reporting conclusions tied to the CPSC record and U.S. consumer-product context.

---

# EP54 — Successful Industrialization Patterns

Target: documented pattern + boundary of transfer. Avoid survivorship-bias storytelling.

## EP54-CAND-01 — GE LEAP fuel nozzle: redesign for process + qualification + serial additive production
**Status:** PROMOTE
**Evidence class:** B
**Pattern:** design simplification / process-specific redesign / cross-functional industrialization

### Documented facts to use
GE documents the LEAP additive fuel-nozzle journey from a conventionally assembled multi-part component to a single-piece additive design, with fewer joining operations, lower weight and improved durability. GE's additive production material also describes co-location of designers, manufacturing engineers and quality teams and transition to FAA-certified serial production.

### Sources
- GE mass-production plant story: https://www.ge.com/news/reports/worlds-first-plant-to-print-jet-engine-nozzles-in
- GE production journey white paper: https://go.additive.ge.com/rs/706-JIU-273/images/GE%20Additive_Path%20to%20Production_White%20paper_Final.pdf
- GE mass-production lessons: https://www.ge.com/news/reports/devil-details-3d-printed-part-jet-engine-part-now

### Canonical lesson candidates
- A new process can require redesigning the part around the process rather than copying the old geometry.
- Prototype success does not prove repeatable serial additive production.
- Design simplification can remove joining operations and their associated evidence burden, but the new process creates its own qualification/control burden.

### Guardrail
Performance and cost claims are company-reported. Before final script, corroborate FAA/product qualification facts and exact numerical claims where they become episode-critical.

## EP54-CAND-02 — GM + Ventec ventilators: scale through partnership with existing domain owner
**Status:** PROMOTE
**Evidence class:** B + A
**Pattern:** industrialization partnership / capability transfer / regulatory boundary

### Documented facts to use
GM and Ventec reported delivery of the 30,000th V+Pro ventilator to HHS in September 2020, completing the federal order in 154 days. HHS/ASPE's later medical-device supply-chain report explains why automotive manufacturers partnered with existing ventilator makers: equipment, labor, planning and logistics capabilities can transfer, while medical-device licensing/regulatory knowledge does not transfer automatically.

### Sources
- GM/Ventec delivery record: https://investors.gm.com/news-releases/news-release-details/general-motors-and-ventec-life-systems-complete-delivery-30000/
- HHS/ASPE medical-device supply-chain report: https://aspe.hhs.gov/sites/default/files/documents/e48047020834c0c34cf6baf08a9428d0/PR-A328-2-medicaldevices.pdf

### Canonical lesson candidates
- Scale capability and domain approval capability are different assets.
- Industrialization suppliers/partners can transfer production-system expertise without pretending regulatory/product knowledge is interchangeable.
- Rapid ramp still requires a defined technical owner for product requirements and applicable regulatory evidence.

### Guardrail
Pandemic emergency conditions, government contracts and emergency regulatory context limit direct transfer to ordinary product launches.

## EP54-SUPPORT-01 — Toyota Production System as an established pattern source
**Status:** SUPPORT, not a standalone success case
**Evidence class:** B/C

Toyota's official history documents TPS around Just-in-Time and jidoka and describes detecting abnormalities at source rather than knowingly propagating defects.

Sources:
- https://www.toyota-global.com/company/history_of_toyota/75years/data/automotive_business/production/system/change.html
- https://www.toyota-global.com/company/history_of_toyota/75years/text/entering_the_automotive_business/chapter1/section4/item4.html

Use only as pattern/context. Do not treat Toyota's production system as a universal maturity template for startups or low-volume hardware.

---

# EP55 — Startup Constraints: Speed Without Manufacturing Debt

Target: evidence around cash, uncertainty, temporary processes and explicit shortcut expiration.

## EP55-CAND-01 — AIMM: a small-scale process failed when scaled
**Status:** PROMOTE
**Evidence class:** D — NIST MEP case study

### Documented case
AIMM's process worked at small scale but water vapor clogged lines during scale-up; the company sought approximately 50× scale, evaluated alternatives and modified the process/equipment toward a scalable solution.

Source:
- https://www.nist.gov/mep/successstories/2025/overcoming-obstacles-scaling-process

Canonical lesson:
`lab/process proof ≠ scale proof`; process physics and utility/byproduct behavior can change when throughput changes.

## EP55-CAND-02 — Prixel Press: bridge tooling and gradual manufacturing transition
**Status:** PROMOTE
**Evidence class:** D

### Documented case
NIST describes a toy startup using laser cutting, vacuum forming, desktop CNC and 3D printing during development, then working through an incubator to move from one kit at a time toward dozens and explore a contract manufacturer.

Source:
- https://www.nist.gov/mep/successstories/2022/prixel-press-leverages-tvcog-ceg-prototyping-commercialization

Canonical lesson:
Bridge processes are legitimate when their expiration condition is visible and the team is intentionally preparing the next production route.

## EP55-CAND-03 — Bedrock Sandals: supplier loss forced a minimum controlled in-house mode
**Status:** PROMOTE
**Evidence class:** D

### Documented case
After losing a planned manufacturing supplier during COVID-19, Bedrock used an existing repair workshop and reconfigured machines for small-scale in-house production. NIST/MMEC supported layout, ergonomics, scheduling and safe start-up rather than requiring a full-scale factory first.

Source:
- https://www.nist.gov/mep/successstories/2021/getting-right-foot-montana-mmec-helps-sandal-company-facility-design

Canonical lesson:
A degraded/temporary manufacturing mode can be acceptable if its scope, controls and economics are explicit.

## EP55-CAND-04 — Free Form Fibers: R&D scale to manufacturing scale
**Status:** PROMOTE
**Evidence class:** D

NIST documents Free Form Fibers' transition from a long-running R&D operation toward commercialization and the stated need to make the “big step” from R&D scale to manufacturing scale.

Source:
- https://www.nist.gov/mep/successstories/2021/free-form-fibers-moves-commercialization-cegs-guidance

Guardrail for all NIST MEP cases:
MEP success stories are official government-hosted case studies but include client-reported outcomes. Do not present the reported savings/growth numbers as independently audited evidence unless separately corroborated.

---

# EP56 — Lessons from Automotive Manufacturing

## EP56-CAND-01 — Chevrolet Bolt battery: two manufacturing defects + supplier QA response
**Status:** PROMOTE
**Evidence class:** A/B through NHTSA-hosted manufacturer communication

GM documented the root cause as the combination of a torn anode and folded separator in the same battery cell, and stated that LG implemented new manufacturing processes and enhanced QA programs before production resumed.

Source:
- https://static.nhtsa.gov/odi/rcl/2021/RCMN-21V650-0383.pdf

Canonical lesson candidates:
- Supplier process evidence is part of product evidence.
- Rare interacting defects can require interaction claims rather than treating failure modes as independent.
- Restart/release after supplier corrective action requires evidence inside the changed process envelope.

## EP56-CAND-02 — Toyota RAV4 seat brackets: defect population bounded by supplier line/time/equipment condition
**Status:** PROMOTE
**Evidence class:** A

Toyota's 2026 NHTSA recall report states that four U.S. vehicles were potentially involved, with seat brackets welded during a specific production period on a specific supplier line; depending on welding-equipment condition, brackets could have missing and/or cold welds.

Source:
- https://static.nhtsa.gov/odi/rcl/2026/RCLRPT-26V256-6965.pdf

Canonical lesson candidates:
- Genealogy/effectivity can dramatically reduce the affected population when supplier line/time/process identity is preserved.
- Equipment condition is part of the demonstrated process envelope.

## EP56-SUPPORT-01 — Automotive Quality Core Tools
**Status:** SUPPORT
**Evidence class:** C

AIAG identifies APQP, Control Plan, PPAP, FMEA, SPC and MSA as automotive Quality Core Tools and states most automotive manufacturers/suppliers require one or more.

Source:
- https://www.aiag.org/expertise-areas/quality/quality-core-tools

## EP56-SUPPORT-02 — IATF 16949 applicability/current-status control
**Status:** SUPPORT
**Evidence class:** C

As of this shortlist date, IATF's publication register still lists IATF 16949:2016 as the published first edition while a second-edition revision is in development; certification Rules 6th Edition became effective in 2025 and has 2026 sanctioned interpretations.

Sources:
- https://www.iatfglobaloversight.org/iatf-publications/
- https://www.iatfglobaloversight.org/news/30-july-2026-iatf-stakeholder-communique-iatf-16949-2nd-edition-update-information/

### Automotive transfer guardrail
APQP/PPAP/FMEA/SPC/MSA and IATF requirements are automotive/customer-context methods. Extract useful mechanisms, but do not state that every hardware startup or industrial product must implement the automotive system wholesale.

---

# EP57 — Lessons from Medical-Device Manufacturing

## EP57-CAND-01 — Philips Respironics foam recall + rework problems
**Status:** PROMOTE — flagship medical case
**Evidence class:** A

### Documented facts to use
FDA records show the 2021 recall of certain ventilators/CPAP/BiPAP devices because PE-PUR sound-abatement foam could degrade. Later FDA records document new issues in certain reworked Trilogy ventilators: replacement silicone foam could separate and block the airpath, and residual PE-PUR debris was found in some reworked devices. FDA later described a 2024 consent decree restricting certain production/sales until requirements were met and requiring a Recall Remediation Plan and independent testing.

Sources:
- FDA recall overview: https://www.fda.gov/medical-devices/respiratory-devices/recalled-philips-ventilators-bipap-machines-and-cpap-machines
- FDA reworked-device recall: https://www.fda.gov/medical-devices/medical-device-recalls-and-early-alerts/philips-respironics-recalls-certain-reworked-philips-respironics-trilogy-100200-and-garbin
- FDA activity/remediation history: https://www.fda.gov/medical-devices/recalled-philips-ventilators-bipap-machines-and-cpap-machines/fda-activities-related-recalled-philips-ventilators-bipap-machines-and-cpap-machines

Canonical lesson candidates:
- Rework/remediation creates a new as-built state and requires its own effectiveness evidence.
- “Repaired” is not equivalent to “risk removed.”
- Field evidence, genealogy, corrective action and independent verification can become one linked evidence chain.

## EP57-CAND-02 — Smith & Nephew tendon staples: packaging-process seal integrity
**Status:** PROMOTE / compact case
**Evidence class:** A

FDA recall database states that the packaging process could produce an improper or incomplete outer-foil-pouch seal, potentially compromising sterility.

Source:
- https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfRES/resCollection_2.cfm?ID=209677

Canonical lesson:
The validated production definition includes packaging/sterility-barrier processes where they are part of product safety/performance.

## EP57-CAND-03 — Philips Achieva MRI body-coil seal adhesive
**Status:** PROMOTE / compact case
**Evidence class:** A

FDA lists the determined cause as process control for a Quadrature Body Coil seal-adhesive failure that could create loose/sharp edges.

Source:
- https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfres/res.cfm?id=205471

## EP57-SUPPORT-01 — U.S. QMSR current applicability
**Status:** SUPPORT
**Evidence class:** A

FDA states that the Quality Management System Regulation became effective 2 February 2026, incorporates ISO 13485:2016 by reference, and applies to finished-device manufacturers intending commercial distribution in the U.S.

Source:
- https://www.fda.gov/medical-devices/postmarket-requirements-devices/quality-management-system-regulation-qmsr

### Medical transfer guardrail
Regulatory/QMS obligations are jurisdiction-, product- and role-specific. Do not generalize U.S. device requirements to all hardware or all medical-device markets.

---

# EP58 — Lessons from Aerospace Manufacturing

## EP58-CAND-01 — Boeing 787 battery: sub-tier manufacturing features escaped supplier oversight
**Status:** PROMOTE — flagship aerospace supplier case
**Evidence class:** A

NTSB's 787 APU-battery report describes manufacturing-process features at GS Yuasa, including electrode perturbations/FOD, and states that quality controls were not established to detect these features. The report also documents the Boeing → Thales → GS Yuasa oversight chain and notes that audit discrepancies had not addressed the relevant cell-manufacturing features.

Sources:
- NTSB report: https://www.ntsb.gov/investigations/AccidentReports/Reports/AIR1401.pdf

Canonical lesson candidates:
- Approved suppliers and completed audits do not prove every critical process characteristic is controlled.
- Sub-tier process knowledge and surveillance scope matter.
- FAI/audit evidence is bounded by what was actually verified.

## EP58-CAND-02 — Alaska Airlines 737-9 door plug: manufacturing rework history and incomplete closure
**Status:** PROMOTE — flagship rework/configuration case
**Evidence class:** A

NTSB's 2025 findings and recommendations identify incomplete closure of the left mid-exit door plug after it had been opened for rework during manufacturing, with securing bolts/hardware missing, and address training/guidance/oversight of Boeing's removal/rework process.

Source:
- NTSB recommendation letter/report summary: https://www.ntsb.gov/safety/safety-recs/recletters/A-25-015-033.pdf

Canonical lesson candidates:
- Rework adds history; it must not erase the failed/interrupted state.
- Configuration/closure verification must survive shift/personnel/process handoffs.
- A production record is useful only if execution state can be reconstructed.

## EP58-CAND-03 — PW4077 fan blade: manufacturing discontinuity + fatigue life
**Status:** PROMOTE
**Evidence class:** A

NTSB's United Airlines Flight 328 final report describes a discontinuity introduced during machining/manufacturing in a hollow fan blade and a Pratt & Whitney estimate that local stress increased and fatigue life was reduced.

Source:
- NTSB final report: https://data.ntsb.gov/carol-repgen/api/Aviation/ReportMain/GenerateFinalReport/102652/pdf

Canonical lesson:
Manufacturing-created geometry/material-state features can become reliability mechanisms long after release; production evidence and lifecycle inspection strategy must connect.

## EP58-SUPPORT-01 — IAQG 9102 FAI
**Status:** SUPPORT
**Evidence class:** C

IAQG states that 9102 standardizes First Article Inspection requirements for aviation, space and defense product across the supply chain. IAQG SCMH also explicitly notes that 9102 may be contractually/self-imposed and is not required by every other published standard.

Sources:
- https://iaqg.org/standard/9102-first-article-inspection-requirement/
- https://scmh.iaqg.org/scmh-make/

### Aerospace transfer guardrail
Do not generalize FAI, special-process or assurance burdens beyond their contractual/regulatory applicability. Extract the mechanism: configuration-specific verification, process change/re-accomplishment logic and high-consequence evidence discipline.

---

# EP59 — Lessons from Industrial Equipment

This episode should emphasize long life, installed-base configuration, site integration, maintenance, retrofits, spares and obsolescence—not re-teach EP10 product-service design.

## EP59-CAND-01 — Legacy machinery safety: retrofit requirements can be triggered by modification/repair context
**Status:** PROMOTE as regulatory-context case, not a company failure story
**Evidence class:** A

OSHA 29 CFR 1910.147 states that after January 2, 1990, when replacement/major repair/renovation/modification is performed, energy-isolating devices for the machine/equipment must be designed to accept a lockout device. OSHA machine-guarding guidance also notes that older machinery often needs safeguarding retrofits.

Sources:
- OSHA 1910.147: https://www.osha.gov/laws-regs/regulations/standardnumber/1910/1910.147
- OSHA machine-guarding guidance: https://www.osha.gov/etools/poultry-processing/plant-wide-hazards/struck-by-against-caught-in

Canonical lesson:
A fielded machine can have a decades-long lifecycle in which modification changes the applicable control/evidence problem. “It was compliant when new” is not a complete lifecycle strategy.

## EP59-CAND-02 — Siemens legacy automation migration
**Status:** PROMOTE as industrial lifecycle pattern
**Evidence class:** B

Siemens documents structured migration of legacy automation systems from project assessment through planning, implementation and commissioning, with goals including reduced downtime, long-term component availability and continued machine functionality.

Sources:
- https://www.siemens.com/en-us/products/industrial-sustainability-services/factory-automation/
- https://www.siemens.com/en-us/products/industrial-sustainability-services/spare-parts-supply/

Canonical lesson:
Installed-base modernization is a configuration/change project, not merely a component swap. Spare-part availability, commissioning and recovery planning belong in the engineering decision.

## EP59-CAND-03 — ABB robot/electrical lifecycle and retrofit programs
**Status:** PROMOTE as industrial lifecycle pattern
**Evidence class:** B

ABB documents robot/electrical equipment lifecycles that can span decades and offers staged upgrade/retrofit, lifecycle assessment, refurbishment and obsolescence-management approaches.

Sources:
- Robotics upgrades/retrofits: https://www.abb.com/global/en/areas/robotics/services/extensions-upgrades-retrofits
- Electrification lifecycle management: https://www.abb.com/global/en/areas/electrification/services/life-cycle-management

Canonical lesson:
Long-lived industrial assets require configuration-aware spares, modernization and support strategies; product discontinuation does not end the installed-base engineering obligation.

## EP59-SUPPORT-01 — EU Machinery Regulation transition and substantial modification
**Status:** SUPPORT — exact applicability must remain date-qualified
**Evidence class:** A

Current consolidated Regulation (EU) 2023/1230 states that the Regulation generally applies from **20 January 2027** (with specified provisions applying earlier). Therefore, as of 8 September 2026, do not describe the full Regulation as already generally applicable. Use it only as a current transition/future-regime source with exact date qualification.

Source:
- https://eur-lex.europa.eu/eli/reg/2023/1230/en

Before final EP59 scripting, verify which regime applies to the specific machine, market-placement date and modification scenario being discussed.

---

# EP60 — From Prototype to Production: The Full Decision Story

EP60 does not need a new public failure case. It should use the existing Sentinel Node/composite journey as the narrative spine and only use engineering rules already evidence-backed in A0–A9/EP53–59.

Required transitions remain:
`Idea → Requirements → Architecture → POC → Integrated Prototype → Engineering Prototype → Production Intent → LVP → Production Validation → Ramp → SVP`

At each transition expose:
- current configuration;
- claim/evidence/applicability envelope;
- remaining uncertainty;
- acceptable shortcut;
- shortcut expiration trigger;
- production-system decision;
- supplier/process/tool/test impact;
- what changes at DEV vs LVP vs SVP.

Do not create a new final mega-framework.

---

# 3. Cross-case ownership and duplication controls

1. A case may be cross-tagged during research, but final narrative ownership should normally sit in one episode.
2. If a case reappears, later use must apply a different canonical lens without retelling the whole story.
3. EP53 owns failure-pattern comparison; EP56–59 own industry-specific transfer boundaries.
4. Tesla Model 3 belongs primarily to EP53 unless EP54/55 needs a short cross-reference to staged automation/capex.
5. Boeing 787 battery belongs primarily to EP58; EP53 may reference it only as a one-line example of supplier/process evidence escape.
6. Chevrolet Bolt belongs primarily to EP56; do not duplicate the full case in EP53.
7. Philips Respironics belongs primarily to EP57 because the regulatory/remediation evidence chain is the main lesson.

# 4. Next evidence work

Before any Season 6 production blueprint is opened:

1. Create a full evidence packet for each flagship candidate selected for EP53–59.
2. For each packet capture exact dates, product/configuration/population, lifecycle stage, documented mechanism, detection/escape path, consequence, corrective action, effectiveness evidence and transfer limit.
3. Separate regulator finding from manufacturer interpretation.
4. Add clause/page/section locators for PDF reports used in episode-critical claims.
5. Run a causal-language audit: use `caused`, `contributed`, `associated`, `observed`, `reported` only at the strength supported by the source.
6. Select 2–4 final cases per EP53–59, then open the episode production blueprints.

## Current gate

**Season 6 case campaign: OPEN / SHORTLIST V1 COMPLETE**

**Episode production blueprints: NOT YET OPEN**
