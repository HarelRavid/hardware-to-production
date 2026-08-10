# Pilot / PVT / Ramp / Yield / Capacity — Evidence Source Map

status: BREADTH COMPLETE
campaign: A5
maps_to: MASTER_WBS Section 5; PODCAST_MAP Episodes 26–31
provenance: primary-source-first

## Purpose
Build the evidence backbone for demonstrating that a production-intent system can repeatedly build conforming product, learn from yield/rework loss, and scale toward required rate without confusing one successful build with proven production capability.

## Source backbone

### NASA — Production Readiness Review / NPR 7123.1
Evidence role:
- PRR asks whether the developer can efficiently produce the required number of systems;
- entrance/success criteria include resolution of production engineering problems/nonconformances, production documentation, process controls, resources and production configuration;
- production readiness therefore concerns the production system and required quantity, not only product function.

### NASA — Quality Assurance / PRR criteria
Evidence role:
- critical process controls and control limits should be identified;
- acceptance/inspection evidence and known manufacturability/supplier/quality risks are part of production-readiness reasoning.

### AIAG — PPAP
Evidence role:
- automotive production-part approval explicitly evaluates whether parts can be produced with consistent quality during an actual production run at production rates;
- useful evidence for run-at-rate/production-representative logic.
Applicability: automotive/customer-specific methods and submissions are not universal requirements.

### NIST MEP — FPY / lead-time case
Evidence role:
- documented improvement from low FPY and extensive rework to much higher FPY materially reduced processing and lead time;
- supports treating yield/rework as flow/capacity variables as well as quality/cost variables.

### NIST — Manufacturing-system throughput and bottleneck research
Evidence role:
- serial/flexible production-system performance depends on throughput, bottlenecks, product mix and finite-buffer/resource interactions;
- bottleneck location can change with product mix;
- supports system-level capacity reasoning rather than averaging local machine utilization.

### NIST MEP — throughput/bottleneck/WIP cases
Evidence role:
- industrial improvement cases use value-stream/bottleneck analysis, WIP management, layout and upstream-quality improvements to increase throughput and reduce lead time;
- case results are illustrative, not universal improvement percentages.

### Lean Enterprise Institute / constraint reasoning
Evidence role:
- constraint/bottleneck is the factor limiting system output toward its goal;
- supports prioritizing the system constraint rather than optimizing every resource independently.
Applicability: management/operations framework; quantitative capacity analysis still requires product/process-specific data.

## Canonical distinctions
- **Takt time** — demand-derived pace required from the production system.
- **Cycle time** — elapsed processing/work-cycle time for a defined operation or unit under stated conditions.
- **Throughput** — accepted output per unit time at the relevant system boundary.
- **Capacity** — sustainable achievable output under explicitly stated resource, uptime, yield, mix and operating assumptions.
- **Lead time** — total elapsed time through the defined system boundary, including waiting/queue where applicable.
- **WIP** — material/product that has entered but not yet exited the relevant process/system boundary.

Do not treat these as interchangeable metrics.

## Production representativeness vector
A pilot/PVT/run-at-rate claim should state representativeness across:
- product design/configuration;
- production materials/components;
- suppliers/sites;
- tooling/fixtures/equipment;
- process recipe/parameters;
- operators/qualification;
- work instructions/routing;
- inspection/test/measurement system;
- quality controls/reaction plans;
- environment/layout/material flow;
- rate/product mix/shift duration;
- maintenance/support conditions.

Evidence transfers only across representative dimensions.

## Sustained run-at-rate principle
A short burst at target rate does not by itself demonstrate sustainable production capacity.

Rate evidence should state, where applicable:
- duration and number of consecutive cycles/shifts;
- product mix;
- accepted output versus gross output;
- downtime/microstops;
- rework/scrap;
- staffing and engineering support level;
- material replenishment and logistics;
- equipment/tooling maintenance state;
- constraint utilization and queues/WIP;
- whether abnormal containment or heroic intervention was required.

## Bottleneck / WIP / queue framework
Capacity should be reasoned from system flow and constraints.

Questions:
1. Which resource/process currently constrains accepted throughput?
2. Does the constraint change with variant/product mix?
3. Where is WIP accumulating and why?
4. Is upstream overproduction masking the constraint rather than increasing system throughput?
5. Are rework loops consuming constraint capacity?
6. Do inspection/test/approval queues constrain release even when fabrication capacity is available?

## Ramp learning model
Ramp is an evidence-building period, not merely a planned quantity increase.

Track at least:
- FPY/RTY where applicable;
- defect/rework/scrap mechanisms;
- cycle-time distribution and downtime;
- engineering support/interventions;
- supplier/input excursions;
- measurement/test escapes;
- open NCR/deviation burden;
- bottleneck migration;
- change frequency;
- sustained-rate evidence.

Learning-curve improvement must not be assumed automatically; identify what actually changed in design, process, tooling, skill, controls or supply.

## Engineering-change cut-in during ramp
Every material design/process/supplier/tooling/software change during ramp should answer:
- what configuration/lot/serial/time effectivity changes;
- WIP and inventory disposition;
- what prior evidence remains valid;
- what needs revalidation/requalification;
- updated PFMEA/control-plan/test/WI impact;
- supplier/tooling readiness;
- containment/monitoring after cut-in;
- genealogy linkage to affected units.

## Claim register
### C-RAMP-001 — A pilot/PVT build should test the production system, not only product function
status: STRONG
Evidence basis: NASA PRR + AIAG PPAP production-run logic.

### C-RAMP-002 — Production representativeness is multidimensional
status: STRONG SYNTHESIS
Evidence basis: PRR/PPAP/readiness evidence spans configuration, process, tooling, resources, controls and production conditions.

### C-RAMP-003 — One successful production build is weak evidence of repeatability
status: STRONG SYNTHESIS
Evidence basis: readiness/approval frameworks seek repeated/production-run evidence rather than a single successful article.

### C-RAMP-004 — Yield, rework and scrap affect flow/capacity as well as quality and cost
status: STRONG
Evidence basis: NIST MEP FPY/rework/lead-time case plus process-economics logic from A3.

### C-RAMP-005 — Ramp problems can expose interactions across product, process, supplier, tooling, measurement and standard work
status: STRONG SYNTHESIS
Pass 2: collect multi-factor launch cases.

### C-RAMP-006 — Capacity should be evaluated at the system constraint rather than by averaging local utilization
status: STRONG DIRECTION
Evidence basis: NIST throughput/bottleneck research + constraint reasoning.

### C-RAMP-007 — Takt time, cycle time, throughput, capacity and lead time are related but distinct
status: STRONG
Evidence basis: operations/lean definitions and manufacturing-system literature.

### C-RAMP-008 — Engineering changes during ramp require controlled cut-in/effectivity and revalidation impact assessment
status: STRONG SYNTHESIS
Evidence basis: configuration/change architecture from A0/A1 plus production-readiness need to maintain final production configuration.

### C-RAMP-009 — Sustainable run-at-rate evidence is stronger than a short target-rate burst
status: STRONG SYNTHESIS / sector-specific methods vary
Evidence basis: PPAP production-run-at-production-rates intent + production-readiness/resource logic.

### C-RAMP-010 — WIP accumulation is a diagnostic signal of flow imbalance/constraints, not proof of productive capacity
status: STRONG DIRECTION
Evidence basis: NIST manufacturing-system and MEP flow/bottleneck cases.

## Myth register
- 'One good pilot means production is validated' — REJECT.
- 'Hit takt once = proven capacity' — REJECT.
- 'High utilization everywhere means a healthy line' — REJECT as universal rule.
- 'More WIP means more output' — REJECT as universal rule.
- 'Rework does not affect capacity because the part is eventually good' — REJECT.
- 'Ramp improvement happens automatically with repetition' — REJECT; mechanisms/interventions must be identified.

## DEV / LVP / SVP lens
### DEV
Build to learn product/system behavior. Do not infer production rate/capability from engineering builds.

### LVP
Pilot builds validate repeatable manual/semi-automated routing, tooling, work instructions, test, controls, supplier inputs and rework/disposition. Capture loss mechanisms and engineering interventions explicitly.

### SVP
Demonstrate stable serial flow, constraint capacity, sustained yield, controlled changes, maintenance/readiness and rate performance under representative production conditions and product mix.

## Breadth result
A5 now contains authoritative source families, episode-critical claims, applicability limits, myth register and explicit Pass-2 targets for pilot/ramp/rate/capacity decisions.

## Pass-2 targets
- worked pilot/PVT readiness checklist;
- representative run-at-rate example with sustained-duration assumptions;
- FPY/rework/lead-time case;
- takt/cycle/throughput/capacity worked example;
- WIP/queue/bottleneck case;
- learning/ramp intervention case;
- engineering-change effectivity/revalidation case;
- product/process representativeness matrix.

## Readiness
Source map: BREADTH COMPLETE
Critical claims identified: YES
Primary-source backbone: GOOD
Applicability conflicts visible: YES
Quantitative/case depth: OPEN
Podcast Ready: NO