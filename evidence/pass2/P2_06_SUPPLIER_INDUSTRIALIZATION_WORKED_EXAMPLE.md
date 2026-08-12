# P2.06 — Supplier Industrialization Worked Example

**Status:** ACTIVE — WORKED EXAMPLE STARTED  
**Canonical product:** Sentinel Node  
**Purpose:** Turn supplier selection into an evidence-based industrialization process across DEV → LVP → SVP.

## 1. Core principle

A supplier that can make a good prototype is not automatically a production-capable supplier.

Supplier industrialization asks whether the supplier can repeatedly produce the required configuration, quality, rate, evidence, traceability, and change discipline under representative production conditions.

## 2. Sentinel Node scenario

The Sentinel Node uses a precision molded enclosure with sealing features, threaded inserts, connector interfaces, cosmetic requirements, and dimensional CTQs affecting gasket compression and sensor mounting.

During DEV, Supplier Alpha successfully produces 12 CNC-machined enclosure sets. Engineering is satisfied because:
- dimensions are acceptable;
- fit is good;
- sealing tests pass on the engineering samples;
- communication is fast;
- prototype lead time is short.

The team therefore assumes Alpha is the natural production supplier.

At LVP, however, the design moves to injection molding and the required output becomes 600 accepted enclosures/month. New evidence is now required.

## 3. What changed when volume changed

The production question is no longer only whether Alpha can make the geometry.

The evidence envelope now includes:
1. production-intent tooling;
2. actual production material and approved resin source;
3. cavity-to-cavity variation;
4. molding process window and control;
5. insert installation process;
6. dimensional CTQs and measurement adequacy;
7. cosmetic defect criteria;
8. sealing-related capability;
9. production rate and yield;
10. packaging/handling damage;
11. traceability;
12. sub-tier control;
13. change notification;
14. recovery/continuity risk.

## 4. Supplier qualification ladder

### Gate S1 — Technical fit
Can the supplier understand and manufacture the design/process at all?

### Gate S2 — Prototype evidence
Can acceptable samples be produced and can technical communication work?

### Gate S3 — Production-intent process evidence
Can parts be made using representative tooling, material, operators, routing, inspection, and sub-tier processes?

### Gate S4 — Production approval evidence
Where applicable, use the required customer/industry approval mechanism such as PPAP, FAI, PPA, customer-specific first-off approval, or an internally defined equivalent.

**Guardrail:** FAI and PPAP are not interchangeable concepts. AIAG describes PPAP around demonstrating that engineering requirements can be consistently met during an actual production run at production rates. Industry-specific approval requirements must be identified explicitly rather than generalized.

### Gate S5 — Rate / capacity evidence
Can the supplier meet required accepted output after yield, downtime, changeover, inspection, and rework effects?

### Gate S6 — Ongoing control
Can the supplier maintain configuration, process control, traceability, calibration, training, maintenance, nonconformance response, and approved sub-tier controls?

### Gate S7 — Change discipline
Will changes to material, source, tooling, process, location, equipment, software, sub-tier, or inspection be assessed and communicated according to applicable requirements before implementation?

### Gate S8 — Sustained supplier performance
Are quality, delivery, responsiveness, escapes, corrective action, capacity, and change performance sustained over time?

## 5. The prototype-success trap

The Sentinel Node team scored Alpha highly based on 12 CNC prototypes. That evidence legitimately supports prototype machining performance. It does **not** automatically support:
- injection-molding capability;
- production-rate capability;
- multi-cavity consistency;
- long-term resin control;
- sub-tier insert control;
- sustained yield;
- production traceability.

Canonical lesson:

> Evidence is valid only inside the process/configuration envelope that produced it.

## 6. LVP failure story

Alpha produces a first production-intent lot of 120 molded housings.

Observed results:
- 120 molded;
- 109 accepted at incoming inspection;
- 11 rejected/reworked;
- most defects cluster around gasket-land flatness and insert position;
- cavity 3 contributes disproportionately to dimensional failures;
- several units show cosmetic handling marks after bulk packaging;
- molding records identify machine and lot but do not reliably preserve cavity identity for every part.

Naive conclusion: "Supplier yield is 90.8%."

Better conclusion: the lot exposed multiple industrialization gaps. The observed acceptance result is useful, but it is not yet sufficient to estimate sustained production performance.

## 7. Evidence chain after the failure

The team should connect:

**Requirement/CTQ → supplier process step → failure mode → process control → measurement → lot/cavity genealogy → containment → corrective action → effectiveness evidence**

For the gasket land, for example:
- requirement: sealing geometry/flatness;
- risk: leak or unstable gasket compression;
- suspected process mechanism: cavity/process-condition interaction;
- immediate containment: segregate cavity output where traceable; increase inspection where justified;
- correction: tooling/process investigation;
- evidence: representative rerun with cavity-level identification;
- closure: demonstrated effectiveness under released process conditions.

## 8. Sub-tier and critical/special-process control

Supplier Alpha installs threaded inserts through a sub-tier service provider and sends some tooling work externally.

The purchasing company therefore needs to know not only "Who is Alpha?" but also:
- Which operations are outsourced?
- Which sub-tier performs them?
- Which requirements must flow down?
- Which records/certifications/qualifications are required?
- What changes require notification or approval?

Nadcap provides a strong aerospace example of process-focused oversight: PRI describes accreditation for critical processes such as heat treatment, NDT, chemical processing, welding, printed board assemblies, materials testing, and measurement/inspection, with periodic audits and continued oversight. This is an industry-specific example, not a universal requirement for all Sentinel Node suppliers.

Canonical lesson:

> Supplier control must follow the process risk through the supply chain, not stop at the purchase-order header.

## 9. FAI vs PPAP vs sustained capability

Keep three questions separate:

1. **Did this defined article/configuration conform?** — first-article/initial-sample style evidence may address this depending on industry.
2. **Can the production process consistently meet requirements under representative production conditions?** — PPAP-style production approval addresses this in automotive contexts.
3. **Is the supplier still capable six months later?** — ongoing supplier performance/process controls address this.

Passing one does not logically prove the other two.

## 10. Supplier scorecard — do not collapse everything into one number

Track at least separate dimensions for:
- technical capability;
- quality performance;
- delivery;
- capacity/rate;
- change discipline;
- corrective-action effectiveness;
- sub-tier control;
- traceability/evidence quality;
- continuity/resilience;
- commercial performance.

A weighted total can support prioritization, but critical red conditions must remain visible. A supplier with excellent price and delivery should not average away an uncontrolled critical process.

## 11. SUPPLIER 10 — listener tool

Before declaring a supplier "production ready," ask:

1. **Requirement** — Are CTQs and acceptance criteria clear?
2. **Process** — Is the real production route known?
3. **Representativeness** — Were samples made using production-intent conditions?
4. **Measurement** — Can the supplier reliably measure what matters?
5. **Capability** — What repeatability/stability/rate evidence exists?
6. **Sub-tier** — Which critical operations leave the supplier's direct control?
7. **Traceability** — Can failures be tied back to relevant lots/processes/cavities/materials?
8. **Change** — What changes require notification, assessment, approval, or requalification?
9. **Recovery** — What happens after a quality escape, tool failure, shortage, or capacity loss?
10. **Sustainment** — What evidence will show that capability remains healthy over time?

## 12. DEV / LVP / SVP interpretation

### DEV
Optimize for technical learning and supplier responsiveness. Prototype evidence is legitimate, but label its envelope honestly.

### LVP
Industrialize the supplier: representative process, released requirements, production evidence, traceability, controls, capacity, corrective-action loops, and appropriate approval packages.

### SVP
Manage sustained capability: trends, audits where applicable, changes, sub-tier risk, continuity, cost, quality escapes, and capacity evolution.

## 13. Podcast claims

Safe canonical claims:
- Prototype success does not prove production capability.
- Supplier capability is process- and configuration-dependent.
- Production approval evidence and sustained supplier performance are different questions.
- Sub-tier processes can carry product risk and therefore require appropriate flow-down and oversight.
- Supplier changes can invalidate prior evidence when they alter assumptions that supported qualification.

Avoid universal claims that a specific approval system (PPAP, Nadcap, AS9102, etc.) is mandatory outside its applicable customer/industry/regulatory context.

## 14. Next depth work

- Build a supplier change-notification / requalification decision tree.
- Build a concrete Alpha supplier scorecard with 6 months of synthetic performance data.
- Add dual-source / continuity decision example.
- Package P2.06 into canonical research pack and listener checklist.
