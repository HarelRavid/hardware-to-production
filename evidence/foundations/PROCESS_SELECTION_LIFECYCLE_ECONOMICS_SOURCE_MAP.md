# Manufacturing Process Selection & Lifecycle Economics — Evidence Source Map

status: IN PROGRESS
campaign: A3
maps_to: MASTER_WBS 3.0, 3.1 and cross-process economics; PODCAST_MAP Episode 11 + process arc
provenance: primary-source-first

## Purpose
Build the evidence backbone for choosing manufacturing processes based on whole-product and whole-chain requirements rather than habit, prototype convenience or single-variable unit price.

## Initial source backbone

### NIST — Manufacturing Process and Material Selection During Conceptual Design
Use for:
- early screening of compatible material/process alternatives
- balancing functional requirements and manufacturing economics
- recognizing that design decisions constrain feasible process choices and cost

### NIST — Decision Support System for Material and Manufacturing Process Selection
Use for:
- multi-attribute decision framing
- uncertain/imprecise early requirements
- process/material compatibility assessment

### NIST — Web-Based Process/Material Advisory System
Use for:
- early process/material comparison
- cost-effective combination search
- ensuring detailed design is compatible with selected process constraints

### NIST — Process/Material Selection During Embodiment Design
Use for:
- evaluating process sequences rather than only isolated processes
- cost estimation as one decision dimension
- exploring multiple material/process options before design lock-in

### NIST — Conceptual Process Planning / DPPI research
Use for:
- manufacturing cost/time estimation in early design
- process planning and design integration
- manufacturing-resource considerations before detailed design freeze

## Initial decision dimensions
- function/performance
- material
- geometry/size
- tolerance/GD&T
- surface/finish
- special material state
- joining/assembly consequences
- volume/rate
- tooling/NRE
- cycle time
- yield/scrap/rework
- inspection/test burden
- secondary/post-process operations
- supplier maturity/capacity
- automation/flexibility
- change frequency/product mix
- logistics/lead time
- cost per good part
- lifecycle/service/end-of-life consequence where material

## Claim register

### C-PS-001 — Manufacturing-process selection is a multi-attribute decision, not a single-variable unit-cost choice
status: STRONG
Evidence basis: NIST process/material decision-support research.

### C-PS-002 — Process selection should occur early enough to influence detailed design
status: STRONG
Evidence basis: NIST conceptual/embodiment design research.

### C-PS-003 — Material and manufacturing process selection are coupled decisions
status: STRONG
Evidence basis: NIST integrated material/process selection work.

### C-PS-004 — A manufacturing process should be evaluated as part of a process chain when secondary operations materially affect performance, tolerance, finish, yield or economics
status: STRONG DIRECTION
Evidence basis: NIST embodiment-design work evaluates process sequences; deep process-chain evidence remains Pass 2.

### C-PS-005 — Lowest quoted piece price is not necessarily lowest cost per good part
status: STRONG SYNTHESIS / quantitative depth open
Evidence direction: tooling/NRE, scrap/rework, inspection, secondary operations, logistics and yield must be incorporated. Pass 2 should quantify examples.

### C-PS-006 — Prototype convenience is not sufficient evidence for serial-process selection
status: STRONG SYNTHESIS from A0/A2
Evidence direction: prototype-fidelity limits + process/material constraints + production economics.

### C-PS-007 — Volume changes the economic tradeoff among flexible low-NRE and dedicated high-NRE processes
status: STRONG ENGINEERING DIRECTION / quantitative curves open
Need: authoritative cost-volume/tooling examples and case studies.

## DEV / LVP / SVP lens
### DEV
Favor fast learning and reversible choices, but record which process/material decisions are temporary and which product requirements are already constraining the future process family.

### LVP
Compare bridge processes, manual/semi-automated routes, soft tooling and supplier options using cost per good part, quality/test burden and expected design-change rate.

### SVP
Include tooling amortization, capacity, yield, process capability, automation, supply-chain maturity, maintenance, product mix and process-chain economics.

## Breadth gaps to close
1. authoritative lifecycle/cost-per-good-part framework;
2. volume/tooling/NRE economics sources;
3. process-chain and secondary-operation cost/yield evidence;
4. supplier maturity/capacity as process-selection variable;
5. process-selection case studies across polymers/metals/AM;
6. explicit make-versus-buy boundary and when it belongs to A3 versus A6;
7. myths: '3D printing is always cheaper at low volume', 'injection molding is always cheapest at volume', 'CNC is too expensive for production', etc.

## Pass-2 candidates
- break-even volume examples with clearly stated assumptions;
- cost-per-good-part models including yield/rework/inspection;
- bridge-manufacturing cases;
- near-net + finish-machining cases;
- process-chain comparison cases;
- supplier/tooling lead-time effects;
- design-change flexibility versus dedicated-tooling lock-in.

## Readiness
Source map: STARTED
Critical claims identified: YES
Primary-source backbone: YES for early multi-attribute selection
Quantitative economics: OPEN
Podcast Ready: NO