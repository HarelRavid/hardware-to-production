# A7 Research Pack — Verification Planning Before DVT/PVT Thinking

status: RESEARCH PACK OPEN
season: Season 1 — Build the Right Thing
primary_audience: Audience A — founders / early hardware development teams
secondary_audience: systems, mechanical, electronics, embedded, test, NPI, quality
lifecycle: DEV-FIRST / CROSS-STAGE
entry_point: FOUNDATION FOR TEAMS MOVING FROM BUILDING TO PROVING
technical_depth: foundation-practitioner

## 1. Episode promise
Teach early hardware teams to plan verification before test activity becomes a late-stage scramble, without forcing a full regulated qualification bureaucracy into early DEV.

Canonical listener question:
> How do we decide what this next build/test must prove, which configuration it proves it on, and what evidence will still matter later?

## 2. Navigation card
**You are here:** Serious prototype → planned evidence → controlled learning.

**Best for:** teams that already have functional prototypes and are beginning environmental, performance, interface, reliability or acceptance testing.

**You should already know:** A1 requirements and A3/A4 concepts are helpful but not mandatory; include concise recap.

**You will leave with:** Verification Intent Sheet + Evidence-to-Claim Review.

**Prototype shortcut:** informal bench tests and exploratory experiments are valid while the objective is learning rather than release evidence.

**Shortcut expires when:** a result will be used to release a design/configuration, support a customer/compliance claim, qualify a supplier/process, establish production acceptance or avoid repeating an expensive test later.

**Next:** A8 Configuration Management from Prototype #1 → Episode 1 industrialization transition.

## 3. Audience contract
### DEV takeaway
Before testing, write down the claim, configuration, conditions, method and decision the result is meant to support.

### Prototype shortcut
Exploratory testing can remain flexible, but it should be labeled as learning evidence rather than silently upgraded into qualification evidence.

### Shortcut expiration
When evidence must survive design change, supplier transfer, formal review or production release, configuration identity and test intent become controlled.

### LVP change
Verification increasingly links requirements/CTQs to representative articles, controlled procedures, calibrated measurement where needed, traceable results and change impact.

### SVP evidence
Release/qualification evidence must remain reconstructable and applicable to the released configuration/process envelope.

### Manufacturing-debt prevention
Do not wait for DVT/PVT labels to ask how a requirement will be demonstrated or whether the prototype represents the eventual claim.

### Listener action
For the next major test, create a one-page Verification Intent Sheet before touching the lab setup.

## 4. Core conceptual chain
Requirement / risk / interface claim
→ verification question
→ article/configuration
→ conditions / environment / load
→ method / measurement
→ acceptance or learning criterion
→ execution record
→ result
→ applicability
→ decision
→ change / re-verification trigger

## 5. Core claim register — draft
| ID | Claim | Class | Priority | Status | Note |
|---|---|---|---|---|---|
| A7-C01 | A test result is meaningful only relative to the claim, configuration, conditions and method it actually exercised. | V2/V6 | P0 | OPEN | Authoritative verification guidance needed. |
| A7-C02 | Verification planning should begin while requirements/interfaces are being matured, not only after the design is nominally complete. | V2/V6 | P0 | OPEN | Systems-engineering support. |
| A7-C03 | Exploratory learning tests and formal release/qualification evidence are different evidence classes even if they use similar hardware or measurements. | V6 + P2.03 | P0 | BACKBONE-STABLE | |
| A7-C04 | Test-article representativeness must be assessed claim-by-claim; a prototype can be representative for one claim and weak for another. | V6 + A4 | P0 | BACKBONE-STABLE | |
| A7-C05 | Measurement adequacy matters before strong acceptance/capability conclusions are drawn. | V2/V6 + P2.03 | P0 | BACKBONE-STABLE / source open | |
| A7-C06 | A change requires re-verification only where it affects the evidence dependency or demonstrated claim. | V6 + P2.02 | P0 | BACKBONE-STABLE | |
| A7-C07 | Passing one end test does not automatically prove all intermediate failure mechanisms are controlled. | V6 + P2.03 | P1 | BACKBONE-STABLE | |
| A7-C08 | Verification evidence should remain traceable to the configuration and procedure that generated it. | V2/V6 + P2.02/P2.08 | P0 | OPEN | Source support useful. |

## 6. Listener tool — Verification Intent Sheet
For every consequential test:
| Field | Question |
|---|---|
| Claim/requirement | What are we trying to prove/learn? |
| Decision | What decision will use the result? |
| Article | Which physical unit/build is tested? |
| Configuration | HW/BOM/FW/material/process version? |
| Representativeness | Which dimensions are/aren't representative? |
| Conditions | load/environment/state/duty cycle? |
| Method | how is the test executed? |
| Measurement | instrument/method adequate for the conclusion? |
| Criterion | what counts as pass, fail or learning outcome? |
| Result record | where is raw/result data stored? |
| Applicability | what exact claim/envelope does the result support? |
| Re-test trigger | what change would require new evidence? |

## 7. Evidence-to-Claim Review
Before accepting a result ask:
1. Did the tested configuration match the claim?
2. Were relevant interfaces/materials/processes represented?
3. Were test conditions representative or intentionally accelerated/limited?
4. Is the measurement method adequate?
5. Were deviations/failures recorded rather than hidden by rework?
6. Does the conclusion exceed what the test actually exercised?
7. What change would invalidate the evidence?
8. Is this learning evidence, release evidence, or both?

## 8. Worked example — Sentinel Node environmental test
Question: can the enclosure/connector interface maintain function after the target environmental exposure?

Early exploratory test:
- printed enclosure;
- prototype connector;
- one unit;
- engineering setup;
- objective: identify likely ingress/thermal weak points.

Useful as learning evidence.

Not sufficient by itself for release if final resin, molded geometry, gasket compression, connector source, assembly method or production variation differ materially.

Production-intent verification later should explicitly bind the result to the released configuration and representative assembly/test conditions.

## 9. Common failure modes
- “We already tested that” with no reconstructable configuration.
- test article differs from released design in a failure-relevant way.
- acceptance threshold invented after data are seen.
- result is reused for a broader claim than the method supports.
- one passing unit is treated as process capability.
- measurement uncertainty/resolution is ignored.
- failed unit is reworked and only the final pass survives in records.

## 10. Standards/source targets
Priority source families:
- NASA Systems Engineering Handbook / verification guidance;
- ISO/IEC/IEEE 29148 where exact requirements-verification language is useful and applicable;
- product/industry-specific environmental, safety, reliability or compliance standards only when a later episode makes those claims.

Guardrail:
This episode is about evidence architecture, not teaching a universal DVT/PVT prescription.

## 11. Applicability statement
General hardware verification-planning framework. It does not replace mandated qualification/validation protocols in regulated, safety-critical, aerospace, automotive, medical or customer-controlled programs.

## 12. What this episode must NOT claim
- every prototype test needs formal qualification paperwork;
- a single test result proves serial production capability;
- DVT/PVT are universal standards-defined phases;
- accelerated tests automatically represent field life;
- every design change requires a full test campaign;
- measurement data are trustworthy without considering method adequacy.

## 13. Research backlog before CLAIM SET STABLE
1. Package authoritative systems-engineering verification support.
2. Verify terminology for verification vs validation without overgeneralizing industry-specific meanings.
3. Cross-link measurement adequacy to Episode 24/P2.03.
4. Technical review: systems/test + NPI/quality.
5. Keep DVT/PVT labels contextual rather than universal.

## 14. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: LOW–MEDIUM
Quantitative burden: LOW
Backbone risk: LOW
Source verification: OPEN

Next status target:
`RESEARCH PACK OPEN → CLAIM SET STABLE`
