# Episode 6 Research Pack — DFM: Design for the Process You Intend to Control

status: CLAIM SET STABLE
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: mechanical, electronics, manufacturing, NPI, quality, suppliers
lifecycle: DEV → LVP → SVP
entry_point: DESIGNING FOR PRODUCTION
technical_depth: practitioner

## 1. Episode promise
Turn DFM from a late supplier checklist into an engineering method for aligning product definition with the manufacturing process, its variation, measurement and intended production stage.

Canonical listener question:
> What should I change in the design today so the intended process can make good parts repeatedly tomorrow?

## 2. Navigation card
**You are here:** readiness/gates → design for production → assembly/process-specific design.
**Best for:** teams moving from prototype methods to controlled production routes.
**Prerequisite:** Episodes 2–5 helpful, not mandatory.
**You will leave with:** DFM Process-Design Contract + DFM Review Questions.
**Next:** Episode 7 DFA/mistake prevention → process-family deep dives.

## 3. Core thesis
DFM is the deliberate matching of product definition to an intended manufacturing process and its real variation, inspection, tooling, supplier and economic envelope. A feature can be geometrically manufacturable yet still be a poor production decision if it creates unstable tolerances, difficult inspection, fragile sourcing, low yield or excessive cost per accepted good unit.

## 4. Stable claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP06-C01 | DFM decisions are process-specific; generic rules cannot replace knowledge of the intended process/material/equipment envelope. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP06-C02 | Tolerances should originate from product function/verification need and be reconciled with achievable process and measurement capability. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP06-C03 | Prototype processes can hide production constraints or create constraints absent from the intended production route. | P0 | BACKBONE-STABLE / A4 |
| EP06-C04 | Manufacturing economics should consider accepted good output, including material yield, scrap/rework, inspection, tooling and cycle effects where material. | P0 | BACKBONE-STABLE |
| EP06-C05 | DFM input is most valuable while architecture, geometry, material and process choices remain economically changeable. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP06-C06 | Supplier DFM feedback is evidence/input, not automatic transfer of product-design authority or applicability judgment. | P1 | SYNTHESIS/BACKBONE STABLE |
| EP06-C07 | Inspection/test accessibility and measurement feasibility are design concerns because they affect whether CTQs can be controlled and verified in production. | P1 | BACKBONE-SUPPORTED / STABLE |
| EP06-C08 | DFM changes must preserve requirements and configuration/change control; manufacturability improvement cannot silently alter the product claim. | P0 | BACKBONE-STABLE |

Publication guardrail: process-specific numerical rules remain unverified until tied to the applicable material/process/equipment/standard/source.

## 5. DFM Process-Design Contract
For each important part/assembly capture:
`Function → intended stage → process family → material/state → critical geometry → CTQ/tolerance rationale → process capability assumption → measurement → tooling/access → supplier/equipment envelope → yield/rework risk → economics → bridge-to-SVP change → evidence`.

## 6. DFM Review Questions
1. Which features are functionally critical versus legacy/default tolerances?
2. What process is assumed at DEV, LVP and SVP?
3. Which prototype evidence will not transfer?
4. What variation/failure mechanisms are plausible in the intended process?
5. Can CTQs be measured reliably without heroic inspection?
6. Does the design unnecessarily require rare equipment/material/source?
7. What happens to accepted yield and rework if the process drifts?
8. Which feature dominates tooling, cycle or inspection economics?
9. Can the design widen the process window without harming function?
10. What evidence is required before locking the design/process pair?

## 7. Worked example — machined prototype to molded enclosure
A CNC enclosure may support geometry/interface evidence while saying little about the future molded distribution. Moving to injection molding changes relevant questions: wall/rib strategy, draft/ejection, flow/gate/weld-line sensitivity, shrink/warpage, inserts/fasteners, cosmetic surface, tooling-change economics and datum/inspection strategy.

The episode must not turn those examples into universal molding design numbers; process-specific rules belong to verified sources and later process episodes.

## 8. DEV/LVP/SVP lens
**DEV:** optimize learning while making provisional process assumptions visible.
**LVP:** use bridge processes intentionally and define expiration triggers.
**SVP:** align design with a demonstrated process/supplier/measurement/economic envelope under controlled change.

## 9. Boundary discipline
Episode 6 owns cross-process DFM logic. Episode 7 owns assembly/DFA and mistake prevention. GD&T/metrology episodes own specification/measurement depth. Process-family episodes own numerical design rules and detailed process physics.

## 10. Standards/source boundary
Cross-process principles may be supported by authoritative engineering/manufacturing references. Any numerical tolerance, geometry, material or process rule must be sourced to the relevant process/material/equipment/standard and applicability. GD&T/GPS/drawing standards must be edition-verified before normative use.

## 11. Applicability statement
The DFM Process-Design Contract is an internal framework. Actual design rules depend on product requirements, material, process, equipment, supplier capability, production stage and applicable standards/customer requirements.

## 12. What this episode must NOT claim
- DFM is synonymous with cost reduction;
- one geometric rule set applies to all processes;
- supplier preference equals engineering requirement;
- tighter tolerance automatically means higher quality;
- prototype-process success proves production-process capability;
- manufacturability permits uncontrolled product-definition change.

## 13. Evidence backlog after claim stabilization
1. Build authoritative cross-process DFM source map.
2. Attach verified process-specific examples only where they improve teaching.
3. Verify any GD&T/GPS/material/process standard editions before publication.
4. Technical review: design + manufacturing/process + quality/metrology.

## 14. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: MEDIUM-HIGH
Quantitative burden: MEDIUM in examples
Backbone risk: LOW
Claim set: STABLE
Source verification: CONTROLLED BACKLOG

Next status target: `CLAIM SET STABLE → EVIDENCE VERIFIED`
