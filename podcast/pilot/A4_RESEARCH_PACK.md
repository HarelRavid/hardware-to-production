# A4 Research Pack — Choosing Prototype Technologies Without Trapping the Product

status: CLAIM SET STABLE
season: Season 1 — Build the Right Thing
primary_audience: Audience A — founders / early hardware development teams
secondary_audience: mechanical, electronics, embedded, test, NPI, supplier leads
lifecycle: DEV-FIRST / CROSS-STAGE
entry_point: ALTERNATIVE SERIES ENTRY FOR TEAMS ALREADY PROTOTYPING
technical_depth: foundation-practitioner
backbone_anchor: `domains/dfx-foundations/PROTOTYPE_REPRESENTATIVENESS_CROSS_PROCESS_GATE.md`

## 1. Episode promise
Teach a team to use fast prototype technologies aggressively without confusing prototype success with production evidence.

Canonical listener question:
> Which parts of what this prototype taught us can safely travel forward — and which conclusions expire when the material, process, supplier, tooling, software or production rate changes?

## 2. Navigation card
**You are here:** Architecture / POC → Integrated Prototype → Engineering Prototype

**Best for:** teams already building with dev boards, 3D-printed/CNC parts, temporary harnesses, lab fixtures or prototype suppliers.

**You should already know:** product intent and the rough function/interfaces being tested. A1/A3 are useful but not mandatory; include a concise recap.

**You will leave with:** Prototype Evidence Transfer Matrix + Shortcut Expiration Card.

**Prototype shortcut:** use non-production materials/processes/components when they accelerate learning and their representativeness limits are explicit.

**Shortcut expires when:** the next decision depends on a dimension the prototype does not represent.

**Next:** A5/A6 → A7 verification → A8 configuration; later Episode 1/6/11 for industrialization and process selection.

## 3. Audience contract
### DEV takeaway
Pick the fastest prototype method that answers the current engineering question — not the method that looks most like a factory by default.

### Prototype shortcut
Dev boards, printed/machined bridge parts, hand wiring, manual assembly and temporary fixtures can be legitimate when their evidence boundary is explicit.

### Shortcut expiration
A shortcut expires when decisions about performance, reliability, compliance, manufacturing capability, supplier qualification, tooling, rate or cost depend on properties it does not reproduce.

### LVP change
Prototype routes progressively give way to production-intent components/materials/processes, or are deliberately retained as controlled bridge manufacturing.

### SVP evidence
Serial-production release evidence must be representative for the specific claim being made; there is no single universal notion of a “representative prototype.”

## 4. Canonical representativeness principle
Backbone rule:
> Prototype evidence transfers only to the dimensions for which the prototype is representative.

Representativeness vector:
- geometry;
- material;
- manufacturing process;
- surface/finish;
- joining/assembly;
- tooling;
- supplier;
- process variation;
- inspection/test;
- software/configuration;
- environment/load;
- production rate.

This is a claim-dependent map, not a scalar score.

## 5. Core claim register — stabilized
| ID | Claim | Class | Priority | Status | Applicability / note |
|---|---|---|---|---|---|
| A4-C01 | Evidence from a prototype/test article should be used only for claims supported by the configuration, interfaces, environment and other relevant characteristics actually represented by that article. | V6 + authoritative V&V support | P0 | STABLE | NASA V&V guidance supports explicit test articles/configurations and testing under operationally relevant conditions; our generalized vector is repository synthesis. |
| A4-C02 | A prototype made by a different manufacturing process may validate geometry/function while not validating production-process-specific failure mechanisms, capability or economics. | V6 | P0 | STABLE SYNTHESIS | Claim must be applied dimension-by-dimension, not universally. |
| A4-C03 | Prototype-versus-production representativeness is multidimensional rather than binary. | V6 | P0 | STABLE SYNTHESIS | Canonical repository framework. |
| A4-C04 | A temporary DEV choice is acceptable when its learning objective, evidence boundary and expiration trigger are explicit. | V6 | P1 | STABLE SYNTHESIS | Internal lifecycle rule, not external normative requirement. |
| A4-C05 | Production-intent transition should be triggered by the evidence required for the next decision, plus risk/economics/lifecycle maturity, rather than a universal prototype-generation number. | V6 | P1 | STABLE SYNTHESIS | Avoid universal EVT/DVT/PVT prescriptions. |
| A4-C06 | A change invalidates the evidence dependent on changed attributes; it does not logically invalidate unrelated evidence by default. | V6 + P2.02 | P0 | STABLE | Evidence-dependency/change-impact rule. Formal requalification requirements remain product/industry specific. |
| A4-C07 | Bridge manufacturing may remain valid into LVP when controlled quality, configuration, rate, cost and risk are acceptable. | V6 + P2.05 | P1 | STABLE SYNTHESIS | Economics/applicability explicit. |
| A4-C08 | Visual or dimensional similarity alone is insufficient evidence for claims that depend on material, process, environment, reliability or compliance behavior. | V6 + V&V principle | P0 | STABLE | Do not infer specific failure mechanisms without process-specific evidence. |
| A4-C09 | Low-volume prototype builds do not by themselves establish production-rate/process-capability evidence. | V6 + P2.04/P2.06 | P1 | STABLE | Keep distinction between functional evidence and manufacturing evidence. |
| A4-C10 | Prototype/test identity and configuration should remain reconstructable when evidence is expected to support later engineering decisions. | V6 + P2.02/P2.08 | P1 | STABLE | Supports traceability and change-impact reasoning. |

## 6. Source-verification note
Authoritative source support is deliberately narrow. NASA Systems Engineering Handbook material separates verification from validation, includes explicit treatment of test articles, and describes verification approaches including test, analysis, demonstration and inspection. NASA software verification guidance further states that target hardware/configuration and operational conditions should be as close as practical to the intended environment when those characteristics matter to verification.

These sources support the evidence-boundary principle; they do **not** define our twelve-dimension representativeness vector or the REPRESENT 8 framework. Those remain clearly labeled repository synthesis.

Source targets retained for final source packet:
- NASA Systems Engineering Handbook — Product Realization / V&V and Appendix material;
- NASA Systems Engineering Handbook — Requirements Verification Matrix / test article guidance;
- NASA Software Engineering Handbook verification guidance as an illustrative authoritative source for configuration/environment fidelity;
- process-specific authoritative sources only when a final script makes a specific material/process claim.

## 7. Prototype Evidence Transfer Matrix — listener tool
| Dimension | Representative? | Difference | Claim still valid | Claim NOT valid | Next evidence needed |
|---|---|---|---|---|---|
| Geometry | | | | | |
| Material | | | | | |
| Manufacturing process | | | | | |
| Surface/finish | | | | | |
| Joining/assembly | | | | | |
| Tooling/fixture | | | | | |
| Supplier/source | | | | | |
| Process variation | | | | | |
| Inspection/test | | | | | |
| Software/configuration | | | | | |
| Environment/load | | | | | |
| Rate/volume | | | | | |

Better question:
> Representative enough for which claim?

## 8. Shortcut Expiration Card — listener tool
1. **Shortcut** — what differs from the likely production route?
2. **Why now** — what learning/speed/cost advantage does it buy?
3. **What it proves** — which claims can use this evidence?
4. **What it does NOT prove** — which dimensions/failure modes are not represented?
5. **Expiration trigger** — what decision/lifecycle event makes it inadequate?
6. **Replacement route** — what more representative route is expected?
7. **Revalidation** — which dependent claims must be rechecked?
8. **Owner/date** — who prevents the shortcut becoming invisible debt?

## 9. Worked examples
### CNC prototype → injection-molded housing
May strongly support package geometry, mounting/interface fit and service-access learning while providing weak evidence for molding-specific behavior, production tooling capability, process variation and production economics. Exact conclusions depend on materials and processes.

### 3D-printed enclosure → production polymer
May support volume, shape, cable routing and ergonomics. It does not automatically support strength, creep, sealing, environmental, fire/compliance or long-term dimensional claims. Exact differences are technology/material specific.

### Dev board → custom PCB
May support processor/sensor concept, firmware logic and communications proof. It does not automatically prove final power integrity, thermal behavior, EMC, production programming/test access, lifecycle/supply or final hardware/firmware behavior.

### Hand-wired harness → production harness
May support pinout/function learning without proving production crimp quality, strain relief, routing, repeatability, identification, traceability or production inspection/test.

## 10. Sentinel Node staged evolution
### DEV-0
Dev board + sensor module + printed enclosure + bench supply + jumper wiring + laptop logging.

Evidence earned: sensing principle and basic firmware/communications under bench conditions.

Evidence not earned: final environmental sealing, thermal behavior, EMC/compliance, assembly repeatability, supplier/process capability, production rate/economics.

### DEV-1
Custom PCB Rev A, representative connector candidate, more representative enclosure, controlled firmware identity and instrumented testing. More evidence is earned, but LVP production capability is still a separate question.

### Production-intent / LVP transition
Released configuration, critical approved sources, intended assembly/fixture, controlled programming/calibration/test, genealogy, and representative process/operator conditions where required by the claim.

## 11. Common failure modes
- “It passed on the prototype” with no evidence-boundary statement.
- Production theater: early NRE spent to look production-like without answering a useful question.
- Shortcut fossilization: temporary choices survive because expiration was never recorded.
- Revalidate everything: total retest because evidence dependencies were never mapped.
- Scale blindness: three careful builds treated as proof for hundreds.
- Geometry-only thinking while material/process/assembly/software/environment changed.

## 12. Decision method — REPRESENT 8
1. **Question**
2. **Claim**
3. **Dimensions**
4. **Differences**
5. **Failure modes**
6. **Expiration**
7. **Next evidence**
8. **Record**

This is repository synthesis, not an external industry standard.

## 13. Applicability statement
Applies to general multidisciplinary hardware prototyping and industrialization. It is an evidence-transfer decision method, not a substitute for prescribed qualification articles, process-specific standards or regulated-product validation requirements.

## 14. Must NOT claim
- prototypes should always use production materials/processes;
- non-production prototypes are weak;
- production-intent prototypes automatically prove process capability;
- different-process prototypes provide zero useful evidence;
- DEV/LVP/SVP are standardized lifecycle labels;
- every change requires full requalification;
- one representativeness score replaces claim-specific judgment.

## 15. Navigation
Standalone entry allowed. Recap A1 requirement/claim concept, A3 interfaces if needed, and DEV/LVP/SVP. Then route to A7 → A8 → Episode 1, or Episode 6/11 for process selection.

## 16. Remaining work before SCRIPT ELIGIBLE
1. Package exact source citations/excerpts in the episode source packet.
2. Verify any process-specific statements retained in final script.
3. Mechanical + electronics + NPI technical review.
4. Optional real-world case only if it improves the lesson without creating provenance ambiguity.
5. Run Episode Packaging Contract gate.

## 17. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation entry-point fit: STRONG
Prototype-shortcut contract: STRONG
Claim set: STABLE
Standards burden: LOW
Quantitative burden: LOW
Backbone risk: LOW
Source verification: SUFFICIENT FOR CLAIM-SET STABILITY; FINAL SOURCE PACK OPEN

Next status target:
`CLAIM SET STABLE → SCRIPT ELIGIBLE`
