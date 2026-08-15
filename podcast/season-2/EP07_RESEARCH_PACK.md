# Episode 7 Research Pack — DFA, Assembly Architecture and Mistake-Proofing

status: CLAIM SET STABLE
season: Season 2 — Turn the Prototype into a Product
primary_audience: Audience A + Audience B
secondary_audience: mechanical, electronics, NPI, manufacturing, quality, operations
lifecycle: DEV → LVP → SVP
entry_point: DESIGNING FOR ASSEMBLY
technical_depth: practitioner

## 1. Episode promise
Teach teams to design assemblies so correct execution is easier, ambiguity is reduced, defects are prevented or exposed early, and assembly evidence can scale beyond the inventor who built the prototype.

Canonical listener question:
> If the product can be assembled by the engineer who designed it, what must change before ordinary production can assemble it correctly and repeatedly?

## 2. Navigation card
**You are here:** DFM → assembly architecture → work/test/process control.
**Best for:** teams preparing first controlled assembly, redesigning high-rework products, or transferring builds to technicians/suppliers.
**Prerequisite:** Episode 6 recommended, not mandatory.
**You will leave with:** Assembly Risk Walk + Mistake-Proofing Ladder.
**Next:** detailed joining/assembly/process-control episodes.

## 3. Core thesis
DFA is not simply minimizing part count or assembly seconds. Good assembly design reduces unnecessary operations and ambiguity while making orientation, access, sequencing, fastening, connection, inspection, test, rework and configuration control compatible with the intended production system.

Mistake-proofing should preferentially prevent an error or expose it near its source when that is technically and economically appropriate, rather than depending only on downstream inspection or operator memory.

## 4. Stable claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP07-C01 | Assembly design is a product-process interaction, not merely a drawing/BOM property. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP07-C02 | Prototype assembly by expert engineers can hide ambiguity, tacit knowledge, access difficulty and recovery burden. | P0 | BACKBONE-STABLE |
| EP07-C03 | Part-count reduction can help but is not a universal objective if integration increases risk, service burden, yield loss or verification difficulty. | P0 | SYNTHESIS/BACKBONE STABLE |
| EP07-C04 | Where feasible and justified, preventing an error or exposing it near its source reduces dependence on downstream-only detection. | P0 | BACKBONE/SYNTHESIS STABLE; external attribution requires source verification |
| EP07-C05 | Orientation, connector/keying, datum/fixture strategy, access and sequence can be designed to reduce assembly ambiguity. | P1 | BACKBONE-SUPPORTED / STABLE |
| EP07-C06 | Fastening/joining strategy should consider repeatability, controlled input, inspection, rework and service where applicable. | P0 | BACKBONE-SUPPORTED / STABLE |
| EP07-C07 | Work instructions alone cannot indefinitely compensate for architecture that makes consequential errors easy and invisible. | P1 | SYNTHESIS STABLE |
| EP07-C08 | Mistake-proofing effectiveness must be evidenced in the relevant process/configuration envelope and controlled against bypass/failure/change. | P0 | BACKBONE-STABLE |

Publication guardrail: any formal poka-yoke hierarchy, human-factors requirement, torque/joint rule or sector-specific assembly control requires verified source/applicability before attribution.

## 5. Listener tool — Assembly Risk Walk
For each operation capture:
`Operation → orientation → access → sequence → identification → controlled force/torque/energy → fixture/datum → hidden defect → verification → rework/recovery → human dependency → design opportunity`.

Flag reversible/symmetric interfaces, crossed or partially seated connectors, inaccessible fasteners, hidden interfaces, feel-based alignment, uncontrolled joining amount/cure, compensating adjustment, and defects that become inaccessible later.

## 6. Mistake-Proofing Ladder
Internal decision framework, not a claimed external standard:
1. **Eliminate** the unnecessary error opportunity.
2. **Prevent** the wrong state through geometry/keying/interlock/hard constraint.
3. **Guide/constrain** execution through fixture, datum, sequence or controlled tool/recipe.
4. **Detect at source** before the error propagates.
5. **Contain** known nonconforming output.
6. **Verify downstream** where earlier control is impractical or insufficient.
7. **Instruction/memory only** — generally fragile when an easy consequential invisible error remains possible.

For every control ask: can it be bypassed, can it fail silently, how is effectiveness verified, and what happens after change/maintenance?

## 7. Worked examples
### Electro-mechanical connector/cover
Expert builder knows cable route and full connector seating. Production risk arises from visually similar orientation, partial seating and hidden cable pinch after closure. Candidate controls include keying, retention indication, routing geometry, sequence constraint, source electrical check and serial-linked result.

### Mechanical fastener/interface
Awkward fastener access causes tool angle variation and feel-based alignment. Candidate responses include architecture/access change, positive datum, controlled tool strategy and source verification. Numerical torque/joint acceptance remains process-specific and source-controlled.

## 8. DEV/LVP/SVP lens
**DEV:** identify where expert knowledge compensates for product/assembly ambiguity.
**LVP:** capture assembly failure modes, rework, sequence and operator variation; introduce targeted design/fixture/source controls.
**SVP:** demonstrate controls, work method, tooling, verification, traceability and recovery at intended population/rate.

## 9. Human factors boundary
Do not reduce assembly quality to “operator error.” Distinguish design-induced ambiguity, tooling/process limitations, work-instruction/training gaps, environment/ergonomics and abnormal execution. Detailed human-factors and occupational-safety requirements need separate applicability/source treatment.

## 10. Boundary discipline
Episode 6 owns DFM/process-design fit. Episode 7 owns assembly architecture and mistake prevention. Joining physics belong to process episodes. PFMEA/control plans own formal risk-to-control deployment. Test/metrology episodes own measurement-system depth.

## 11. Applicability statement
The Assembly Risk Walk and Mistake-Proofing Ladder are internal podcast frameworks. Actual controls depend on product risk, process, service strategy, production volume, automation, operator environment and applicable standards/customer/regulatory requirements.

## 12. What this episode must NOT claim
- fewer parts always means better DFA;
- every human error should be physically prevented;
- poka-yoke removes the need for validation/training;
- downstream inspection is always useless;
- torque alone proves joint integrity;
- expert prototype assembly proves production readiness.

## 13. Evidence backlog after claim stabilization
1. Build authoritative DFA/mistake-proofing source map.
2. Verify terminology before attributing formal methods to Lean/Toyota/standards.
3. Add process-specific sources only where examples need normative detail.
4. Technical review: design + manufacturing/NPI + quality/operations; human factors when needed.

## 14. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: MEDIUM-HIGH
Quantitative burden: LOW-MEDIUM
Backbone risk: LOW
Claim set: STABLE
Source verification: CONTROLLED BACKLOG

Next status target: `CLAIM SET STABLE → EVIDENCE VERIFIED`
