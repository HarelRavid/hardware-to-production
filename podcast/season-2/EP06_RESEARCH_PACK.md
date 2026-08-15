# Episode 6 Research Pack — DFM: Design for the Process You Intend to Control

status: RESEARCH PACK OPEN
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: mechanical, electronics, manufacturing, NPI, quality, suppliers
lifecycle: DEV → LVP → SVP
entry_point: DESIGNING FOR PRODUCTION
technical_depth: practitioner

## 1. Episode promise
Turn DFM from a late supplier checklist into an engineering method for aligning product geometry, materials, tolerances and architecture with the manufacturing process, its variation and the intended production stage.

Canonical listener question:
> What should I change in the design today so the intended process can make good parts repeatedly tomorrow?

## 2. Navigation card
**You are here:** readiness/gates → design for production → process-specific design.
**Best for:** teams moving from prototype methods to controlled production routes.
**Prerequisite:** Episodes 2–5 helpful, not mandatory.
**You will leave with:** DFM Process-Design Contract + DFM Review Questions.
**Next:** Episode 7 DFA/mistake prevention → process-family deep dives.

## 3. Core thesis
DFM is not “make the CAD cheaper.” It is the deliberate matching of product definition to the intended manufacturing process and its real capability, variation, inspection, tooling, economics and stage of production.

A feature can be geometrically manufacturable yet still be a poor production decision because it drives unstable tolerances, difficult inspection, special tooling, low yield, fragile suppliers or excessive cost per good unit.

## 4. Draft claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP06-C01 | DFM decisions are process-specific; generic manufacturability rules cannot replace knowledge of the intended process/material/equipment envelope. | P0 | BACKBONE-SUPPORTED |
| EP06-C02 | Tolerance should be driven by function and verification need while remaining compatible with achievable process/measurement capability. | P0 | BACKBONE-SUPPORTED |
| EP06-C03 | Prototype processes can hide production constraints or create constraints that will not exist in the production route. | P0 | BACKBONE-STABLE / A4 |
| EP06-C04 | Manufacturing cost should be considered as cost per accepted good unit, including yield/rework/inspection/tooling effects where material. | P0 | BACKBONE-STABLE |
| EP06-C05 | DFM should begin while architecture/geometry/material choices remain changeable, not only after drawing release. | P0 | BACKBONE-SUPPORTED |
| EP06-C06 | Supplier DFM feedback is valuable evidence but does not transfer product-design authority or eliminate the need to understand applicability. | P1 | SYNTHESIS/BACKBONE |
| EP06-C07 | Inspection/test accessibility and measurement strategy are design concerns, not only quality-department concerns. | P1 | BACKBONE-SUPPORTED |
| EP06-C08 | DFM changes must preserve configuration/change control and product requirements; manufacturability improvement cannot silently change the product claim. | P0 | BACKBONE-STABLE |

## 5. DFM Process-Design Contract
For each important part/assembly capture:
| Dimension | Question |
|---|---|
| Product function | What must the feature/material/interface actually achieve? |
| Intended stage | DEV, bridge/LVP or SVP route? |
| Process family | machining, molding, casting, forming, AM, PCB, joining, coating, etc. |
| Material/state | What material, temper/state/finish matters? |
| Critical geometry | Which features drive function/assembly/process risk? |
| Tolerance/CTQ | Which limits are truly required and why? |
| Process capability assumption | What variation/process window are we assuming? |
| Measurement | Can the characteristic be measured reliably at production rate? |
| Tooling/access | What tooling, fixturing, datum/access constraints exist? |
| Supplier/equipment envelope | What machine/process/source limitations are relevant? |
| Yield/rework risk | What defects or variation modes are likely? |
| Economics | What drives cost per good unit? |
| Bridge-to-SVP change | What must change when volume/process changes? |
| Evidence | What prototype, coupon, trial, capability or supplier evidence supports the choice? |

## 6. DFM Review Questions
1. Which dimensions/features are functionally critical and which are legacy/default tolerances?
2. What process is assumed at DEV, LVP and SVP?
3. Which prototype evidence will not transfer to that process?
4. What are the likely process failure/variation mechanisms?
5. Can CTQs be measured without heroic inspection?
6. Does the design require a rare machine, tool, material or supplier unnecessarily?
7. What happens to yield and rework if the process drifts?
8. Which feature dominates tooling/cycle/inspection cost?
9. Can a design change widen the process window without harming product function?
10. What evidence is needed before locking the design/process pair?

## 7. Worked example — machined prototype to molded enclosure
Prototype enclosure is CNC machined and meets geometry. Proposed SVP route is injection molding.

DFM questions expose differences: wall thickness and ribs; draft/ejection; gate/flow/weld-line sensitivity; shrink/warpage; insert/fastener strategy; cosmetic surface; tooling change cost; datum/inspection strategy.

The CNC prototype proved selected geometry/interface claims. It did not prove moldability or molded-part dimensional distribution.

## 8. DEV/LVP/SVP lens
**DEV:** optimize learning while recording which process assumptions are provisional.
**LVP:** use bridge processes intentionally and define expiration triggers.
**SVP:** align design with a demonstrated process/supplier/measurement/economic envelope and controlled changes.

## 9. Standards and source burden
This episode is a cross-process DFM foundation. Process-specific numerical rules must come from the relevant process standards, material standards, supplier/equipment evidence or authoritative engineering sources. Do not universalize injection-molding, machining, PCB or AM heuristics across process families.

GD&T/GPS, drawing, material and process standards will be cited only where their applicability and editions are verified.

## 10. Applicability statement
The DFM Process-Design Contract is an internal framework. Actual design rules depend on product requirements, material, process, equipment, supplier capability, production stage and applicable standards/customer requirements.

## 11. What this episode must NOT claim
- DFM is synonymous with cost reduction;
- one set of geometric rules applies to all processes;
- supplier preference equals engineering requirement;
- tight tolerances always improve quality;
- a prototype process proves production-process capability;
- manufacturability justifies changing product requirements without control.

## 12. Research backlog before CLAIM SET STABLE
1. Cross-check canonical DFX/process-selection backbone.
2. Build source map for cross-process DFM principles and verified process-specific examples.
3. Confirm boundary with DFA, GD&T/metrology and process-family episodes.
4. Technical review: design + manufacturing/process + quality/metrology.

## 13. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: MEDIUM-HIGH
Quantitative burden: MEDIUM in examples
Backbone risk: LOW
Source verification: OPEN

Next status target: `RESEARCH PACK OPEN → CLAIM SET STABLE`
