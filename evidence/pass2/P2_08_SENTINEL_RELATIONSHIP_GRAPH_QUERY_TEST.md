# P2.08 — Sentinel Node Relationship Graph + Genealogy Query Test

Status: ACTIVE — IMPLEMENTATION VALIDATION
Provenance: [GNR] implementation synthesis; conceptual alignment checked against ISA-95 and NIST digital-thread principles. Exact standard object/attribute mappings require source-level verification before Podcast Ready.

## Purpose

Test whether the Manufacturing Atlas can answer real manufacturing questions from linked records rather than from narrative documents or tribal knowledge.

The test object is Sentinel Node SN-0284.

The architecture passes only if a reviewer can reconstruct what SN-0284 was supposed to be, what it actually became, what happened during manufacture, why it was accepted, which evidence supports that decision, and which populations become suspect after a change.

## 1. Minimal object model

### Definition objects
- Requirement
- CTQ Definition
- Product Type
- Product Revision
- Part Definition
- BOM Revision
- Process Plan Revision
- Operation Definition
- Work Instruction Revision
- Test Definition/Revision
- Firmware Definition/Revision
- Tooling/Fixture Definition/Revision
- Recipe Definition/Revision
- Supplier Part Approval / approved source definition

### Execution / instance objects
- Serial Unit
- Work Order
- Operation Execution
- Material Lot
- Component Instance where serialized
- Equipment Asset
- Fixture Instance
- Operator/Personnel Instance
- Measurement Result
- Test Execution
- NCR
- Rework Execution
- Deviation/Waiver
- Release/Disposition Decision
- Change Instance

### Evidence / knowledge objects
- Claim
- Evidence Item
- Applicability Statement
- Decision Instance

## 2. Relationship graph — SN-0284

```text
REQ-CONN-001
  └─defines→ CTQ-SEAT-DEPTH-001 [4.80–5.20 mm]

PRODUCT-SN
  └─revision→ SN-REV-C
      ├─uses→ BOM-C
      ├─uses→ PROCESS-PLAN-C
      └─compatible-with→ FW-1.9.0

BOM-C
  └─requires→ CONN-PN-104
       └─approved-source→ SUPPLIER-ALPHA

WO-240812-07
  └─builds→ SN-0284

SN-0284
  ├─as-planned→ SN-REV-C
  ├─consumed→ CONN-PN-104 / LOT-CA-771
  ├─executed→ OP30-EXE-0284-A
  ├─executed→ OP30-RWK-0284-B
  ├─executed→ OP40-CAL-0284
  ├─executed→ OP50-FT-0284
  └─released-by→ DISP-0284-01

OP30-EXE-0284-A
  ├─operation-definition→ OP30-CONNECTOR-INSERT
  ├─fixture→ FIX-INS-07 / REV-B
  ├─recipe→ RCP-INS-3.2
  ├─operator→ OPERATOR-17
  ├─produced→ MEAS-0284-001 [4.76 mm / FAIL]
  └─triggered→ NCR-0284-001

NCR-0284-001
  ├─references→ MEAS-0284-001
  ├─disposition→ REWORK-AUTH-0284
  └─requires→ OP30-RWK-0284-B

OP30-RWK-0284-B
  ├─removed→ CONN-PN-104 / LOT-CA-771
  ├─consumed→ CONN-PN-104 / LOT-CA-779
  ├─fixture→ FIX-INS-07 / REV-B
  ├─recipe→ RCP-INS-3.2
  └─produced→ MEAS-0284-002 [5.02 mm / PASS]

OP40-CAL-0284
  ├─loads→ FW-1.9.0
  ├─uses→ CAL-RECIPE-2.4
  └─result→ CAL-PASS-0284

OP50-FT-0284
  ├─test-definition→ FT-SN-REV-6
  └─result→ FT-PASS-0284

DISP-0284-01
  ├─considers→ NCR-0284-001
  ├─considers→ MEAS-0284-002
  ├─considers→ CAL-PASS-0284
  ├─considers→ FT-PASS-0284
  └─decision→ ACCEPT
```

## 3. As-designed vs as-built vs as-tested

### As-designed
SN Rev C + BOM C + process plan C + approved firmware/configuration.

### As-built
SN-0284 contains the replacement connector from LOT-CA-779 after approved rework, not the originally issued LOT-CA-771 connector.

### As-tested
SN-0284 was calibrated with FW 1.9.0 / calibration recipe 2.4 and passed functional test definition FT-SN-REV-6.

These three views must remain distinguishable.

## 4. Query tests

### Q1 — What connector is actually inside SN-0284?

Expected answer:
CONN-PN-104 from LOT-CA-779.

Required path:
Serial → rework execution → consumed replacement material lot.

Failure condition:
System returns LOT-CA-771 merely because it was originally issued to the work order.

### Q2 — Did SN-0284 ever fail a CTQ?

Expected answer:
Yes. Initial connector seating depth = 4.76 mm, below LSL 4.80 mm.

Required path:
Serial → operation execution → measurement → CTQ/specification.

Failure condition:
Only final PASS value remains visible.

### Q3 — Why was the unit released after a failure?

Expected answer:
Approved NCR/rework path replaced the connector; post-rework seating depth was 5.02 mm; calibration and final functional test passed; release decision considered those records.

Required path:
NCR → disposition → rework → measurement/test evidence → release decision.

### Q4 — Which firmware was actually tested on the unit?

Expected answer:
FW 1.9.0.

Required path:
Serial → calibration/test execution → loaded firmware/configuration.

Failure condition:
System answers with “latest firmware” or engineering baseline rather than execution evidence.

### Q5 — Which units could be affected if LOT-CA-779 is later found suspect?

Expected method:
Reverse genealogy query from material lot → consumption events → serial units → downstream tests/releases/shipment status.

The query must not rely on searching free-text work instructions.

### Q6 — Which units were produced using fixture Rev B and recipe 3.2?

Expected method:
Fixture/recipe configuration → operation executions → serial units.

This supports containment after tooling/recipe discoveries.

### Q7 — A connector supplier changes plating. Which previous evidence remains applicable?

Expected method:
Change → affected part/process characteristics → affected claims → Applicability Statements → evidence dependencies.

Geometry evidence may remain applicable while insertion-force, electrical-contact, corrosion or reliability evidence may require targeted review/reverification.

### Q8 — Was SN-0284 built exactly to the nominal released route?

Expected answer:
No. It contains an approved exception/rework history. It can still be conforming/released, but “nominal route” and “accepted as-built history” are not the same claim.

## 5. Mock relational schema

This is implementation-oriented synthesis, not a mandated ISA-95 database schema.

```text
product_revision(id, product_id, revision, effective_from, effective_to)
bom_revision(id, product_revision_id, revision)
bom_item(id, bom_revision_id, part_definition_id, qty, approved_source_rule_id)
process_plan_revision(id, product_revision_id, revision)
operation_definition(id, process_plan_revision_id, sequence, operation_type)
serial_unit(id, product_id, planned_revision_id, work_order_id, status)
material_lot(id, part_definition_id, supplier_id, supplier_lot, received_status)
operation_execution(id, serial_unit_id, operation_definition_id, start_ts, end_ts, result)
operation_material(operation_execution_id, material_lot_id, action, qty)
operation_resource(operation_execution_id, resource_type, resource_id, resource_revision, role)
measurement_result(id, operation_execution_id, ctq_id, value, unit, result, method_revision)
test_execution(id, serial_unit_id, test_definition_revision_id, firmware_revision_id, result)
ncr(id, serial_unit_id, originating_record_type, originating_record_id, status)
rework_execution(id, ncr_id, operation_execution_id, authorization_revision)
release_decision(id, serial_unit_id, decision, authority, timestamp)
release_evidence(release_decision_id, evidence_record_type, evidence_record_id)
change_instance(id, change_type, description, approval_status, effectivity_rule)
claim(id, claim_text, status)
evidence_item(id, source_type, source_record_id, verification_status)
claim_evidence(claim_id, evidence_item_id)
applicability_statement(id, claim_id, envelope_definition, exclusions, validity_status)
```

## 6. Integrity rules

1. Released definition is immutable; new definition requires revision/version identity.
2. Execution records are append-only from the manufacturing-history perspective; correction is itself traceable.
3. Rework does not overwrite the failed operation.
4. Material replacement changes as-built genealogy.
5. Firmware/recipe/tooling identities are execution attributes where they can affect outcome.
6. Release decisions link to the evidence considered at decision time.
7. Claims cannot inherit evidence outside its applicability envelope without review.
8. Effectivity is explicit; approval timestamp alone is not sufficient.
9. Reverse genealogy must be possible for critical material/process/resource relationships.
10. Identity is semantic and persistent; a PLC/MES tag name alone is not the enterprise identity.

## 7. ISA-95 alignment note

ISA-95 provides models/terminology for enterprise-control integration and manufacturing operations management. Its information models include material, equipment/physical assets, personnel and manufacturing operations information. This implementation uses those concepts as an interoperability backbone, but does not claim that ISA-95 mandates this exact database schema or the complete PLM/QMS/claim-evidence model.

## 8. NIST digital-thread alignment note

The model supports reuse and traceability of information across engineering, manufacturing and quality, while preserving the version/configuration context needed to interpret the records. The implementation deliberately links inspection/measurement results back to product/process definition rather than leaving them as isolated result files.

## 9. Architecture validation scorecard

A Data Hub subdomain can move from ARCHITECTURE DRAFTED to ARCHITECTURE VALIDATED AGAINST IMPLEMENTATION EXAMPLE only when the Sentinel graph demonstrates the relevant behavior.

Validation checks:
- identity resolution: PASS
- type vs instance: PASS
- definition vs execution: PASS
- temporal/effectivity distinction: PASS conceptually
- material genealogy: PASS
- equipment/tooling/recipe context: PASS
- measurement/test linkage: PASS
- NCR/rework history preservation: PASS
- release-decision evidence linkage: PASS
- claim/evidence/applicability linkage: PASS conceptually
- reverse trace query: PASS at schema/graph level
- real software implementation: NOT YET VALIDATED

Therefore:

> Architecture validated against implementation example ≠ implementation validated in production software.

## 10. Listener tool — RECONSTRUCT 8

Pick any shipped serial number and ask:
1. What was it supposed to be?
2. What materials/components actually went into it?
3. Which process/resource/configuration actually touched it?
4. What did it measure/test at each critical step?
5. What exceptions/rework occurred?
6. Why was it accepted/released?
7. Which evidence/claims depend on its configuration/process envelope?
8. Can we find every other unit affected by a suspect lot/process/tool/change?

If the answer requires asking the engineer who remembers, the digital thread is incomplete.

## 11. P2.08 remaining work

Before NEAR PODCAST READY:
1. map this implementation back to the existing 12 Manufacturing Data Hub files and mark which architectural sections are now implementation-example validated;
2. create one canonical Atlas pack with system-of-record boundaries and minimum viable implementation guidance for startups/LVP teams;
3. primary-source verification for ISA-95/IEC 62264 and any other standards claims used in the episode;
4. technical review and episode source-note packaging.
