# EP59 Case Evidence Pack — Lessons from Industrial Equipment

status: EVIDENCE PACK V1 — CASE SET SELECTED, LIFECYCLE/APPLICABILITY REVIEW ACTIVE
season: Season 6 — Manufacturing Atlas: Decision Playbooks and Case Studies
canonical_episode: EP59 — Lessons from Industrial Equipment
primary_mode: installed-base / retrofit / obsolescence case analysis
opened: 2026-09-08

## 1. Episode job

EP59 must answer:

> What changes when hardware is expected to operate for years or decades at customer sites while controls, software, safety expectations, spare parts and component generations continue to change around it?

EP10 already owns **designing for reliability, service and repair before production**.

EP59 owns a different problem:
- the fielded installed base already exists;
- multiple configurations/generations coexist;
- parts/controllers/software become obsolete;
- upgrades/retrofits alter interfaces and safety assumptions;
- site commissioning and recovery are part of the change;
- service records and as-built identity become manufacturing/lifecycle evidence.

The episode must therefore treat retrofit as an engineering/configuration transition, not merely as replacing an old component with a newer one.

Required separation:

`INSTALLED-BASE FACT → CHANGE/RETROFIT EVIDENCE NEED → CURRENT APPLICABILITY → TRANSFERABLE LIFECYCLE LESSON`

## 2. Selected case set

1. Coca-Cola Beverages South Africa Phoenix bottling plant — modernization of an installed automation/control system driven by obsolescence, diagnostics/backup and network/control migration needs.
2. Safilin spinning-machine retrofit — a retrofit that crossed mechanical, drive, control, HMI and safety boundaries rather than being a controller-only swap.
3. OSHA lockout/tagout modification rule — current U.S. workplace-safety support showing that major repair/renovation/modification can change energy-isolation design obligations.
4. ABB lifecycle/retrofit material — supporting evidence that industrial assets commonly outlive individual automation/product generations and therefore require lifecycle/obsolescence planning.
5. EU Machinery Regulation Article 18 — future/current-transition support only; exact date qualification required because general application begins 20 January 2027.

---

# CASE 59-01 — CCBSA Phoenix bottling plant: installed-base automation modernization

## A. Case identity
- Site: Coca-Cola Beverages South Africa (CCBSA), Phoenix bottling plant
- Asset context: existing bottling/packaging production equipment and automation
- Lifecycle: installed production line → legacy/obsolescence pressure → controls/network/HMI modernization
- Primary lens: obsolescence, installed configuration, migration, diagnostics/backup, recommissioning
- Evidence source: Siemens customer reference / primary vendor case material

Source:
https://www.siemens.com/global/en/products/services/digital-enterprise-services/consulting-services/modernization-services/cc-bsa-phoenix.html

If this URL redirects or regionalizes at publication time, retrieve the current Siemens CCBSA Phoenix modernization case page and preserve an archived/source locator in the final source pack.

## B. Source-status rule
This is a Siemens customer/vendor case study. It is strong for the **documented project objectives, architecture changes and migration scope** described by Siemens, but performance/benefit claims remain company/vendor-reported unless independently corroborated.

## C. Documented fact set

### F59-01-01 — obsolescence/failure risk was part of the modernization need
The Siemens case describes an installed bottling operation facing legacy-drive/control issues, including obsolete variable-speed-drive equipment whose failures created maintenance/support concerns.

### F59-01-02 — controller-generation migration
The project scope included migration from SIMATIC S7-300 PLC technology toward S7-1500 controllers.

### F59-01-03 — network migration
The case includes migration from Profibus-based communication toward Profinet in the upgraded architecture.

### F59-01-04 — HMI/diagnostics/backup considerations
The case identifies obsolete HMI elements and includes requirements around improved diagnostics, system visibility and ability to maintain/restore automation backups.

### F59-01-05 — modernization is not one-component replacement
The documented objectives span drives, PLCs, networking, HMI and engineering/diagnostic capability, demonstrating that a legacy controls change can cross multiple architecture layers.

## D. Source-supported interpretation
The useful industrial-equipment lesson is that **obsolescence accumulates across a system**, not only at a single spare part. A controller upgrade can force interface/network/HMI/engineering-tool changes, and the upgraded line must still be commissioned as one functioning production system.

## E. Framework lesson
- Installed-base configuration must include hardware, firmware/software, network/protocol, parameters/recipes and engineering backups where they affect recoverability.
- Obsolescence is an engineering risk when replacement parts/tools/expertise can no longer preserve the demonstrated production state.
- A retrofit has an evidence envelope: affected interfaces must be identified and reverified rather than assuming drop-in equivalence.
- Backup is not recovery. The organization must know that the correct configuration can be restored and that production/quality state remains trustworthy afterward.
- Modernization should define rollback/transition/commissioning behavior before the old system is removed.

## F. Transfer limit
- Siemens is the vendor in this source; do not treat its recommended architecture as universally optimal.
- Bottling-line automation economics and uptime requirements differ from low-volume or intermittently operated industrial equipment.
- Profinet/S7 migration is one implementation example, not the canonical technology choice.

## G. What EP59 must NOT claim
- all S7-300/Profibus systems must be replaced;
- a newer controller automatically improves production quality;
- vendor modernization automatically proves safety/compliance;
- migration success can be inferred solely from successful power-up.

## H. Case readiness
Installed-base/lifecycle fit: STRONG
Independent outcome evidence: LIMITED / vendor case
Architecture-change teaching value: STRONG
Episode use: FLAGSHIP

---

# CASE 59-02 — Safilin spinning-machine retrofit: one retrofit crosses mechanics, control and safety

## A. Case identity
- Company/site: Safilin industrial spinning equipment modernization
- Lifecycle: existing machine platform → retrofit/modernization
- Primary lens: multi-domain change impact, commissioning, operator interface, safety boundaries
- Evidence source: Siemens customer reference / primary vendor case material

Source:
https://www.siemens.com/global/en/company/stories/industry/safilin-retrofit-spinning-machines.html

If the public URL changes, retain the current Siemens Safilin retrofit reference as the primary source in the final source pack.

## B. Source-status rule
Company/vendor case study: use for documented retrofit scope and architecture changes. Do not convert vendor benefit statements into independent causal findings.

## C. Documented fact set

### F59-02-01 — retrofit program period
Siemens describes the modernization work across a program running approximately from May 2023 through July 2024.

### F59-02-02 — mechanical architecture changed
The retrofit included redesign/rework of machine/cabinet/mechanical elements rather than only replacement of electronic controls.

### F59-02-03 — drive-train changes
The project replaced legacy gear-train/drive elements with servo-based motion/control elements and included changes to bearing assemblies/drive shafts or related mechanical interfaces.

### F59-02-04 — operator interface changed
Machine control functions were migrated toward an HMI-based operator interface, while physical controls remained for defined safety/emergency/reset functions.

### F59-02-05 — utility/safety isolation remained explicit
The retrofit description preserves explicit emergency-stop/reset and utility-isolation considerations rather than treating modernization as a software-only change.

## D. Source-supported interpretation
The case demonstrates that a retrofit often invalidates evidence across **multiple disciplines at once**. A drive/control upgrade can change machine dynamics, mechanical loads, operator interaction, fault behavior, maintenance procedures and safety functions.

## E. Framework lesson
- Retrofit = `CHANGE 9` applied to an installed asset.
- Start with impact mapping, not with the replacement BOM.
- A changed controller/drive may require revalidation of motion behavior, protection, interlocks, tooling/process output and operator/maintenance instructions.
- HMI migration changes human-system interfaces and therefore can affect abnormal/recovery behavior.
- Safety and energy-isolation functions must remain independently verifiable through the change.
- Commissioning should prove both machine function and the production/quality claim that depends on the machine.

## F. Transfer limit
The exact servo/HMI architecture is product/site-specific. The transferable mechanism is cross-domain impact control, not the Siemens implementation.

## G. What EP59 must NOT claim
- retrofit is always cheaper than replacement;
- HMI-based operation is inherently safer/better;
- replacing mechanical transmission with servo control is a universal modernization pattern;
- the vendor case alone proves lifecycle economics.

## H. Case readiness
Multi-domain retrofit lesson: STRONG
Independent outcome evidence: LIMITED / vendor case
Episode use: FLAGSHIP SECOND CASE

---

# SUPPORT 59-03 — OSHA 29 CFR 1910.147: modification can change energy-isolation obligations

## A. Current U.S. regulatory fact
OSHA 29 CFR 1910.147(c)(2)(iii) states, in substance, that after January 2, 1990, whenever replacement or major repair, renovation or modification of a machine/equipment is performed, and whenever new machines/equipment are installed, energy-isolating devices for such machine/equipment must be designed to accept a lockout device.

Primary source:
https://www.osha.gov/laws-regs/regulations/standardnumber/1910/1910.147

Supporting OSHA tutorial/reference:
https://www.osha.gov/etools/lockout-tagout/new-or-modified-equipment

## B. Episode use
This is useful not because EP59 is a lockout/tagout episode, but because it demonstrates a lifecycle principle:

> a modification can change the applicable control obligation for an installed asset.

The machine's historical design state does not automatically govern every future modification scenario.

## C. Applicability guardrail
- This is U.S. occupational-safety law for covered employers/workplaces/equipment within the standard's scope.
- It is not a universal product-design requirement for every machine worldwide.
- OSHA interpretation letters explain enforcement/application but do not create new obligations and can be superseded; anchor the episode in the current regulation text.

## D. Transferable mechanism
Before modifying installed equipment, ask whether the change triggers:
- new safety-control obligations;
- changed hazard analysis;
- changed guarding/isolation/interlock requirements;
- new commissioning/training/procedure evidence.

---

# SUPPORT 59-04 — ABB lifecycle / retrofit / obsolescence context

## A. Purpose
Use ABB material only to support the operational reality that industrial electrical/automation/robotic assets can remain in service across long product generations and therefore vendors maintain lifecycle phases, spare-parts/retrofit/modernization programs and obsolescence-management strategies.

Sources:
- Electrification lifecycle management:
  https://www.abb.com/global/en/areas/electrification/services/life-cycle-management
- Robotics extensions/upgrades/retrofits:
  https://www.abb.com/global/en/areas/robotics/services/extensions-upgrades-retrofits
- Modernization services:
  https://www.abb.com/global/en/areas/process-automation/process-automation-service/modernization-services

## B. Source-status rule
These are vendor lifecycle/service policies, not independent industry standards.

Do not state ABB lifecycle terms/support durations as universal industrial rules.

## C. Transferable mechanism
- installed equipment can outlive availability of original electronics/software/spares;
- lifecycle planning needs explicit obsolescence and replacement/upgrade triggers;
- supportability is part of the long-term engineering/economic envelope.

---

# SUPPORT 59-05 — EU Machinery Regulation 2023/1230: substantial modification, future/current-transition context

## A. Date/applicability fact
Regulation (EU) 2023/1230 generally applies from **20 January 2027**, with specified provisions applying earlier.

As of this evidence-pack date, **8 September 2026**, do not describe the Regulation as already generally applicable.

Primary source:
https://eur-lex.europa.eu/eli/reg/2023/1230/en

## B. Article 18 concept
Article 18 addresses a natural or legal person carrying out a `substantial modification` of machinery/related product and treats that person as the manufacturer for the modified machinery/product under the Regulation, subject to the Article's conditions and obligations.

## C. Episode use
This is a strong future-regime illustration that a sufficiently significant field modification can change legal/manufacturer responsibility—not merely technical configuration.

## D. Guardrails
- At publication time, re-check application date and any transitional provisions.
- Do not apply Article 18 retrospectively to pre-2027 scenarios without legal/applicability analysis.
- Do not generalize EU obligations to other jurisdictions.
- Do not make legal conclusions about whether a specific retrofit is `substantial` without fact-specific analysis.

---

# 3. Installed-base lifecycle model derived from the cases

This is internal synthesis, not an external standard.

## State L1 — Supported original configuration
Original hardware/software/process configuration remains supportable; parts/tools/documentation are available.

Engineering need:
maintain accurate as-built/installed identity and verified backups/settings.

## State L2 — Constrained support / obsolescence emerging
Key parts/software/tools/expertise become difficult to source or maintain.

Engineering need:
identify single points of lifecycle failure, last-buy/spare/repair options and migration lead time.

## State L3 — Planned retrofit / modernization
A defined change replaces one or more subsystems while preserving the required machine/product function.

Engineering need:
change-impact analysis, interface mapping, safety/applicability review, migration plan and recommissioning evidence.

## State L4 — Modified installed configuration
The asset now has a new as-built/as-configured state that may differ across customer sites or serial populations.

Engineering need:
configuration/genealogy update, procedures/spares/software baselines, operator/maintenance training and support ownership.

## State L5 — End-of-support / replacement decision
Continued operation can no longer be justified inside the technical, safety, economic or supportability envelope.

Engineering need:
controlled retirement/replacement/migration—not indefinite exception handling.

The states are descriptive synthesis only; they are not a universal lifecycle standard.

---

# 4. Cross-case matrix

| Lifecycle problem | CCBSA | Safilin | OSHA support | Canonical object |
|---|---|---|---|---|
| electronics/control obsolescence | central | central | not primary | lifecycle/support envelope |
| multi-domain change | controls/network/HMI/drives | mechanics/drives/HMI/safety | safety-isolation trigger | CHANGE 9 / interaction claim |
| configuration identity | legacy vs migrated controls | old vs retrofitted machine | modified machine state | genealogy/effectivity |
| recommissioning/release | modernization/migration | retrofit commissioning | control/procedure implications | release evidence |
| safety applicability after change | contextual | explicit safety functions | very strong U.S. example | applicability/change impact |
| recovery/backups | strong case objective | secondary | procedures/energy control | recovery/configuration integrity |

## 5. Episode-level synthesis claim candidates

### EP59-C01
For long-lived industrial equipment, serviceability is not only a design attribute; it becomes an installed-base configuration-management problem as multiple hardware/software generations and site-specific retrofits coexist.

Status: STRONG INTERNAL SYNTHESIS.

### EP59-C02
Obsolescence becomes a manufacturing/operations risk when loss of parts, tools, software or expertise threatens the ability to restore the demonstrated production state after failure.

Status: STRONG SYNTHESIS, illustrated by CCBSA/ABB lifecycle context.

### EP59-C03
A retrofit should be treated as a controlled engineering change with affected-interface identification, safety/applicability review and recommissioning—not as a maintenance action simply because the machine already exists.

Status: STRONG, Safilin + OSHA support.

### EP59-C04
The evidence required after retrofit should be impact-based: reverify the functions, hazards, process outputs, interfaces and recovery paths actually affected rather than blindly repeating everything or verifying only the new component.

Status: CANONICAL BACKBONE synthesis.

### EP59-C05
Installed-base support strategy should preserve the ability to reconstruct `what is installed where`, including relevant hardware/software/parameters/retrofit history, because the answer determines spares, service procedures, safety and requalification scope.

Status: STRONG INTERNAL SYNTHESIS.

## 6. Boundary with EP10

### EP10 owns
- design-for-service/repair before/around product release;
- access, replaceability, diagnostics and field-learning architecture as design concerns;
- reliability/serviceability design choices.

### EP59 owns
- decades-long installed-base management after products/machines are already deployed;
- obsolescence and coexistence of multiple configurations;
- retrofit/change impact and recommissioning;
- site/customer integration and support ownership;
- changed safety/regulatory obligations triggered by modification;
- lifecycle spares/software/backup/recovery strategy.

Do not re-teach EP10 fundamentals. Use them as prerequisites and move directly to the installed-base problem.

## 7. Recommended narrative order

1. **CCBSA cold open:** the machine still physically works, but parts/control/network/HMI generations around it are becoming the risk.
2. Define obsolescence as loss of ability to reliably restore/support the demonstrated configuration—not merely “old equipment.”
3. **Safilin:** show why retrofit rapidly crosses mechanics, motion control, HMI and safety.
4. Apply `CHANGE 9`: what evidence dependencies did the retrofit actually invalidate?
5. **OSHA modification rule:** an installed machine's legal/safety obligations can change when it is modified; historical acceptance is not the end of applicability analysis.
6. Add ABB lifecycle context: long-lived industrial assets need explicit support/obsolescence triggers.
7. Close with EU future-regime substantial-modification example, explicitly date-qualified.
8. Final lesson: fielded equipment remains an engineering system throughout its lifecycle.

## 8. Listener tool — Installed-Base Change & Retrofit Gate

For each asset/change:

`Asset ID / installed site → current as-built hardware → current software/firmware/parameters → original vs retrofitted subsystems → reason for change → obsolescence/support status → interfaces affected → mechanical/electrical/network/software/safety impacts → regulatory/customer trigger → spare/backward-compatibility plan → migration/rollback plan → backup/recovery proof → commissioning tests → process/product-quality verification → updated as-built record → operator/maintenance procedure/training change → lifecycle owner`

Internal synthesis only.

## 9. Evidence/reporting guardrails

- Siemens/ABB are vendor/company sources. Use them for documented project/lifecycle scope, not independent proof that vendor solutions caused claimed benefits.
- OSHA applicability is U.S.-workplace specific.
- EU Machinery Regulation 2023/1230 is date-sensitive; general application begins 20 January 2027.
- `Retrofit`, `major repair`, `substantial modification` and similar legal/standards terms must not be treated as interchangeable.
- A field modification may change safety/compliance responsibility, but exact legal consequences are jurisdiction/fact specific.
- Do not equate old equipment with unsafe equipment; the issue is whether current condition/configuration/support/evidence remain adequate.

## 10. Remaining evidence gaps before episode lock

1. Preserve stable/archive locators for Siemens customer-reference pages because vendor URLs can move.
2. If any performance/uptime savings from vendor cases are used, independently corroborate or attribute them explicitly.
3. Re-check OSHA 1910.147 text immediately before publication for current wording/applicability.
4. Re-check EU Machinery Regulation application status at publication date; if after 20 January 2027, rewrite the future-regime language accordingly.
5. Regulatory/legal review required for any statement about a specific modification creating manufacturer obligations.
6. Ensure no listener interprets EP59 as a substitute for machine-specific functional-safety/risk assessment.

## 11. Gate

Installed-base/lifecycle coverage: STRONG
Retrofit/change coverage: STRONG
Regulatory support: STRONG WITH JURISDICTION/DATE LIMITS
Vendor-source bias: VISIBLE / CONTROLLED
Boundary with EP10: EXPLICIT

Current status:

**EP59 CASE EVIDENCE PACK V1: COMPLETE — LIFECYCLE/APPLICABILITY CHECK REQUIRED AT SCRIPT GATE**
