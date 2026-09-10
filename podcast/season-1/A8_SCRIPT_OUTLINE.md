# A8 Script Outline — Configuration Management from Prototype #1

status: SCRIPT OUTLINE COMPLETE — FULL SCRIPT DRAFT NEXT
season: Season 1 — Build the Right Hardware Before Production Finds Your Mistakes
primary_audience: founders / early hardware teams / systems / test / NPI / quality
lifecycle: DEV-FIRST / CROSS-STAGE
entry_point: YES
production_blueprint: `A8_PRODUCTION_BLUEPRINT.md`
claim_basis: `A8_RESEARCH_PACK.md`
source_lock: `evidence/source-lock/wave-01/W1_A1_A7_A8_CLAIM_LOCK.md`
shared_sources: `evidence/source-lock/wave-01/W1_SHARED_SOURCE_REGISTER.md`
technical_review: `evidence/source-lock/wave-01/W1_INTERNAL_TECHNICAL_REVIEW.md`
outline_contract: `podcast/SCRIPT_OUTLINE_CONTRACT.md`

## 1. Episode job

Listener enters with:
> We know roughly which prototype/revision we tested.

Listener leaves with:
> I can reconstruct what was intended, what each unit actually contained, what changed/reworked, and which evidence belongs to which configuration — using lightweight tools first and scaling formality only when needed.

Primary listener action:
Attempt the **Five-Build Reconstruction Challenge** and create a Minimum Prototype Configuration Record for the next build.

## 2. Cold open — two identical-looking prototypes

[ILLUSTRATIVE]
Two prototypes look identical. One passes environmental testing and one fails.

Weeks later the team learns:
- one had a different connector lot;
- one had a different firmware build;
- one had a hand rework;
- calibration data differed;
- the test procedure had been updated between runs.

The failure could have become knowledge. Instead, configuration ambiguity makes the comparison weak.

Core point:
[SYNTHESIS — A8-C01/A8-C02]
A result is only reusable when the team can reconstruct the configuration and context that generated it.

Source anchors:
S-W1-03 / S-W1-04.

## 3. Beat 1 — configuration management is product truth, not PLM software

[AUTH-GUIDANCE + SYNTHESIS]
NASA CM guidance identifies configuration planning, identification, change management, status accounting and verification as connected activities.

Podcast translation:
You can begin the discipline with serial labels, controlled drawings/BOM snapshots, Git/version IDs and a simple record. Enterprise tooling is not the starting requirement.

Guard:
Do not say NASA prescribes spreadsheets/Git or that startups must implement NASA CM.

## 4. Beat 2 — three truths that must not collapse

Canonical internal model:
1. **Definition** — what should be built.
2. **As-built / as-programmed / as-run** — what this particular unit/process actually became.
3. **Evidence** — what happened when that state was tested, inspected or used.

[SYNTHESIS informed by S-W1-03/S-W1-04]

Examples of divergence:
- alternate component installed;
- firmware changed after assembly;
- rework wire added;
- calibration table updated;
- supplier material lot changed;
- process/test procedure revised.

Guard:
Do not present the three-object wording as an ISO/NASA formal taxonomy.

## 5. Beat 3 — minimum prototype identity

Listener tool fields:
`Unit/build ID → mechanical rev → PCB/HW rev → BOM rev → FW/software build → calibration/configuration → critical supplier/material/lot → test procedure/result → deviations/rework`.

[SYNTHESIS]

Technical nuance:
Not every product needs every field for every unit.
Capture what matters to claims, safety, reliability, quality, service, investigation and change decisions.

This avoids `trace everything because traceability is good` bureaucracy.

## 6. Beat 4 — rework adds history

Scenario:
A connector is re-seated/reworked after an initial failure and the unit later passes.

Bad record:
`PASS`.

Useful record:
`initial fail → observed condition → rework/action → resulting configuration → retest → final result`.

[SYNTHESIS — A8-C04]
S-W1-03 supports preserving discrepancies/anomalies/corrective actions in verification records.

Guard:
Do not imply every tiny cosmetic touch-up needs enterprise NCR paperwork. Preserve consequential history proportionate to context.

## 7. Beat 5 — revision is not the same question as effectivity

Internal practitioner distinction:
- Revision: which definition/version exists?
- Effectivity: where/when/which serials/lots/orders actually receive it?

[V6 SYNTHESIS — P2-C-CM-002]

Example:
Drawing Rev C released Monday does not prove every Tuesday-built unit is Rev C if old WIP, old supplier lots, delayed shop-floor instructions or firmware pairing remain.

Guard:
Do not attribute our exact terminology distinction to ISO/NASA until separately source-locked.

## 8. Beat 6 — the Change Impact Check

When something changes:
1. what exactly changed?
2. which units/builds receive it?
3. which requirements/interfaces/CTQs depend on it?
4. which prior evidence depended on the previous state?
5. which supplier/process/test/tooling assumptions change?
6. is targeted re-verification enough or is broader evidence invalidated?
7. how is effectivity recorded?
8. can old/new populations be reconstructed later?

[SYNTHESIS informed by S-W1-02/S-W1-03/S-W1-04]

Guard:
Do not attribute this exact eight-question algorithm to NASA/ISO.

## 9. Beat 7 — Sentinel Node alternate sensor cut-in

[ILLUSTRATIVE / CANONICAL SENTINEL]

Trigger:
primary vibration sensor becomes supply constrained.
Purchasing finds a same-package alternate with similar headline specifications.

Bad implementation:
substitute in ERP, build one unit, run a quick functional test, continue production.

Controlled implementation:
map possible impacts:
- sensitivity/frequency response/noise;
- temperature behavior;
- firmware coefficients;
- calibration;
- production-test limits;
- electrical/mechanical fit;
- reliability;
- supplier/process evidence;
- compliance where applicable.

Then decide proportionate evidence, release new definitions if accepted, define cut-in/effectivity and preserve old/new genealogy.

Dependency:
Supplier qualification/reapproval specifics remain P2.06; A8 teaches generic change/configuration logic only.

## 10. Beat 8 — lightweight tools and the point where they stop scaling

DEV:
spreadsheet + serial labels + controlled BOM/drawing snapshots + Git/software identifiers may be enough.

Failure signals that more formal integration is needed:
- multiple builders/suppliers/sites;
- frequent alternates and WIP;
- inability to reconstruct units;
- changes cut in incorrectly;
- test/configuration mismatch;
- field events cannot be segmented;
- too much manual reconciliation.

[SYNTHESIS]

Lesson:
Buy/integrate tooling because information relationships are breaking, not because `mature companies use PLM`.

## 11. Beat 9 — DEV / LVP / SVP

DEV:
know what configuration produced each important engineering result.

LVP:
controlled BOM/drawings/FW/WI, change authority, deviations/rework, supplier lots/effectivity and as-built reconstruction become production infrastructure.

SVP:
configuration/change control scales across suppliers, sites, software, service, field feedback and sustained production.

[SYNTHESIS]

## 12. Misconceptions to challenge

1. `Git/version control is configuration management.`
2. `CM means freezing the design.`
3. `We are too small for revision/build identity.`
4. `Released Rev C means all new units contain Rev C.`
5. `A final PASS erases earlier failure/rework.`
6. `Every change requires complete requalification.`
7. `Same package/spec headline means equivalent evidence.`
8. `PLM solves unclear ownership and bad records automatically.`

## 13. Closing action — Five-Build Reconstruction Challenge

Take the last five meaningful prototypes/units.
Without asking the original builder, reconstruct:
- HW/mechanical revision;
- PCB/BOM;
- firmware/software;
- key material/supplier state;
- calibration/configuration;
- test procedure/results;
- deviations/rework.

Every missing fact that could change an engineering conclusion is configuration debt.

Then create the Minimum Prototype Configuration Record for the next build.

## 14. Season closing handoff

A1–A8 have now built a controlled DEV system:
`requirements → ownership → architecture → representative prototypes → discipline-specific evidence → verification intent → configuration identity`.

Season 1 then continues into EP01–10 and asks the production-intent question:
> The product works. Why still can't we manufacture it repeatedly?

## 15. Source-note skeleton

Spoken anchors:
- S-W1-04 NASA Configuration Management;
- S-W1-03 NASA Product Verification;
- S-W1-02 NASA Requirements Management/change impact.

Standards show-notes context:
- ISO 10007:2017 identity/current status only; no clause-level normative claims.

Dependencies:
- P2.06 supplier-change obligations;
- later traceability/genealogy episodes for production-scale depth.

## 16. P0 check

Unsupported normative claims planned: 0.
Engineering-significant sourced numbers: 0.
Real case facts: 0.
Product-specific compliance claims: 0.

**A8 SCRIPT OUTLINE: COMPLETE — READY FOR FULL SCRIPT DRAFT**
