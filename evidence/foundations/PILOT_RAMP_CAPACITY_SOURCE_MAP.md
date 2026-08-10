# Pilot / PVT / Ramp / Yield / Capacity — Evidence Source Map

status: IN PROGRESS — PILOT/RATE/YIELD BACKBONE CAPTURED
campaign: A5
maps_to: MASTER_WBS Section 5; PODCAST_MAP Episodes 26–31
provenance: primary-source-first

## Purpose
Build the evidence backbone for demonstrating that a production-intent system can repeatedly build conforming product, learn from yield/rework loss, and scale toward required rate without confusing one successful build with proven production capability.

## Source backbone

### NASA Production Readiness Review / manufacturing-readiness material
Evidence role:
- PRR asks whether the developer can efficiently produce the required number of systems, not merely whether one unit functions;
- entrance/success criteria include resolved production-engineering problems/nonconformances, adequate production documentation, production plans, critical controls/procedures, production-enabling resources, personnel and production configuration;
- additional NASA quality guidance identifies process controls/control limits, inspections and acceptance-data expectations.

Applicability boundary: aerospace/government program implementation is not a universal startup process. The transferable engineering principle is that production readiness is demonstrated across design, process, resources, controls and repeatable output.

### NIST MEP — First Pass Yield / lead-time case evidence
Evidence role:
- documents a manufacturing improvement where FPY increased from 10% to 90%, total processing time dropped from 11.8 h to 3.4 h and lead time fell from >40 days to 5 days;
- supports treating rework/low FPY as capacity and flow losses, not only quality-reporting metrics.

Applicability boundary: this is a case study, not a universal conversion formula between FPY and lead time.

### NIST MEP — Flow/WIP/production lead-time cases
Evidence role:
- industrial cases link WIP, layout, equipment availability, first-pass yield and production lead time;
- useful for demonstrating that system throughput/ramp performance can be constrained by flow and availability as well as nominal machine speed.

### Lean Enterprise Institute — takt time
Evidence role:
- takt time = available production time / customer demand;
- takt represents the pace required to satisfy demand and is therefore a demand/planning quantity, not an observed process cycle time.

### Lean Enterprise Institute — cycle time
Evidence role:
- cycle time is the measured time to produce a part or complete a process;
- machine cycle, operator cycle and effective machine cycle are distinct useful concepts;
- setup/load/unload can materially change effective cycle economics/capacity.

### Lean Enterprise Institute — standardized work / process capacity
Evidence role:
- process-capacity sheets use machine cycle, setup/change intervals and manual work to determine actual capacity and identify bottlenecks;
- standardized work explicitly relates takt, cycle time, work sequence and WIP.

Applicability boundary: lean terminology/practices are useful operating concepts, not universal regulatory requirements.

### ASQ quality glossary — First Pass Yield
Evidence role:
- FPY measures the share of units completing a process without scrap, rerun, retest, return or offline repair;
- supports keeping first-pass flow distinct from eventual final yield after rework.

## Production-validation representativeness framework
A pilot/PVT result should record which dimensions were production representative:
- released design/configuration
- production-intent materials/components
- intended suppliers/sites
- tooling/fixtures/equipment
- routing/process sequence
- recipes/parameters
- operators/training model
- work instructions/standard work
- measurement/test systems
- quality controls/reaction plans
- traceability/data capture
- environmental conditions
- batch/lot size
- run duration
- rate/takt/loading
- maintenance/setup/changeover state

Do not label a build simply 'production representative' without identifying the dimensions that actually were.

## Core metric distinctions
### Takt time
Demand-facing pace: available production time / required customer demand.

### Cycle time
Observed/engineered time for a work cycle/process/unit at a resource or station.

### Throughput
Accepted output per unit time across the defined system boundary.

### Capacity
Maximum sustainable output under stated assumptions/resource/configuration/availability conditions.

### Lead time
Elapsed time across the defined order/material/process boundary; can include queue/WIP/wait/rework as well as processing.

### FPY
Share passing a process first time without rework/retest/offline repair or scrap.

These terms must not be used interchangeably.

## Claim register

### C-RAMP-001 — A pilot/PVT build should test the production system, not only product function
status: STRONG
Evidence basis: NASA PRR explicitly evaluates readiness to produce the required number of units through production plans, resources, process controls, documentation and production configuration.

### C-RAMP-002 — Production representativeness is multidimensional
status: STRONG SYNTHESIS
Evidence basis: NASA readiness criteria span design, production plans, process controls, resources, personnel and configuration; A0/A1 prototype-fidelity work supports explicit dimension tracking.

### C-RAMP-003 — One successful production build is weak evidence of repeatability
status: STRONG SYNTHESIS
Evidence basis: PRR intent is efficient production of the required number, and A4 capability/stability evidence requires repeated process observations rather than one successful outcome.

### C-RAMP-004 — Yield, rework and scrap are flow/capacity signals as well as quality/financial metrics
status: STRONG INDUSTRIAL SUPPORT
Evidence basis: NIST MEP FPY case demonstrates simultaneous changes in FPY, processing time, lead time and available capacity.
Boundary: effect size is process-specific.

### C-RAMP-005 — Ramp problems can expose interactions among product design, process, supplier, tooling, measurement and standard work
status: STRONG SYNTHESIS
Evidence direction: NASA production-readiness scope + A1/A4/A6 interfaces. Pass 2 should capture concrete launch cases.

### C-RAMP-006 — Capacity should be evaluated at the system/constraint level, not inferred from average utilization
status: STRONG DIRECTION
Evidence basis: LEI process-capacity methods explicitly evaluate each linked process/resource to identify bottlenecks; quantitative constraint theory depth remains Pass 2.

### C-RAMP-007 — Takt time, cycle time, throughput, lead time and capacity are related but different
status: STRONG
Evidence basis: Lean Enterprise Institute definitions and process-capacity practices.

### C-RAMP-008 — Meeting takt for a brief run is not the same as demonstrating sustainable production rate
status: STRONG SYNTHESIS
Reasoning: sustainable rate also depends on yield, downtime, setup/changeover, maintenance, staffing, replenishment and the system constraint. Pass 2 should add rate-run cases.

### C-RAMP-009 — Engineering changes during ramp require controlled cut-in/effectivity and re-evaluation of affected production evidence
status: STRONG SYNTHESIS from A0/A1/Section 5 architecture
Need: direct change/ramp case studies in Pass 2.

### C-RAMP-010 — Final yield can hide unstable first-pass flow
status: STRONG DIRECTION
Evidence basis: ASQ definition of FPY distinguishes first-pass output from units later recovered by rerun/retest/repair; NIST case demonstrates the operational importance of reducing rework.

## Pilot / PVT evidence questions
1. Was the product configuration production intent and traceable?
2. Were suppliers/materials representative?
3. Were intended tooling/process/test systems used?
4. Were operators and instructions representative of normal production rather than engineering heroics?
5. What failures/rework/holds occurred and where were they created/detected?
6. What was FPY versus eventual final yield?
7. What rate was actually demonstrated and for how long?
8. What downtime/setup/changeover/maintenance was excluded?
9. What was the system constraint during the run?
10. What changed after the build, and which evidence therefore expired?

## DEV / LVP / SVP lens
### DEV
Build to learn product/system behavior. Do not infer production rate/capability from engineering builds or engineer-intensive assembly.

### LVP
Use pilot builds to validate repeatable manual/semi-automated routing, tooling, work instructions, test, controls, supplier inputs and rework/disposition. Capture first-pass losses and engineering intervention explicitly.

### SVP
Demonstrate stable serial flow, sustained constraint capacity, yield, staffing/material replenishment, maintenance readiness and rate performance using representative production conditions.

## Myth register
- 'We built one good unit, so production is ready' — REJECT.
- 'Meeting takt for one shift proves capacity' — REJECT as universal claim.
- 'Final yield is enough; rework does not matter if the product ships' — REJECT.
- 'High utilization everywhere means a healthy line' — REJECT as decision rule; local utilization can conflict with system flow.
- 'Cycle time and takt time are the same thing' — REJECT.
- 'The fastest machine defines line capacity' — REJECT.

## Breadth gaps to close
1. production-rate/run-at-rate evidence and sustained-rate cases;
2. stronger bottleneck/constraint sources and queue/WIP relationships;
3. ramp/learning-curve sources;
4. engineering-change cut-in during ramp;
5. explicit PVT/pilot nomenclature applicability outside specific companies/sectors;
6. case studies for Episodes 26–31.

## Pass-2 targets
- worked pilot readiness checklist;
- repeated-build evidence example;
- FPY/rework/lead-time case;
- takt/cycle/capacity worked example;
- bottleneck/line-balance case;
- sustained-rate/run-at-rate case;
- ramp change/effectivity case;
- product/process representativeness matrix.

## Readiness
Source map: IN PROGRESS — PILOT/RATE/YIELD BACKBONE CAPTURED
Critical claims identified: YES
Primary-source backbone: GOOD
Metric definitions: CAPTURED
Pilot/PRR evidence: CAPTURED
Yield/flow case evidence: CAPTURED
Ramp/change cases: OPEN
Podcast Ready: NO