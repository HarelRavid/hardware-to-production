# A8 Research Pack — Configuration Management from Prototype #1

status: CLAIM SET STABLE
season: Season 1 — Build the Right Thing
primary_audience: Audience A — founders / early hardware development teams
secondary_audience: systems, mechanical, electronics, embedded, test, NPI, quality, suppliers
lifecycle: DEV-FIRST / CROSS-STAGE
entry_point: FOUNDATION FOR TEAMS WITH MULTIPLE PROTOTYPE BUILDS
technical_depth: foundation-practitioner

## 1. Episode promise
Teach early hardware teams how to preserve product identity and change history from the first repeated prototype without imposing enterprise PLM bureaucracy.

Canonical listener question:
> If a prototype passes or fails today, can we reconstruct exactly what hardware, BOM, firmware, configuration, material and rework state produced that result six weeks from now?

## 2. Navigation card
**You are here:** Repeated prototype builds → controlled evidence → industrialization.

**Best for:** teams moving beyond one-off bench articles into multiple units, revisions, suppliers or shared testing.

**You should already know:** no mandatory prerequisite; A1/A7 help explain requirement/evidence linkage.

**You will leave with:** Minimum Prototype Configuration Record + Change Impact Check.

**Prototype shortcut:** lightweight spreadsheets, Git, drawing revision folders and simple serial labels are acceptable in DEV.

**Shortcut expires when:** multiple units/revisions/suppliers/tests coexist and the team can no longer reliably reconstruct what was built, tested, changed or released.

**Next:** Episode 1 industrialization transition → later configuration/change-control deep dives.

## 3. Audience contract
### DEV takeaway
Give every meaningful build an identity and link it to the definitions and evidence that matter.

### Prototype shortcut
Use lightweight tools; the discipline matters before the software platform.

### Shortcut expiration
When ambiguity in HW/FW/BOM/material/rework state can change an engineering conclusion, configuration identity must be controlled.

### LVP change
Released BOM/drawings/specs, effectivity, deviations/rework, supplier lots, programming/calibration and as-built genealogy become increasingly necessary.

### SVP evidence
Serial production requires controlled definition, execution/as-built truth, change authority/effectivity and traceable evidence across the released population.

### Manufacturing-debt prevention
Do not allow successful prototype behavior to become detached from the exact configuration that generated it.

### Listener action
Assign identities to the last five prototype units/builds and attempt to reconstruct each one completely.

## 4. Stable conceptual chain
Definition
→ revision/version
→ build/unit identity
→ as-built/as-programmed configuration
→ test/evidence
→ deviation/rework
→ change decision
→ effectivity
→ new configuration
→ re-verification where affected

## 5. Stable core claim set
A8-C01 — Evidence should remain linked to the exact product/configuration that generated it.

A8-C02 — Definition, as-built/as-run state and evidence are distinct objects that should remain traceably linked.

A8-C03 — Lightweight configuration control can begin in DEV without enterprise PLM/MES tooling.

A8-C04 — Rework/deviation should add history rather than overwrite the failed/original state.

A8-C05 — A change should trigger impact/re-verification only where it affects relevant claims/evidence dependencies.

A8-C06 — Hardware, firmware/software, calibration/configuration and test procedure identity can interact and must be considered together when they contribute to the claim.

A8-C07 — Multiple suppliers/lots/alternates increase the importance of as-built identity because nominal part equivalence may not prove equal evidence.

A8-C08 — Configuration control becomes a production enabler when it allows defects, changes and field signals to be segmented by actual population.

## 6. Claim classes / source status
- C01/C02/C04/C05/C06/C08: V6 + frozen backbone/global invariants.
- C03: V6 synthesis; lightweight implementation rule.
- C07: V6 + P2.06 supplier/change principles.
- Open P0 normative claims in conceptual core: 0.
- Any exact ISO 10007, NASA or industry-specific configuration requirement becomes P0 when used as normative language.

## 7. Listener tool — Minimum Prototype Configuration Record
For each prototype/build/unit capture:
| Field | Minimum record |
|---|---|
| Unit/build ID | unique identifier |
| Date/build | when built |
| Mechanical revision | drawing/CAD/released definition reference |
| PCB/HW revision | board revision |
| BOM revision | component list/approved alternates |
| Firmware/software | version/commit/build |
| Configuration/calibration | relevant settings/data version |
| Critical material/supplier | where claim-dependent |
| Test procedure | version/method |
| Result/evidence link | where raw/result data live |
| Deviations/rework | original failure + action + final state |
| Owner | person responsible for record |

## 8. Change Impact Check
When something changes ask:
1. What exactly changed?
2. Which units/builds receive the change?
3. Which requirements/interfaces/CTQs depend on it?
4. Which existing evidence depended on the previous state?
5. Which supplier/process/test/tooling assumptions change?
6. Is targeted re-verification enough or is broader evidence invalidated?
7. How will effectivity be recorded?
8. Can old/new populations be reconstructed later?

## 9. Sentinel Node worked example
Unit SN-DEV-07:
- enclosure Rev B;
- PCB Rev A2;
- BOM Rev A2.3;
- firmware commit/build F-017;
- calibration table C-04;
- connector supplier lot L-118;
- environmental test procedure TP-ENV-03;
- connector seating rework performed after initial fail.

If the unit later passes environmental testing, the evidence must preserve both the original fail/rework history and the final configuration. A later connector supplier change should trigger an impact decision against only the claims/evidence that depend on connector behavior rather than automatically invalidating every test ever run.

## 10. Common failure modes
- filenames like FINAL_v7_really_final;
- test report has no reconstructable HW/FW version;
- engineer changes firmware between tests without recording it;
- BOM alternate silently substituted;
- reworked unit appears only as PASS;
- supplier lot/change cannot be linked to affected units;
- every change causes total re-test because evidence dependencies are unknown;
- no effectivity date/serial boundary for change.

## 11. Standards/source targets
Priority authoritative source families:
- NASA / government configuration-management guidance;
- ISO 10007 or other CM guidance where exact terminology is useful and applicable;
- industry-specific configuration/change requirements only when a later episode requires them.

Guardrail:
Do not imply a startup must implement a formal aerospace-grade CM system from prototype #1. The episode teaches minimum product truth and reconstructability.

## 12. Applicability statement
General hardware configuration/evidence discipline. Regulated, aerospace, medical, automotive, defense and contractual programs may impose formal CM, release, traceability, approval and record-retention requirements beyond this lightweight DEV model.

## 13. What this episode must NOT claim
- enterprise PLM is required in DEV;
- every minor edit needs a formal ECO immediately;
- configuration control means freezing design early;
- all changes invalidate all prior evidence;
- a final PASS erases prior failure/rework;
- version control alone proves full product genealogy.

## 14. Claim-set-stable result
PASS.
- Eight distinct claims retained.
- A8 remains the lightweight DEV configuration foundation; deep change-control mechanics stay in P2.02/later episodes.
- No enterprise tooling requirement was introduced.
- Global invariants on definition/execution/evidence, rework history and evidence-dependent change remain intact.
- Standards-specific CM claims remain behind the Source Verification gate.

Next maturity target: EVIDENCE VERIFIED after authoritative configuration-management support and any selected standards-specific claims are verified.
