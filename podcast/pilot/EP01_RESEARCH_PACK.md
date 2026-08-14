# Episode 1 Research Pack — The Product Works. Why Can’t We Manufacture It?

status: RESEARCH PACK OPEN
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

## 5. Claim register — draft
| ID | Claim | Class | Priority | Status | Note |
|---|---|---|---|---|---|
| EP01-C01 | A successful prototype does not by itself demonstrate repeatable production capability. | V6 + backbone | P0 | STABLE BACKBONE | Central distinction. |
| EP01-C02 | Verification/validation evidence and production acceptance/process-control evidence answer related but different questions. | V6 + P2.03 | P0 | OPEN | Source/terminology verification required. |
| EP01-C03 | Manufacturing readiness is multidimensional: design/configuration, process, supplier, measurement/test, quality, people/standard work, rate/capacity and economics can mature at different speeds. | V6 | P0 | SYNTHESIS | Avoid presenting as an external standard taxonomy. |
| EP01-C04 | Hidden expert intervention is a form of manufacturing dependency that must become visible before scaling. | V6 | P1 | SYNTHESIS | Narrative principle. |
| EP01-C05 | CTQs should flow from product/process risk and requirements rather than from inspecting every dimension equally. | V6 + P2.03 | P0 | BACKBONE-SUPPORTED | Quality terminology review needed. |
| EP01-C06 | Configuration identity is necessary to relate build/test evidence to the product version that generated it. | V6 + P2.02 | P0 | BACKBONE-SUPPORTED | Cross-link A8. |
| EP01-C07 | A supplier sample that meets drawing requirements is not by itself evidence of sustained supplier/process capability at production conditions. | V6 + P2.04 | P1 | OPEN | Need careful sourcing/application. |
| EP01-C08 | Rate and cost can expose failure modes or constraints invisible in a few engineering builds. | V6 + P2.05/P2.06 | P1 | BACKBONE-SUPPORTED | Quantitative examples later. |
| EP01-C09 | Industrialization should close evidence gaps deliberately rather than copy every prototype method into production. | V6 | P0 | STABLE SYNTHESIS | Episode conclusion. |

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

## 9. Common failure modes
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

## 10. Applicability statement
General hardware industrialization framework. It does not define contractual production-readiness criteria for regulated sectors, nor replace industry-specific APQP/PPAP/FAI/qualification requirements. Those methods can later be mapped onto the evidence dimensions where applicable.

## 11. What this episode must NOT claim
- a working prototype has little value;
- production readiness is one universal TRL/MRL number;
- every startup needs automotive APQP/PPAP;
- every dimension is a CTQ;
- automation is required for scale;
- LVP/SVP are external standard lifecycle labels;
- a fixed unit count proves readiness.

## 12. Research backlog before CLAIM SET STABLE
1. Verify terminology separating product V&V from production acceptance/process evidence.
2. Source authoritative support for configuration-to-evidence traceability.
3. Source supplier/process-capability distinction without overgeneralizing PPAP beyond applicability.
4. Build one quantitative mini-example showing how rate/yield changes cost per good unit.
5. Cross-check against P2.01–P2.10 and Global Invariants.
6. Technical review: NPI + quality + manufacturing + systems.

## 13. Pilot-test objective
Episode 1 tests whether the packaging contract can synthesize many backbone domains into one accessible entry episode without becoming a checklist dump.

PASS signal:
A team with a working prototype should be able to identify its five highest-risk missing evidence classes and define the next build around closing them.

## 14. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Cross-domain burden: HIGH
Standards burden: MEDIUM
Quantitative burden: MEDIUM
Backbone risk: MEDIUM — synthesis discipline required
Source verification: OPEN

Next status target:
`RESEARCH PACK OPEN → CLAIM SET STABLE`
