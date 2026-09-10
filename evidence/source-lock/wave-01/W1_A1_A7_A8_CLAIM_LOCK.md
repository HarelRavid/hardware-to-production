# Wave 01 Claim Lock — A1 / A7 / A8

status: CLAIM-LEVEL EVIDENCE LOCK COMPLETE
checked: 2026-09-10
shared_sources: `W1_SHARED_SOURCE_REGISTER.md`

## Status vocabulary used here

- `VERIFIED V2` — authoritative engineering guidance directly supports the premise.
- `VERIFIED V2 + V6` — external source supports the engineering premise; the podcast wording/tool remains our synthesis.
- `V6 LOCKED AS SYNTHESIS` — no external attribution is needed at current script scope; wording must remain explicitly ours/general guidance.
- `DEPENDENCY` — detailed source burden belongs to another canonical package and must not be duplicated here.
- `V1 NOT INVOKED` — no named standard requirement is needed for the current script scope.

# A1 — From an Idea to Engineering Requirements

## A1-C01
Claim: A product idea is not yet an engineering requirement set; explicit functional/interface/constraint statements are needed before detailed design can be coordinated.

Lock: `VERIFIED V2 + V6`
Sources: S-W1-01, S-W1-02.
Boundary: NASA supports the requirements-engineering premise. The podcast phrase `idea is not yet a requirement set` is our educational synthesis.

## A1-C02
Claim: useful requirements should be clear enough to support verification or another explicit determination of satisfaction.

Lock: `VERIFIED V2`
Sources: S-W1-01, S-W1-03, S-W1-05.
Exact support: NASA Technical Requirements Definition + requirement-verifiability guidance + Product Verification / Requirements Verification Matrix.

## A1-C03
Claim: requirements/assumptions should be traceable to the need/constraint they serve and to downstream design/verification evidence where practical.

Lock: `VERIFIED V2 + V6`
Sources: S-W1-02, S-W1-03, S-W1-05.
Boundary: NASA directly supports requirements/source/bidirectional traceability and links to test plans/procedures. `where practical` and the startup implementation remain our tailoring.

## A1-C04
Claim: interfaces deserve explicit ownership because multidisciplinary failures often arise from incompatible assumptions across subsystem boundaries.

Lock: `SUPPORTED V2 + V6 — P1 NARRATIVE CLAIM`
Source: S-W1-01.
Boundary: NASA strongly supports explicit definition/control of interfaces. The causal frequency statement about multidisciplinary failures must remain qualitative unless a separate empirical source is added.

Script rule: Prefer `interfaces are explicit engineering objects that must be defined and controlled across teams` over a quantitative/general causal claim.

## A1-C05
Claim: early requirements may remain ranges/targets/TBDs when uncertainty is explicit and paired with a learning action.

Lock: `V6 LOCKED AS SYNTHESIS`.
No external attribution.

## A1-C06
Claim: safety, regulatory and environmental constraints should be surfaced early because they can constrain architecture/design/test choices.

Lock: `VERIFIED V2 + V6`
Source: S-W1-01.
Exact support: NASA Technical Requirements Definition includes environmental, safety and standards/regulatory-type constraints among requirement/constraint inputs.
Boundary: this is an engineering-planning premise, **not** a generic legal claim. Any actual legal/standard obligation requires product/jurisdiction-specific evidence.

## A1-C07
Claim: not every requirement becomes a production CTQ.

Lock: `DEPENDENCY — P2.03`.
A1 may preview this only. Do not define formal CTQ selection/quality methodology here.

## A1-C08
Claim: once a requirement is part of a controlled baseline and drives dependent engineering, changes should be impact-assessed and controlled rather than silently edited.

Lock: `VERIFIED V2 + V6`
Sources: S-W1-02, S-W1-04.
Boundary: supplier/tooling/acceptance examples are Hardware-to-Production application examples, not a NASA-required trigger list.

## A1-C09
Claim: development verification and production acceptance are different evidence problems even when related characteristics are measured.

Lock: `V6 LOCKED AS LIFECYCLE SYNTHESIS`, with S-W1-03 supporting the verification side.
Dependency: production-acceptance specifics belong to later quality/production source packs.

## A1-C10
Claim: requirements maturity should increase from DEV → LVP → SVP rather than being binary `none/frozen`.

Lock: `V6 LOCKED AS SYNTHESIS`.
No external lifecycle-standard attribution.

### A1 gate
P0 external-premise blockers at current non-normative script scope: `0`.

Decision:
`A1 EVIDENCE VERIFIED FOR CURRENT SCRIPT SCOPE — TECHNICAL REVIEW PENDING`.

ISO rule:
Do not say `ISO 29148 requires ...` unless the exact licensed clause is separately verified.

---

# A7 — Verification Planning Before DVT/PVT Thinking

## A7-C01
Claim: a test result is meaningful only relative to the claim, configuration, conditions and method actually exercised.

Lock: `VERIFIED V2 + V6`
Source: S-W1-03.
Exact support: NASA verification work products record requirement/version of product/version of requirements/tools/equipment/procedures/environments/results/discrepancies.
Boundary: our compact four-part formulation is synthesis.

## A7-C02
Claim: verification planning should begin while requirements/interfaces are being matured, not only after nominal design completion.

Lock: `VERIFIED V2`
Sources: S-W1-01, S-W1-02, S-W1-05.

## A7-C03
Claim: exploratory learning tests and release/qualification evidence are different evidence classes.

Lock: `V6 LOCKED AS SYNTHESIS`.
NASA supports formal verification work-product discipline but this exact two-class framing is ours.

## A7-C04
Claim: representativeness is claim-specific.

Lock: `DEPENDENCY / V6`.
Canonical owner: A4 prototype representativeness/source package.
A7 reuses the concept; it must not re-source/redefine it.

## A7-C05
Claim: measurement adequacy matters before strong acceptance/capability conclusions.

Lock: `DEPENDENCY — P2.03`.
A7 may state the principle only. Numerical MSA/capability criteria are prohibited until the quality source-lock wave.

## A7-C06
Claim: a change requires re-verification where it affects the evidence dependency/demonstrated claim, not automatically everywhere.

Lock: `VERIFIED PREMISE V2 + V6 RULE`
Sources: S-W1-02, S-W1-03, S-W1-04.
NASA supports impact assessment and that changed products/nonconformances may require reverification. The **targeted dependency-based scope** is our frozen global invariant, not a quoted NASA rule.

## A7-C07
Claim: passing one end test does not automatically prove all intermediate failure mechanisms are controlled.

Lock: `V6 LOCKED AS SYNTHESIS`.
No external attribution at current scope.

## A7-C08
Claim: verification evidence should remain traceable to the configuration and procedure that generated it.

Lock: `VERIFIED V2`
Sources: S-W1-03, S-W1-04.

### A7 gate
P0 named-standard blockers at current scope: `0`.

Decision:
`A7 EVIDENCE VERIFIED FOR CURRENT SCRIPT SCOPE — TECHNICAL REVIEW PENDING`.

DVT/PVT rule:
DVT/PVT remain contextual industry labels; this episode does not present them as universally standardized phases.

---

# A8 — Configuration Management from Prototype #1

## A8-C01
Claim: evidence should remain linked to the exact product/configuration that generated it.

Lock: `VERIFIED V2 + V6`
Sources: S-W1-03, S-W1-04.

## A8-C02
Claim: definition, as-built/as-run state and evidence are distinct objects that should remain traceably linked.

Lock: `VERIFIED PREMISE V2 + V6 MODEL`
Sources: S-W1-03, S-W1-04.
Boundary: NASA supports controlled product/configuration/version records and verification records. The three-object model wording is our canonical synthesis.

## A8-C03
Claim: lightweight configuration control can begin in DEV without enterprise PLM/MES tooling.

Lock: `V6 LOCKED AS SYNTHESIS`.
No claim that NASA/ISO endorses a spreadsheet/Git implementation.

## A8-C04
Claim: rework/deviation should add history rather than overwrite the failed/original state.

Lock: `V6 LOCKED AS GLOBAL INVARIANT`.
S-W1-03 supports capture of anomalies/corrective actions/discrepancies; our `rework adds history` formulation remains synthesis.

## A8-C05
Claim: change should trigger impact/re-verification only where relevant claims/evidence dependencies are affected.

Lock: `VERIFIED PREMISE V2 + V6 RULE`
Sources: S-W1-02, S-W1-03, S-W1-04.
Boundary: NASA supports impact assessment and reverification after affected changes. Exact dependency-scoping logic is ours.

## A8-C06
Claim: hardware, firmware/software, calibration/configuration and test-procedure identity can interact and should be considered together when they contribute to the claim.

Lock: `VERIFIED V2 + V6`
Source: S-W1-03 supports version/context capture across product, requirements, tools/data/equipment/procedures; S-W1-04 supports product/configuration identification.

## A8-C07
Claim: multiple suppliers/lots/alternates increase the importance of as-built identity because nominal equivalence does not itself prove equal evidence.

Lock: `DEPENDENCY — P2.06`, with V6 use permitted as a qualitative preview.
No supplier requalification rule may be attributed here until the supplier source-lock wave.

## A8-C08
Claim: configuration control enables population segmentation for defects, changes and field signals.

Lock: `V6 LOCKED AS SYNTHESIS`, supported by the general status-accounting/reconstructability premise from S-W1-04.

### A8 gate
P0 external-premise blockers at current script scope: `0`.

Decision:
`A8 EVIDENCE VERIFIED FOR CURRENT SCRIPT SCOPE — TECHNICAL REVIEW PENDING`.

ISO rule:
ISO 10007 may be named as a configuration-management guidance standard and its current edition/status may be stated. Do not state detailed ISO 10007 process requirements as normative without controlled full-text verification.

---

# P2.02 shared claim lock

## P2-C-CM-001
A successful test result is weak evidence if tested configuration cannot be reconstructed.
Status: `VERIFIED V2 + V6` via S-W1-03/S-W1-04.

## P2-C-CM-002
Release revision and production effectivity are different concepts.
Status: `V6 LOCKED AS SYNTHESIS — FORMAL EFFECTIVITY TERMINOLOGY STILL ENRICHABLE`.
Do not claim ISO/NASA defines our exact distinction unless separately verified.

## P2-C-CM-003
An approved change is not complete until implementation and applicable verification are confirmed.
Status: `VERIFIED V2` via NASA SEH 6.5.1.2.3.

## P2-C-CM-004
Supplier/component substitution can require reevaluation even if form/fit appears unchanged.
Status: `DEPENDENCY — P2.06` for external/industry obligations; allowed as V6 engineering synthesis before then.

## P2-C-CM-005
Deviation/waiver should remain distinguishable from a baseline engineering change.
Status: `VERIFIED V2 IN NASA TERMINOLOGY`; local/industry terminology varies and must be stated.

# Final Wave 01 claim decision

No selected A1/A7/A8 claim currently requires an unsupported named-standard SHALL statement.

No known V1 claim has been falsely upgraded.

The three episodes may progress to **technical review** under the current non-normative script architecture.

**W1 CLAIM LOCK: PASS**
