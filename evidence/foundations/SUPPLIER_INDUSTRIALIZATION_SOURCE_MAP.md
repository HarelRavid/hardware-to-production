# Supplier Industrialization / Qualification / Change Control — Evidence Source Map

status: IN PROGRESS — SELECTION/CAPABILITY/RESILIENCE BACKBONE CAPTURED
campaign: A6
maps_to: MASTER_WBS Section 7 and 5.8; PODCAST_MAP Episodes 30, 37–40
provenance: primary-source-first

## Purpose
Build the evidence backbone for selecting, qualifying and scaling suppliers based on demonstrated manufacturing capability, quality systems, process control, capacity, change discipline and resilience rather than quotation quality or presentation quality alone.

## Source backbone captured
### NIST MEP — Supply Chain Management
Primary use:
- supplier evaluation and selection;
- supplier segmentation by criticality;
- total cost of ownership;
- supplier development;
- supplier metrics/scorecards;
- process improvement and quality-system development across supply-chain tiers.
Editorial implication: supplier management is an ongoing operating system, not a one-time sourcing event.

### NIST MEP — Supplier Selection guidance
Primary use:
- capacity dynamics;
- staff/equipment flexibility;
- maintenance of key equipment/tooling;
- logistics;
- quality-system evidence;
- TCO versus unit-price thinking.
Applicability note: example capacity percentages in advisory articles are heuristics, not universal qualification limits.

### NIST MEP — Supplier Scouting
Primary use:
- distinction between nominal supplier identity and demonstrated technical/process capability/capacity;
- matching technical requirements, tolerances, materials, certifications and business requirements to candidate suppliers.
Editorial implication: possessing equipment is weaker evidence than having the capability, capacity and proficiency to make the defined product.

### NIST MEP — Supply-chain mapping and resilience
Primary use:
- Tier 2/Tier 3 visibility;
- geographic concentration;
- critical material/part dependency;
- supplier risk indices;
- common dependencies and bottlenecks.
Editorial implication: two Tier-1 suppliers can still share common-mode risk through the same sub-tier, geography, material source, logistics path or special process.

### NIST MEP case — Abtech supplier scale-up (2026)
Observed sequence:
- supplier identified for production need;
- supplier quality process audited;
- supplier trained on testing protocols;
- supplier integrated into QA process;
- capacity increased materially afterward.
Use: commercial illustration that finding a supplier and industrializing/qualifying that supplier are separate steps.
Do not generalize the reported improvement magnitude.

### AIAG / Automotive Core Tools and PPAP
Target use:
- supplier production-part approval;
- production-run evidence;
- process/change submissions;
- process capability/control evidence.
Applicability: customer/automotive-specific submission rules must not be generalized as universal law.
Status: primary-source depth still required in Pass 2.

### AS9102 / aerospace First Article Inspection family
Target use:
- first-article verification and configuration evidence;
- distinction between first-article conformance and ongoing process capability.
Applicability: aerospace-specific requirements and revision control.
Status: primary-source depth still required.

### ISO 9001 / supplier-control requirements
Target use:
- control of externally provided processes/products/services;
- supplier evaluation/monitoring boundaries;
- change and nonconformance governance.
Applicability: management-system requirements do not replace technical process qualification.
Status: clause-level extraction reserved for Pass 2.

### Special-process accreditation/qualification families
Target use:
- welding, heat treatment, coatings, NDT and other processes where process execution/control is central to product assurance.
Status: process-specific mapping reserved for later evidence campaigns.

## Supplier lifecycle model
Candidate discovery -> screening -> technical/process evaluation -> sample/FAI evidence where appropriate -> production-process qualification/approval -> capacity/rate evidence -> controlled launch -> ongoing performance monitoring -> change/requalification -> resilience/recovery.

The exact formal gates vary by sector/customer/risk. The lifecycle is a decision framework, not a universal standard sequence.

## Decision dimensions
- product/process technical fit
- material/process competence
- quality-system maturity
- process capability and measurement capability
- special-process control
- tooling/equipment adequacy
- capacity and scalability
- maintenance/readiness
- operator qualification
- traceability/genealogy
- sub-tier control
- change notification/approval
- engineering responsiveness
- lead time/logistics
- business continuity/resilience
- cybersecurity/data exchange where material
- cost/TCO

## Claim register
### C-SUP-001 — Lowest supplier quote is not sufficient evidence of lowest total manufacturing cost or risk
status: SUPPORTED DIRECTION
Evidence: NIST MEP supplier-selection/TCO guidance.
Boundary: TCO model must expose assumptions rather than replace commercial negotiation with one synthetic score.

### C-SUP-002 — Supplier selection and supplier qualification are different decisions
status: SUPPORTED SYNTHESIS
Evidence: NIST supplier scouting identifies capability/capacity candidates; Abtech case subsequently audited quality and trained/integrated the chosen supplier before full use.
Meaning: selection chooses whom to evaluate/use; qualification demonstrates suitability for a defined product/process/configuration/rate and evidence requirement.

### C-SUP-003 — A conforming first article does not by itself prove serial process capability
status: HIGH PRIORITY / STRONG ENGINEERING DIRECTION
Evidence target: AS9102/PPAP and repeated-production evidence.
Reason: one article primarily demonstrates a configuration/output result; serial capability requires evidence about repeated production process behavior and controls.
Do not promote to verified universal claim until primary FAI/PPAP comparison is captured.

### C-SUP-004 — Supplier capability includes process, measurement, tooling, people and capacity, not only nominal machine list
status: SUPPORTED
Evidence: NIST MEP supplier-selection/scouting guidance explicitly evaluates technical/process capability, capacity, proficiency, staffing flexibility, quality systems and equipment/tool maintenance.

### C-SUP-005 — Supplier/sub-tier/process changes can invalidate prior qualification evidence
status: STRONG SYNTHESIS / CHANGE EVIDENCE OPEN
Need: primary change-notification/PPAP/customer requirements and cases.

### C-SUP-006 — Dual sourcing is not automatically resilience if sources share hidden common dependencies
status: SUPPORTED DIRECTION
Evidence: NIST supply-chain mapping explicitly calls for Tier 2/Tier 3 visibility, geographic concentration, critical-material origins and risk mapping.
Boundary: dual sourcing still can reduce risk; the claim is that supplier count alone is insufficient evidence of independence.

### C-SUP-007 — Supplier performance metrics should include more than on-time delivery and incoming rejects
status: SUPPORTED DIRECTION
Evidence: NIST MEP describes supplier metrics/scorecards for performance and supplier development; mapping guidance includes responsiveness/risk factors.
Potential dimensions: escapes, responsiveness, process changes, CAPA effectiveness, capacity, lead-time stability, quality-at-source and resilience.

### C-SUP-008 — Capacity is a qualification variable, not merely a procurement promise
status: SUPPORTED
Evidence: NIST MEP supplier selection/scouting repeatedly treats capability and capacity as separate evaluation dimensions.
Editorial question: Can the supplier make it? Can they make enough of it, repeatedly, when we need it?

### C-SUP-009 — Supplier criticality should determine depth of qualification and monitoring
status: SUPPORTED DIRECTION
Evidence: NIST MEP supply-chain management includes supplier segmentation and differentiated strategy for critical versus lower-risk supply.
Boundary: exact risk classes/gates are organization and sector specific.

## Resilience lens — independence versus redundancy
For a critical part, map at least where material risk justifies it:
Supplier A/B -> production site -> special-process sub-tier -> critical material/source -> tooling dependency -> logistics route -> geography/utilities.

A second supplier improves resilience only to the extent that it removes or reduces relevant failure modes. This avoids the false binary of single-source versus dual-source.

## DEV / LVP / SVP lens
### DEV
Use suppliers for speed/learning but document process, material and configuration assumptions. Avoid accidental sole-source lock-in where future scale is foreseeable.

### LVP
Qualify critical suppliers/processes enough to support repeatable tens/hundreds: controlled drawing/spec revision, material certificates where needed, agreed inspection/test, change notification, traceable lots and capacity assumptions.

### SVP
Formalize supplier approval, production validation, capacity/rate evidence, ongoing performance monitoring, sub-tier/special-process controls, change governance, resilience and recovery plans according to risk/industry/customer requirements.

## Podcast tools emerging
### Supplier qualification ladder
1. Can they quote it?
2. Do they understand the technical requirement?
3. Do they possess the relevant process capability?
4. Can they demonstrate a conforming product/configuration?
5. Can their production system repeat it?
6. Can their measurement/control system detect and react to drift?
7. Can they make it at required rate/capacity?
8. Will changes be controlled and communicated?
9. Can the supply chain survive credible disruptions?

### Supplier evidence packet — risk-scaled concept
Potential contents:
- controlled drawing/spec/BOM revision;
- process flow/routing;
- material/certificate requirements;
- FAI/sample evidence where relevant;
- process/measurement capability evidence where relevant;
- control/inspection/test plan;
- special-process qualification;
- tooling/equipment readiness;
- rate/capacity assumptions;
- traceability requirements;
- sub-tier disclosure/control where critical;
- change-notification requirements;
- contingency/recovery information.
Not every item applies to every supplier.

## Myths to challenge
1. Two quotes = two qualified suppliers. — FALSE.
2. They own the right machine, therefore they can make the part. — FALSE/INCOMPLETE.
3. A good first article proves serial capability. — INCOMPLETE; primary comparison still needed.
4. Dual source means resilient. — FALSE/INCOMPLETE.
5. Supplier qualification ends after approval. — FALSE; ongoing monitoring/change control matters.
6. Cheapest piece price is cheapest supply. — FALSE/INCOMPLETE; evaluate TCO/risk.

## Remaining breadth gaps
1. primary FAI versus PPAP versus ongoing capability boundary;
2. supplier-change notification/approval evidence;
3. special-process/sub-tier control principles;
4. supplier capacity/run-at-rate primary evidence linkage;
5. stronger industrial resilience/common-mode case;
6. supplier scorecard primary/industry examples;
7. myths/case studies for Episodes 30, 37–40.

## Pass-2 targets
- worked supplier capability audit/checklist;
- FAI vs PPAP vs capability comparison;
- supplier change/effectivity case;
- sub-tier/special-process escape case;
- supplier capacity/run-at-rate example;
- dual-source hidden-common-mode example;
- supplier TCO comparison.

## Readiness
Source map: ACTIVE
Critical claims identified: YES
Primary-source backbone: PARTIAL — NIST supplier/capability/resilience captured; FAI/PPAP/change depth open
Applicability conflicts visible: YES
Podcast Ready: NO