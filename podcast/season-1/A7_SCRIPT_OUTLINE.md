# A7 Script Outline — Verification Planning Before DVT/PVT Thinking

status: SCRIPT OUTLINE COMPLETE — FULL SCRIPT DRAFT NEXT
season: Season 1 — Build the Right Hardware Before Production Finds Your Mistakes
primary_audience: founders / early hardware teams / systems / test / NPI
lifecycle: DEV-FIRST / CROSS-STAGE
entry_point: YES WITH SHORT REQUIREMENTS/REPRESENTATIVENESS RECAP
production_blueprint: `A7_PRODUCTION_BLUEPRINT.md`
claim_basis: `A7_RESEARCH_PACK.md`
source_lock: `evidence/source-lock/wave-01/W1_A1_A7_A8_CLAIM_LOCK.md`
shared_sources: `evidence/source-lock/wave-01/W1_SHARED_SOURCE_REGISTER.md`
technical_review: `evidence/source-lock/wave-01/W1_INTERNAL_TECHNICAL_REVIEW.md`
outline_contract: `podcast/SCRIPT_OUTLINE_CONTRACT.md`

## 1. Episode job

Listener enters with:
> We ran a lot of tests, so we have a lot of evidence.

Listener leaves with:
> I can define what a test is supposed to prove, which exact configuration it applies to, under what conditions, with what method/measurement, and what decision the evidence may legitimately support.

Primary listener action:
Complete a **Verification Intent Sheet** before the next consequential test.

## 2. Cold open — the expensive test nobody can reuse

[ILLUSTRATIVE]
A team completes weeks of environmental testing and gets clean pass reports. Months later, before production release, somebody asks:
- which enclosure revision was tested?
- which firmware build?
- was the gasket final?
- what exact environmental profile was used?
- was the pass/fail criterion defined before the data?
- did the tested unit include the production-intent connector?

The answers are fragmented or missing.

Core point:
[SYNTHESIS — A7-C01]
Testing created activity and observations. Weak configuration/method/claim linkage made the result difficult to reuse as defensible evidence.

Source anchor:
[AUTH-GUIDANCE]
S-W1-03 NASA Product Verification describes verification records that preserve requirement/product version, methods, tools/equipment, conditions, results and discrepancies.

Guard:
Do not imply the scenario is a real documented case.
Do not imply all exploratory tests need formal release documentation.

## 3. Beat 1 — testing is not automatically verification evidence

Teach three useful modes:
- exploration/debug: learn what is happening;
- verification: obtain evidence against a specified requirement/claim;
- validation: evaluate whether the product satisfies intended use/stakeholder expectations.

[AUTH-GUIDANCE + SYNTHESIS]
Source: S-W1-03 for verification/validation distinction.

Guard:
Do not use `validation` merely to mean `more formal testing`.
Do not claim our three-mode presentation is a formal external taxonomy.

Transition:
For verification, the first question is not `what test can we run?` but `what claim are we trying to support?`

## 4. Beat 2 — the verification chain

Canonical listener chain:
`Requirement/risk/interface claim → decision → article/configuration → conditions → method → measurement → criterion/learning objective → result → applicability → decision → retest trigger`.

[SYNTHESIS informed by S-W1-03]

Walk through each field briefly.

Key engineering point:
A test result does not exist in a vacuum. Its meaning is bounded by the configuration, environment, method and measurement used.

## 5. Beat 3 — plan verification while the design is still flexible

[AUTH-GUIDANCE — A7-C02]
Sources S-W1-01/S-W1-02/S-W1-05 support linking requirements and verification planning.

Example:
A requirement says the device must be serviceable in a tight installed space. If nobody asks how that will be verified until the enclosure is frozen, the team may discover too late that the service interface cannot be accessed or measured realistically.

[SYNTHESIS/ILLUSTRATIVE]

Lesson:
Verification intent is a design input because it exposes ambiguous requirements, inaccessible interfaces and unmeasurable claims before late-stage test.

Guard:
Do not imply every requirement needs a complete formal test procedure during early DEV.

## 6. Beat 4 — representativeness is claim-specific

Reuse A4; do not redefine it.

Example:
A 3D-printed enclosure may be representative enough for connector access and installation geometry but poor evidence for molded-part sealing, material aging or production variation.

[SYNTHESIS / A7-C04 dependency]

Listener question:
`Representative for which claim?`

Do not say `prototype is representative/nonrepresentative` as one binary property.

## 7. Beat 5 — measurement adequacy before confidence

Principle only:
If the method cannot resolve the difference that drives the decision, a crisp number can still be weak evidence.

[DEPENDENCY P2.03 — A7-C05]

Illustrative examples:
- caliper resolution vs tiny tolerance;
- temperature sensor placement vs thermal gradient;
- production test noise vs acceptance boundary.

Guard:
No universal GR&R percentages, 10:1 rules, Cp/Cpk values or other numeric thresholds in A7.
Detailed MSA belongs later.

## 8. Beat 6 — criterion before results, when it is truly a pass/fail test

[SYNTHESIS]
For verification intended to make a pass/fail release decision, define the criterion and decision logic before interpreting the result.

Contrast:
- verification test: criterion pre-defined;
- exploratory characterization: outcome may intentionally refine the model/target.

Guard:
Do not imply all experiments need frozen acceptance limits.

## 9. Beat 7 — one passing unit: what did it prove?

Important nuance from technical review.

[SYNTHESIS]
One unit can sometimes provide valid evidence for a deterministic/configuration-specific requirement if the claim/method justify it.

But one passing article does not, by itself, establish:
- population variation;
- production process capability;
- supplier consistency;
- long-term reliability;
- sustainable production quality.

This prevents the false absolute `one unit proves nothing` while preserving the population/process boundary.

## 10. Beat 8 — change and re-verification

[AUTH-GUIDANCE + SYNTHESIS — A7-C06]
Sources S-W1-02/S-W1-03/S-W1-04 support impact assessment and the need for reverification when relevant changes affect the product/evidence.

Internal rule:
`What changed? → which assumptions/claims/evidence depended on it? → what evidence must be repeated or supplemented?`

Guard:
Do not attribute this exact dependency algorithm to NASA/ISO.
Do not teach `every change = full retest` or `minor change = no retest`.

## 11. Beat 9 — Sentinel Node worked verification

[ILLUSTRATIVE / CANONICAL SENTINEL]

Claim:
The enclosure/connector system maintains required function after the intended wet/environmental exposure.

Early learning test:
- printed enclosure;
- prototype connector;
- engineering assembly;
- objective: expose likely ingress paths.

Useful evidence:
learning about geometry/sealing weak points.

Not automatically transferable to final release if:
- resin/process changes;
- gasket geometry/material changes;
- connector changes;
- fastener/torque process changes;
- production variation becomes relevant.

Production-intent verification later:
bind the evidence to actual configuration, procedure, exposure, measurement and acceptance criteria.

Tool execution:
Fill the Verification Intent Sheet for the later test.

## 12. Beat 10 — DEV / LVP / SVP

DEV:
rapid exploratory tests are valuable; label what they actually prove/learn.

LVP:
important evidence increasingly needs controlled articles, procedures, measurements, criteria and traceable results.

SVP:
release/qualification evidence must remain reconstructable for the released configuration/process envelope, and change/reverification logic must scale.

[SYNTHESIS]

## 13. Misconceptions to challenge

1. `More tests = more confidence.`
2. `Verification starts at DVT.`
3. `A pass proves the whole product.`
4. `One passing unit proves production capability.`
5. `Every change means full retest.`
6. `Exploratory tests are useless later.`
7. `Validation is just a more serious form of verification.`
8. `A precise measurement is automatically an adequate measurement.`

## 14. Closing action

Before the next consequential test, create one page:
`Claim → decision → article/configuration → representativeness → conditions → method → measurement → criterion/learning objective → result location → applicability → retest trigger`.

Ask one final question before starting:
> If this test passes, what exactly will we be justified in saying afterward?

## 15. Handoff to A8

A7 creates meaningful evidence.
A8 answers the problem that appears immediately afterward:
> Six weeks later, can we still reconstruct exactly which hardware, firmware, material, supplier and rework state generated that evidence?

## 16. Source-note skeleton

Spoken external anchors:
- S-W1-03 NASA Product Verification;
- S-W1-01/02/05 for requirements/verification linkage.

Show-notes context:
- ISO/IEC/IEEE 29148:2018 current published identity/status only if useful.

Dependencies:
- A4 representativeness;
- P2.03 measurement-system depth.

## 17. P0 check

Unsupported normative claims planned: 0.
Engineering-significant sourced numbers: 0.
Real case facts: 0.
Product-specific compliance claims: 0.

**A7 SCRIPT OUTLINE: COMPLETE — READY FOR FULL SCRIPT DRAFT**
