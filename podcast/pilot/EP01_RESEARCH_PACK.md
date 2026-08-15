# Episode 1 Research Pack — The Product Works. Why Can’t We Manufacture It?

status: CLAIM SET STABLE
season: Season 2 — From Working Prototype to Manufacturable Product
primary_audience: Audience B — teams with a working prototype entering industrialization
secondary_audience: founders, engineering leads, NPI, manufacturing, quality, supply chain
lifecycle: DEV → LVP TRANSITION
entry_point: PRIMARY ENTRY FOR TEAMS WITH A WORKING PROTOTYPE
technical_depth: foundation-practitioner

## 1. Episode promise
Explain why functional success is only one evidence class, and give a team a concrete method to expose the missing evidence between “it works” and “we can repeatedly build good units.”

Canonical listener question:
> We have a prototype that works. What exactly is still unknown before we can call this a manufacturable product?

## 2. Navigation card
**You are here:** Working Prototype → Industrialization

**Best for:** a team whose integrated prototype demonstrates the core function and now faces BOM release, suppliers, fixtures, quality, test, cost, rate or pilot-build questions.

**Prerequisite:** none mandatory. A4 is recommended if the prototype uses many temporary technologies.

**You will leave with:** Manufacturability Evidence Gap Map + First Industrialization Review agenda.

**Prototype shortcut:** engineering can still hand-tune, manually inspect or use bridge processes while learning.

**Shortcut expires when:** repeatability, acceptance, traceability, supplier transfer, takt/capacity, cost or field risk depends on undocumented expert intervention.

**Next:** Episode 2 evidence ladder / Episode 3 NPI / Episode 6 DFM / Episode 11 process selection according to the gap found.

## 3. Core thesis
A working prototype answers a narrow but important question: can this configuration perform the intended function under the conditions tested?

Manufacturability asks additional questions:
- Can the design be built repeatedly within controlled variation?
- Can requirements be translated into CTQs and acceptance evidence?
- Can the exact configuration be reconstructed?
- Can suppliers and processes reproduce the intended characteristics?
- Can assembly/test be executed without hidden expert knowledge?
- Can defects be detected at the right stage?
- Can the product be built at the required rate and cost?
- Can changes be controlled without losing evidence?

Therefore:
> Functional proof is necessary evidence, but it is not production evidence.

## 4. Audience contract
### DEV takeaway
Do not punish the prototype for being a prototype. Use it to expose the evidence still missing.

### Prototype shortcut
Manual tuning, temporary fixtures, engineering inspection, bridge parts and hand-built units may remain valid learning tools.

### Shortcut expiration
When a customer, operator, supplier, quality decision or production release depends on the result, hidden expert intervention must become a controlled process, specification, test, fixture, training element or explicit risk acceptance.

### LVP change
LVP is where product truth begins to be translated into controlled build/test/supplier/configuration evidence across multiple units.

### SVP evidence
Stable serial production requires evidence that product, process, measurement, supplier, configuration and rate controls collectively sustain acceptable output.

## 5. Claim register — stabilized
| ID | Claim | Class | Priority | Status | Note |
|---|---|---|---|---|---|
| EP01-C01 | A successful prototype does not by itself demonstrate repeatable production capability. | V6 + backbone | P0 | CLAIM STABLE | Central distinction; supported across P2.01/P2.03/P2.04. |
| EP01-C02 | Product verification/validation evidence and production acceptance/process-control evidence answer related but different questions. | V6 + P2.03 | P0 | CLAIM STABLE / source packaging open | Keep terminology application-neutral until episode source pack. |
| EP01-C03 | Manufacturing readiness is multidimensional: design/configuration, process, supplier, measurement/test, quality, people/standard work, rate/capacity and economics can mature at different speeds. | V6 | P0 | CLAIM STABLE | Repository synthesis; do not present as external standard taxonomy. |
| EP01-C04 | Hidden expert intervention is a manufacturing dependency that must become visible before scaling. | V6 | P1 | CLAIM STABLE | Synthesis; convert hero knowledge into controlled method where it affects release/repeatability. |
| EP01-C05 | CTQs should flow from product/process risk and requirements rather than from inspecting every dimension equally. | V6 + P2.03 | P0 | CLAIM STABLE | Exact external terminology remains source-pack work. |
| EP01-C06 | Configuration identity is necessary to relate build/test evidence to the product version that generated it. | V6 + P2.02/P2.08 | P0 | CLAIM STABLE | Global invariant alignment. |
| EP01-C07 | A supplier sample that meets drawing requirements is not by itself evidence of sustained supplier/process capability at representative production conditions. | V6 + P2.06 | P1 | CLAIM STABLE / source packaging open | Avoid universal PPAP claim. |
| EP01-C08 | Rate, yield and rework can materially change cost per accepted unit and expose constraints not visible in a few engineering builds. | V3/V6 + P2.04/P2.05 | P1 | CLAIM STABLE | Numerical mini-example included below. |
| EP01-C09 | Industrialization should close evidence gaps deliberately rather than copy every prototype method into production. | V6 | P0 | CLAIM STABLE | Episode conclusion. |
| EP01-C10 | Production readiness should be treated as a set of evidence-supported claims inside a defined configuration/process envelope, not as a universal binary label. | V6 + Global Invariants | P0 | CLAIM STABLE | Directly aligns P2.01/P2.02/P2.08. |

## 6. Manufacturability Evidence Gap Map — listener tool
For the current product, score each row as `KNOWN / PARTIAL / UNKNOWN / NOT YET APPLICABLE` and record the next evidence action.

| Evidence dimension | Key question | Current state | Next evidence |
|---|---|---|---|
| Product requirements | What must every released unit satisfy? | | |
| Configuration | Which exact HW/FW/BOM/drawing/spec is being built? | | |
| CTQs | Which characteristics materially control function/risk? | | |
| Process route | What sequence/process will make and assemble it? | | |
| Process window | Which parameters/conditions matter? | | |
| Supplier | Can the intended source repeatedly supply the needed output? | | |
| Measurement | Can we measure the important characteristics reliably? | | |
| Production test | What evidence releases a unit/process step? | | |
| Fixtures/tooling | Can work be located/assembled/tested repeatably? | | |
| Work instructions | Can a trained person execute without inventor knowledge? | | |
| Traceability | Can a failed unit be reconstructed by configuration/material/process/test history? | | |
| Yield/rework | What fails, how often, and what is the controlled disposition? | | |
| Rate/capacity | Can the route meet the required volume/takt? | | |
| Cost | What is cost per good part/unit at the intended route? | | |
| Reliability/compliance | Which product claims still need representative evidence? | | |
| Change control | What evidence must be revisited when something changes? | | |

## 7. First Industrialization Review — listener agenda
A 60–90 minute cross-functional review:
1. Show the working prototype and state exactly what it has proven.
2. List prototype shortcuts and expiration triggers.
3. Freeze nothing by default; identify which interfaces/configuration elements now require control.
4. Walk the Manufacturability Evidence Gap Map.
5. Select top five evidence gaps by risk/lead time.
6. Identify long-lead supplier/tooling/compliance actions.
7. Define the next build’s learning objectives.
8. Assign owners and evidence outputs.

The output is not “production ready / not ready.” It is a prioritized evidence-closure plan.

## 8. Sentinel Node example
The Sentinel Node works on a bench and has survived a small engineering test set.

What the team has:
- working sensing/communications concept;
- custom PCB prototype;
- enclosure prototype;
- basic firmware;
- engineering test data.

What may still be missing:
- released configuration/BOM alternates;
- production-intent enclosure process/material evidence;
- connector sealing/assembly controls;
- programming/calibration/test fixture;
- CTQ definition;
- measurement-system evidence;
- supplier/process capability;
- traceability/genealogy;
- cycle-time/capacity model;
- controlled rework/defect disposition;
- representative reliability/compliance evidence.

Episode lesson: the prototype did not fail. It successfully revealed the next class of engineering work.

## 9. Quantitative mini-example — why rate/yield matters
Illustrative only.

Assume a bridge process costs $42 of direct conversion per attempted unit before scrap/rework.

Case A — 95% FPY, negligible rework:
- expected direct conversion cost per first-pass good unit ≈ $42 / 0.95 = $44.21.

Case B — 80% FPY, same nominal conversion cost:
- expected direct conversion cost per first-pass good unit ≈ $42 / 0.80 = $52.50.

Before adding rework labor, delay, extra test or capacity loss, the lower-yield route already appears ~18.8% more expensive per first-pass good unit than Case A.

This example does NOT prove a universal production-cost formula. It illustrates why unit cost, yield and accepted throughput must be evaluated together.

## 10. Cross-package consistency map
Episode 1 must remain consistent with:

- **P2.01** — readiness is evidence-based and multidimensional.
- **P2.02** — definition/configuration/effectivity determine which evidence applies.
- **P2.03** — CTQ/measurement/process-quality evidence cannot be replaced by final inspection alone.
- **P2.04** — sustainable accepted throughput matters more than a short peak build rate.
- **P2.05** — economics must use cost per good output, realistic yield/ramp/support assumptions.
- **P2.06** — supplier approval is inside a demonstrated process/configuration/rate envelope.
- **P2.08** — evidence must remain reconstructable to as-built/as-run truth.

Global-invariant check: PASS at claim-set level.

## 11. Common failure modes
### “Just build 100”
Quantity is increased before the evidence gaps and learning objectives are defined.

### Freeze too early
Prototype choices are treated as released production architecture simply because they work.

### Freeze too late
Every unit remains unique; failures cannot be tied to configuration.

### Inspect quality in
A large final inspection plan is created instead of controlling upstream characteristics and process risk.

### Hero technician manufacturing
One expert can make every unit work through undocumented adjustment.

### Supplier sample illusion
A few excellent samples are mistaken for evidence of repeatability, capacity and change control.

### Factory theater
Fixtures, dashboards and automation are purchased before the product/process evidence model is understood.

## 12. Applicability statement
General hardware industrialization framework. It does not define contractual production-readiness criteria for regulated sectors, nor replace industry-specific APQP/PPAP/FAI/qualification requirements. Those methods can later be mapped onto the evidence dimensions where applicable.

## 13. What this episode must NOT claim
- a working prototype has little value;
- production readiness is one universal TRL/MRL number;
- every startup needs automotive APQP/PPAP;
- every dimension is a CTQ;
- automation is required for scale;
- LVP/SVP are external standard lifecycle labels;
- a fixed unit count proves readiness.

## 14. Remaining work before EVIDENCE VERIFIED
1. Package authoritative support for product V&V versus production acceptance/process evidence.
2. Package authoritative support for configuration-to-evidence traceability.
3. Add supplier/process-capability source support without overgeneralizing PPAP.
4. Independently recheck numerical examples during quantitative gate.
5. Technical review: NPI + quality + manufacturing + systems.

## 15. Pilot-test objective
Episode 1 tests whether the packaging contract can synthesize many backbone domains into one accessible entry episode without becoming a checklist dump.

PASS signal:
A team with a working prototype should be able to identify its five highest-risk missing evidence classes and define the next build around closing them.

## 16. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Cross-domain burden: HIGH
Standards burden: MEDIUM
Quantitative burden: MEDIUM
Backbone risk: CONTROLLED
Source verification: PARTIAL / episode source-pack work remains

Next status target:
`CLAIM SET STABLE → EVIDENCE VERIFIED`
