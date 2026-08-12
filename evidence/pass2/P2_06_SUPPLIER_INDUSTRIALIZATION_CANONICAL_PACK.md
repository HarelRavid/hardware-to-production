# P2.06 — Supplier Industrialization Canonical Pack

**Status:** NEAR PODCAST READY  
**Purpose:** Canonical evidence-backed framework for supplier industrialization from source selection through sustained production and controlled change.

## 1. Core claim

A supplier is not qualified in the abstract. Approval is meaningful only for a defined product/process/configuration/rate envelope supported by evidence.

Prototype success, a good first article, production approval, demonstrated rate capability, and sustained supplier performance answer different questions and must not be collapsed into one label such as “approved supplier.”

## 2. Canonical lifecycle

**Requirement → Source/Select → Qualify → Production-Intent Evidence → Production Approval → Rate/Ramp → Ongoing Performance → Change Control → Requalification/Recovery**

### 2.1 Requirement
Define CTQs, special/critical characteristics, specifications, expected volume/rate, traceability, packaging, test/inspection, documentation, regulatory/customer-specific requirements, and required notification rules.

### 2.2 Source / Select
Evaluate technical process fit, quality system, relevant equipment, capacity, financial/continuity risk, sub-tier dependencies, measurement capability, lead time, TCO, communication, and development maturity.

### 2.3 Qualify
Generate evidence using representative material, tooling, process route, operators, measurement and controls. Prototype evidence is useful but its applicability is limited to the demonstrated envelope.

### 2.4 Production-intent evidence
The evidence becomes stronger when parts come from production-intent tooling/processes and the supplier can demonstrate controlled inputs, CTQ measurement, traceability, process controls and disposition of nonconformance.

### 2.5 Production approval
Where PPAP or a comparable customer approval system applies, the objective is not merely a correct sample. AIAG describes PPAP as demonstrating that engineering design/specification requirements can be consistently met during an actual production run at production rates.

**Guardrail:** PPAP is an automotive-origin framework and is not automatically mandatory for every hardware company. The transferable principle is evidence-based production approval under representative conditions.

### 2.6 Rate / ramp
Approval of a part does not automatically prove capacity. Verify actual production rate, constraint, staffing, uptime, yield/rework, replenishment, material availability and recovery behavior against required demand.

### 2.7 Ongoing performance
Track multiple dimensions rather than a single purchasing score: quality escapes, PPM/rejects, FPY where available, OTD, responsiveness, corrective-action closure, capacity risk, traceability integrity, change discipline and recurring failure modes.

### 2.8 Change control
Supplier approval remains valid only inside the approved/demonstrated envelope. Changes to material, sub-tier, process, tooling, site, equipment, software/test method, inspection method, packaging or other relevant assumptions trigger impact assessment.

### 2.9 Requalification / recovery
Requalification scope should be proportional to what changed and which prior evidence assumptions were invalidated. Do not automatically re-run everything; do not automatically reuse evidence that no longer applies.

## 3. SUPPLIER 10 — listener framework

1. **Requirement** — What must the supplier actually control and prove?
2. **Process** — What manufacturing process creates the part and its risks?
3. **Representativeness** — Was the evidence generated with production-intent conditions?
4. **Measurement** — Can the supplier reliably measure the CTQs?
5. **Capability** — What evidence supports repeatability/capability at the required state?
6. **Sub-tier** — Which critical materials/processes are outside the direct supplier?
7. **Traceability** — Can affected product populations be identified?
8. **Change** — What changes require notification, review or requalification?
9. **Recovery** — How are escapes, shortages, capacity loss and corrective actions handled?
10. **Sustainment** — Does performance remain acceptable over time and at the required rate?

## 4. Supplier approval ladder

| State | What is demonstrated | What is NOT yet demonstrated |
|---|---|---|
| Candidate | Commercial/technical possibility | Repeatable production |
| Prototype-capable | Can make useful prototype parts | Production-intent process/rate |
| Production-intent qualified | Representative process evidence exists | Sustained production |
| Production approved | Defined approval evidence accepted | Future capacity/sustainment under all conditions |
| Rate demonstrated | Required rate shown in defined envelope | Long-term robustness by itself |
| Sustained supplier | Performance maintained with controlled changes | Immunity from future degradation/change |

## 5. Sentinel Node worked example — Supplier Alpha

### DEV
Supplier Alpha machines 12 CNC enclosures. Dimensional results and workmanship are excellent. The team is tempted to call Alpha “qualified.”

Correct interpretation: Alpha has demonstrated useful prototype capability for the CNC route.

### LVP transition
The product moves to injection molding and demand rises toward 600 units/month. New evidence is needed for mold/tooling condition, resin control, cavity-to-cavity behavior, gasket-land CTQ, insert placement, process window, measurement, packaging, traceability and rate.

### LVP signal
120 enclosures arrive. 109 are accepted without the identified issue and 11 require rejection/rework associated mainly with gasket-land and insert-placement behavior. Investigation suggests concentration around cavity 3, but cavity identity was not preserved in part genealogy.

**Lesson:** data without the contextual identity needed to segment it can be insufficient evidence.

### Supplier change
Alpha later changes the gasket-material sub-tier to improve lead time. Geometry may be unchanged, so existing dimensional evidence may remain applicable to geometry. But sealing/compression/environmental evidence that depended on material properties must be reassessed.

The correct question is not “Do we repeat the whole qualification?” but “Which supported claims lost their evidentiary basis?”

## 6. CHANGE 9 — supplier-change decision tool

1. What changed?
2. Why did it change?
3. Which requirement/CTQ can it affect?
4. Which prior evidence supports that requirement?
5. Which assumptions behind that evidence changed?
6. What analysis/test/reverification/requalification is proportionate?
7. What is the approved effectivity/cut-in?
8. How will affected WIP/stock/field population be identified and controlled?
9. What evidence closes temporary containment and returns the supplier to normal control?

## 7. Supplier scorecard architecture

Do not hide engineering risk inside one weighted score.

### Performance indicators
- OTD
- incoming rejects / PPM where meaningful
- customer/line escapes
- supplier FPY/rework where available and trustworthy
- corrective-action response and closure
- responsiveness
- lead-time stability
- capacity adherence
- traceability integrity
- change-notification compliance
- recurring failure modes

### Hard-stop examples
A supplier can have excellent OTD and price and still be RED if a critical governance/evidence failure exists, such as:
- unauthorized material/process/sub-tier change;
- inability to identify affected product population;
- repeated critical escapes;
- inadequate measurement for a critical characteristic;
- inability to demonstrate required production rate;
- unresolved systemic corrective action.

NIST MEP describes supplier metrics/scorecards as important for performance measurement, improvement and sourcing decisions, while also treating supplier evaluation, selection, TCO and strategic supplier relationships as broader management activities. A scorecard is therefore an input to supplier governance, not a substitute for engineering judgment.

## 8. Sub-tier and critical-process principle

The direct supplier is not necessarily the full process boundary. Critical characteristics can be created or altered by material producers, plating/heat-treatment houses, molding compound suppliers, calibration laboratories, PCB assemblers, special-process providers and other sub-tiers.

AIAG CQI-19 explicitly addresses sub-tier supplier management and pass-through characteristics. Nadcap provides an industry-specific example of independent accreditation/oversight for special processes. These examples support the transferable principle that critical outsourced process evidence must remain visible and controlled.

**Guardrail:** sector-specific accreditation or PPAP requirements must not be presented as universal requirements outside their applicability.

## 9. Evidence hierarchy for supplier claims

**E1 — Direct representative production evidence**  
Generated from the intended supplier/process/tooling/material/rate envelope.

**E2 — Representative qualification evidence**  
Strong but not yet sustained over production time/rate.

**E3 — Analogous/process-family evidence**  
Useful with explicit applicability limits.

**E4 — Supplier statement / forecast / assumption**  
Useful for planning, weak for readiness claims until verified.

A supplier claim should never silently move from E4 to E1 because the project needs the schedule to work.

## 10. Canonical decision gates

### Gate A — Source decision
Can this supplier plausibly satisfy technical, quality, commercial and continuity requirements?

### Gate B — Prototype authorization
Is the supplier suitable for learning/prototype builds, with explicit limits on what those builds prove?

### Gate C — Production-intent qualification
Does representative evidence support the intended process/configuration?

### Gate D — Production approval
Are required approval artifacts and engineering evidence accepted for the defined envelope?

### Gate E — Ramp authorization
Has required rate/capacity, yield, recovery and supply readiness been demonstrated sufficiently for the ramp claim?

### Gate F — Sustained status
Is ongoing performance acceptable, and are changes controlled?

### Gate G — Change/recovery
After a significant change or systemic failure, what evidence is required to restore the previous approval state?

## 11. Common myths to break in the podcast

- “They made 10 perfect prototypes, so they are a production supplier.”
- “FAI passed, therefore capacity is proven.”
- “PPAP/production approval means the supplier will always remain capable.”
- “OTD + price is enough to rank suppliers.”
- “Same drawing means a supplier/material/process change needs no new evidence.”
- “Our Tier-1 supplier owns the sub-tier risk, so we do not need visibility.”
- “A certificate is equivalent to evidence for our actual CTQs.”

## 12. Podcast-ready teaching sequence

1. Start with the 12 perfect CNC prototypes.
2. Ask: “What exactly did they prove?”
3. Change process and volume at LVP.
4. Reveal cavity-related defects and missing genealogy.
5. Separate sample approval from production/rate evidence.
6. Introduce SUPPLIER 10.
7. Introduce the unauthorized sub-tier change.
8. Apply CHANGE 9 to determine requalification scope.
9. Show why a green commercial scorecard can coexist with RED engineering risk.
10. Close with the approval-envelope principle.

## 13. Canonical podcast lines

> A supplier is not qualified in the abstract; an evidence-backed production envelope is qualified.

> Prototype success proves what happened in the prototype process — not what will happen at production rate.

> Supplier approval is a state that must survive evidence, rate, time and controlled change.

> A green delivery score cannot compensate for an uncontrolled engineering change.

> Evidence is valid only inside the process and configuration envelope that produced it.

## 14. Source backbone

- AIAG — Production Part Approval Process (PPAP): production approval and consistent conformance during actual production runs at production rates.
- AIAG — CQI-19 Sub-Tier Supplier Management Process Guideline: sub-tier quality management and pass-through characteristics.
- NIST MEP — Supply Chain Management: supplier evaluation/selection, TCO, supplier development and performance scorecards.
- NIST — supply-chain risk guidance: scorecards should mix relevant quantitative and qualitative risk/performance indicators rather than become a blind single metric.
- PRI/Nadcap — sector-specific example of accreditation/oversight for critical/special processes.

## 15. Provenance / applicability note

The lifecycle, SUPPLIER 10, CHANGE 9, approval ladder, hard-stop logic, evidence classes and Sentinel Node examples are project synthesis frameworks. They are not represented as clauses copied from AIAG, NIST, ISO, IATF or Nadcap.

Industry-specific requirements such as PPAP, IATF customer-specific requirements, AS9145/AS9102, Nadcap or medical-device supplier controls must be applied only when the product, customer, contract and regulatory context makes them applicable.

## 16. Readiness status

**P2.06 status: NEAR PODCAST READY**

Completed:
- supplier lifecycle architecture;
- source/selection principles;
- production-intent qualification logic;
- PPAP applicability guardrail;
- rate/capacity distinction;
- sub-tier principle;
- change/requalification decision tree;
- six-month scorecard concept and hard-stop logic;
- Sentinel Node worked example;
- SUPPLIER 10 and CHANGE 9 listener tools;
- canonical teaching sequence.

Remaining before PODCAST READY:
- episode-specific source-note packaging;
- final technical/editorial review;
- optional cross-industry contrast (automotive vs aerospace vs general industrial hardware) where editorially useful.
