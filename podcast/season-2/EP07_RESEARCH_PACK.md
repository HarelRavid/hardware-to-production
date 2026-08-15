# Episode 7 Research Pack — DFA, Assembly Architecture and Mistake-Proofing

status: RESEARCH PACK OPEN
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

Mistake-proofing should preferentially prevent an error or make it immediately detectable at the source rather than relying only on downstream inspection or operator memory.

## 4. Draft claim register
| ID | Claim | Priority | Status |
|---|---|---|---|
| EP07-C01 | Assembly design should be evaluated as a product-process interaction, not merely as a drawing/BOM property. | P0 | BACKBONE-SUPPORTED |
| EP07-C02 | Prototype assembly by expert engineers can hide ambiguity, tacit knowledge, access difficulty and recovery burden. | P0 | BACKBONE-STABLE |
| EP07-C03 | Part-count reduction can help but is not a universal DFA objective if integration increases risk, service burden, yield loss or verification difficulty. | P0 | SYNTHESIS/BACKBONE |
| EP07-C04 | Error prevention is generally stronger than relying only on detection after the error has propagated, where technically/economically feasible. | P0 | SOURCE + BACKBONE VERIFICATION NEEDED |
| EP07-C05 | Orientation, connector/keying, datum/fixture strategy, access and sequence can be intentionally designed to reduce assembly ambiguity. | P1 | BACKBONE-SUPPORTED |
| EP07-C06 | Fastening/joining strategy must consider repeatability, torque/energy/process control, inspection, rework and service requirements where applicable. | P0 | BACKBONE-SUPPORTED |
| EP07-C07 | Assembly work instructions cannot compensate indefinitely for a product architecture that makes errors easy and invisible. | P1 | SYNTHESIS STABLE |
| EP07-C08 | Mistake-proofing effectiveness should be evidenced in the actual process/configuration envelope, not assumed from the concept alone. | P0 | BACKBONE-STABLE |

## 5. Listener tool — Assembly Risk Walk
Walk the real or simulated build and record each operation:
| Field | Question |
|---|---|
| Operation | What is being assembled/joined/connected? |
| Orientation | Can it be reversed/rotated/mislocated? |
| Access | Can the tool/operator reach correctly? |
| Sequence | Does order matter and can the wrong order trap later work? |
| Identification | Can variants/parts/connectors be confused? |
| Force/torque/energy | What controlled input matters? |
| Fixture/datum | What locates the part and how repeatably? |
| Hidden defect | What error can escape visually? |
| Verification | How/when is correct execution confirmed? |
| Rework/recovery | What happens if it is wrong? |
| Human dependency | What tacit knowledge is required? |
| Design opportunity | Can product/process design remove or expose the risk? |

## 6. Mistake-Proofing Ladder
Use as an internal decision hierarchy, not a claimed external standard:
1. **Eliminate** — remove the unnecessary operation/error opportunity.
2. **Prevent** — geometry/keying/interlock makes the wrong action impossible or strongly constrained.
3. **Guide** — fixtures, datums, sequencing or interfaces make the correct action obvious/easy.
4. **Detect at source** — sensor/test/check immediately identifies incorrect execution before propagation.
5. **Contain** — stop nonconforming output from moving forward.
6. **Downstream inspect** — detect later when earlier control is not feasible.
7. **Instruction/memory only** — weakest default when the system otherwise permits an easy invisible error.

The ladder is contextual: safety, serviceability, cost, process physics and human factors can alter the appropriate solution.

## 7. Worked example — symmetric connector and hidden fastener
Prototype uses two visually similar connectors that can be swapped and a fastener requiring awkward access. The engineer remembers which is which and feels correct engagement by experience.

Production risk: wrong connection passes visual inspection; fastener torque varies with access; rework requires partial disassembly.

Potential controls: differentiated/keyed interface, routing/length constraints, fixture-guided presentation, accessible fastening architecture, torque-controlled tool with result capture, source functional check. The best solution depends on actual product/process constraints.

## 8. DEV/LVP/SVP lens
**DEV:** notice where expert knowledge is compensating for product/assembly ambiguity.
**LVP:** capture assembly failure modes, rework, sequence and operator variation across multiple units; introduce targeted fixtures/guidance/source checks.
**SVP:** demonstrate assembly controls, work method, tooling, verification, traceability and recovery at intended rate/population.

## 9. Human factors boundary
This episode will not reduce assembly quality to “operator error.” Human actions are part of a designed sociotechnical system. We will distinguish design-induced ambiguity, process/tooling limitations, training/work-instruction gaps and true abnormal execution.

Detailed ergonomics, occupational safety and human-factors standards require separate applicability/source treatment.

## 10. Standards/source burden
Potential source families include DFA literature, mistake-proofing/quality references, human factors, fastening/joining standards and process-specific guidance. Numerical torque, joint, connector, ESD, ergonomics or safety rules must remain outside the script until the applicable source/edition/context is verified.

## 11. Applicability statement
Assembly architecture and mistake-proofing depend on product risk, process, service strategy, automation level, operator environment, joining method and applicable safety/quality requirements. The Assembly Risk Walk and Mistake-Proofing Ladder are internal podcast tools.

## 12. What this episode must NOT claim
- fewer parts always means better DFA;
- every human error can or should be physically prevented;
- poka-yoke removes the need for process validation or training;
- downstream inspection is always useless;
- torque alone proves joint integrity;
- an expert prototype assembly proves production assembly readiness.

## 13. Research backlog before CLAIM SET STABLE
1. Verify cross-domain DFA/mistake-proofing source foundation.
2. Cross-check fastening/joining and human-factors boundaries.
3. Add at least one mechanical and one electro-mechanical assembly example.
4. Technical review: design + manufacturing/NPI + quality; human factors where claims require it.

## 14. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: MEDIUM-HIGH
Quantitative burden: LOW-MEDIUM
Backbone risk: LOW
Source verification: OPEN

Next status target: `RESEARCH PACK OPEN → CLAIM SET STABLE`
