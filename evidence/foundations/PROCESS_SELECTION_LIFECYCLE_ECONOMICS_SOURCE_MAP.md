# Manufacturing Process Selection & Lifecycle Economics — Evidence Source Map

status: IN PROGRESS — BRIDGE MANUFACTURING BACKBONE CAPTURED
campaign: A3
maps_to: MASTER_WBS 3.0, 3.1 and cross-process economics; PODCAST_MAP Episode 11 + process arc
provenance: primary-source-first

## Purpose
Build the evidence backbone for choosing manufacturing processes based on whole-product and whole-chain requirements rather than habit, prototype convenience or single-variable unit price.

## Source backbone

### NIST — Conceptual Process Planning / DPPI
Evidence role:
- conceptual process planning allows designers to evaluate manufacturability, manufacturing cost and manufacturing time early;
- process planning/design integration is necessary because major manufacturing cost is committed during specification/design;
- process selection, resource selection and cost/time estimation belong in early design reasoning.

### NIST — Manufacturing Process and Material Selection / MAMPS
Evidence role:
- material and process selection are coupled;
- selection is multi-attribute rather than single-variable;
- early requirements may be incomplete/imprecise and alternatives must be screened against multiple criteria.

### NIST — Manufacturing process object-model research
Evidence role:
- manufacturing economics includes more than the transformation step;
- process representations include setup, handling, loading/unloading, processing, equipment, sequence, estimated cost and time;
- supports process-chain rather than isolated-machine reasoning.

### NIST SP 1176 — Costs and Cost Effectiveness of Additive Manufacturing
Evidence role:
- AM is not universally cheaper than traditional manufacturing;
- tooling avoidance can materially change low-volume economics;
- machine utilization and material cost can dominate AM economics;
- comparison is context dependent and many studies have limited scope.

### NIST — Costs, Benefits and Adoption of Additive Manufacturing: A Supply Chain Perspective
Evidence role:
- published cost comparisons often focus on individual parts and may omit inventory, transport and supply-disruption effects;
- total advantage may therefore differ from direct part-production cost;
- evidence supports explicit system boundary when making process-economics claims.

### NIST MEP — Additive Manufacturing / 3D Printing
Evidence role:
- identifies rapid prototyping, avoidance of tooling lead time/cost, low-volume/custom production, replacement parts and tooling applications as common AM opportunities;
- useful practitioner corroboration, but not a universal break-even rule.

### NIST Manufacturing Cost Guide
Evidence role:
- manufacturing economics can be decomposed into broader standardized cost categories and supply-chain components;
- useful for reinforcing cost-boundary discipline;
- not a direct part-level process-selection calculator and must not be presented as one.

### Commercial bridge-manufacturing examples — Protolabs
Evidence role:
- aluminum injection tooling can be used as an intermediate bridge before higher-capital steel tooling;
- pilot/low-volume molding can validate design, assembly and market demand before mass-production commitment;
- bridge tooling can reduce schedule and capital exposure while long-term tooling is not yet justified.

Applicability boundary: supplier-specific capabilities and quoted volume ranges are examples, not universal process thresholds.

### Commercial bridge-manufacturing examples — Formlabs
Evidence role:
- 3D-printed molds combined with injection molding provide a concrete example of a hybrid bridge route;
- short-run molding may be used for functional prototypes, pilot production or low-volume end-use parts.

Applicability boundary: tool durability, material compatibility, tolerance/capability and economics are application-specific.

## Canonical process-selection decision dimensions
- function/performance
- material
- geometry/size
- tolerance/GD&T
- surface/finish
- special material state
- joining/assembly consequences
- volume/rate
- tooling/NRE
- tooling lead time and useful life
- setup/changeover
- direct processing/cycle time
- labor/handling
- machine/resource utilization
- yield/scrap/rework
- inspection/test burden
- secondary/post-process operations
- supplier maturity/capacity
- automation/flexibility
- change frequency/product mix
- forecast confidence / demand volatility
- logistics/lead time/inventory
- supply disruption exposure where material
- cost per good part
- lifecycle/service/end-of-life consequence where material

## Cost-boundary model for the podcast
Do not compare processes until the cost boundary is explicit.

### Minimum direct manufacturing boundary
Cost per good part should consider, as applicable:
- material consumed
- direct processing/resource time
- setup/changeover allocation
- direct labor/handling
- tooling/NRE amortization
- consumables
- secondary operations
- inspection/test
- expected scrap/rework/yield loss

### Extended business boundary
For decisions where material, additionally evaluate:
- tooling lead time
- inventory/warehousing
- logistics/transport
- supplier qualification/management
- design-change cost and obsolete inventory/tooling
- maintenance/spares
- capacity constraint/opportunity cost
- supply disruption exposure

Do not mix direct-part and extended-business cost boundaries without labeling the difference.

## Break-even reasoning model
For two candidate routes A and B, a useful first-order educational model is:

TotalCost_A(Q) = Fixed_A + Q * VariableGoodPart_A
TotalCost_B(Q) = Fixed_B + Q * VariableGoodPart_B

where VariableGoodPart must use expected good output rather than ideal machine-cycle cost when yield/rework/inspection materially differ.

Simple break-even quantity, only when assumptions are sufficiently linear:
Q* = (Fixed_B - Fixed_A) / (VariableGoodPart_A - VariableGoodPart_B)

### Required warning
This equation is an educational first-order model, not a universal manufacturing law. Real routes may have stepped tooling, cavities, nonlinear labor, MOQ, capacity limits, learning curves, maintenance, tool replacement, supplier pricing tiers and design changes.

## Bridge Manufacturing framework
Bridge manufacturing is a deliberate temporary or intermediate route used to learn, supply early demand, validate production assumptions or reduce schedule/capital risk before committing to the intended long-term route.

It is not a single technology. Examples can include:
- CNC before casting/forging/molding;
- AM for low-volume end-use parts before dedicated tooling;
- aluminum/soft tooling before hardened production tooling;
- 3D-printed molds for short-run molding;
- manual/semi-automated assembly before dedicated automation;
- a prototype route combined with production-representative finishing, inspection or test.

### Bridge decision questions
1. What uncertainty is the bridge buying down: design, demand, process, supplier, tooling or schedule?
2. Which properties/failure mechanisms are representative of the intended route, and which are not?
3. What is the bridge's NRE, cost per good part, lead time and capacity envelope?
4. How likely is another design change before long-term tooling/process lock-in?
5. What is the cost of waiting for the intended serial route versus producing now?
6. What requalification/revalidation will be required when the route changes?
7. What is the explicit exit trigger from the bridge?

### Exit triggers from a bridge route
Do not use fixed universal quantities such as 10/100/1,000/10,000 as engineering rules. Transition when one or more of these become true:
- demand/rate exceeds bridge capacity or lead-time needs;
- cumulative variable-cost penalty justifies long-term NRE;
- design stability is sufficient to justify tooling lock-in;
- bridge process cannot achieve CTQ/capability/reliability requirements;
- inspection/rework burden becomes uneconomic;
- supplier/process risk changes materially;
- automation/tooling now meets ROI and flexibility needs;
- commercial schedule, inventory or supply economics favor the target route.

## Claim register

### C-PS-001 — Manufacturing-process selection is a multi-attribute decision, not a single-variable unit-cost choice
status: STRONG
Evidence basis: NIST process/material decision-support research.

### C-PS-002 — Process selection should occur early enough to influence detailed design
status: STRONG
Evidence basis: NIST conceptual/embodiment design and process-planning research.

### C-PS-003 — Material and manufacturing process selection are coupled decisions
status: STRONG
Evidence basis: NIST integrated material/process selection work.

### C-PS-004 — A manufacturing process should be evaluated as part of a process chain when secondary operations materially affect performance, tolerance, finish, yield or economics
status: STRONG DIRECTION
Evidence basis: NIST process models include sequences, setup, handling and processing; deeper quantitative process-chain cases remain Pass 2.

### C-PS-005 — Lowest quoted piece price is not necessarily lowest cost per good part
status: STRONG SYNTHESIS
Evidence basis: NIST cost/process models and AM supply-chain literature show relevant costs outside nominal transformation price. Quantitative examples remain Pass 2.

### C-PS-006 — Prototype convenience is not sufficient evidence for serial-process selection
status: STRONG SYNTHESIS from A0/A2/A3
Evidence basis: prototype representativeness limits + material/process coupling + production economics.

### C-PS-007 — Volume changes the tradeoff among flexible low-NRE and dedicated high-NRE processes
status: STRONG DIRECTION
Evidence basis: NIST AM economics supports tooling-avoidance/low-batch advantage in applicable cases while warning that AM can exceed traditional-process cost in many instances. Universal break-even volumes are explicitly rejected.

### C-PS-008 — '3D printing is always cheaper at low volume' is false as a universal rule
status: STRONG
Evidence basis: NIST SP 1176 reports many instances where AM product cost exceeds traditional methods while identifying contexts where small-batch economics can favor AM.

### C-PS-009 — A process-cost comparison is incomplete if its system boundary omits material secondary costs that differ between routes
status: STRONG DIRECTION
Evidence basis: NIST AM supply-chain review explicitly notes that many comparisons omit inventory, transportation and supply-disruption effects.

### C-PS-010 — Cost-per-good-part should use expected accepted output, not ideal cycle economics, when routes differ materially in yield/rework/inspection
status: ENGINEERING SYNTHESIS — NEEDS DIRECT CORROBORATION
Keep visible for Pass 2 rather than promote to verified fact solely from logic.

### C-PS-011 — Bridge manufacturing can reduce schedule/capital risk before final production commitment
status: MODERATE/STRONG INDUSTRIAL SUPPORT
Evidence basis: NIST tooling/low-volume economics plus commercial bridge-tooling examples.
Boundary: benefit depends on design stability, demand, representativeness, qualification and the economics of the specific route.

### C-PS-012 — The correct exit from a bridge process should be decision-triggered, not based on a universal quantity threshold
status: STRONG SYNTHESIS
Evidence basis: source material shows process economics are context-specific and practical supplier ranges vary materially.

### C-PS-013 — Switching from a bridge route to the serial route can invalidate part of the prior evidence and require revalidation
status: STRONG SYNTHESIS from A0/A2
Basis: process/material/tooling changes can alter failure mechanisms, tolerance distributions, surface state, residual stress, assembly behavior or inspection strategy.
Pass 2: collect concrete commercial cases.

## DEV / LVP / SVP lens
### DEV
Optimize learning speed and reversibility. Tooling avoidance can be economically valuable, but record which prototype-route assumptions do not transfer to production.

### LVP
Use bridge routes deliberately. Compare manual/semi-automated routes, AM/CNC/soft tooling and supplier options using cost per good part, design-change flexibility, quality/test burden, representativeness and expected demand.

### SVP
Evaluate stable process chains using capacity, yield, capability, tooling life/amortization, automation, supplier maturity, maintenance and full process-chain economics. A mature serial route can still be a flexible process if it wins the whole-system decision.

## Myth register
- '3D printing is always cheaper at low volume' — REJECT as universal claim; context dependent.
- 'Injection molding is always cheapest at volume' — OPEN; likely directionally common in appropriate geometry/material but requires assumptions and counterexamples.
- 'CNC is too expensive for production' — OPEN; cannot state without geometry/material/tolerance/volume/automation context.
- 'The process with the lowest quote wins' — REJECT as decision rule.
- 'Break-even volume is a property of the process' — REJECT; it is a property of compared routes and assumptions.
- 'Once volume reaches X, switch processes' — REJECT as universal rule.

## Breadth gaps to close
1. direct authoritative treatment of yield/rework/inspection in part-level cost-per-good-part;
2. tooling/NRE/tool-life and stepped-capacity economics outside AM;
3. cross-process bridge cases across metals/polymers beyond supplier examples;
4. supplier maturity/capacity as process-selection variable;
5. cross-process cases: injection molding vs machining/AM, casting + machining, forming + finish operations;
6. explicit make-versus-buy boundary and when it belongs to A3 versus supplier campaign;
7. stronger evidence for design-change flexibility versus dedicated-tooling lock-in.

## Pass-2 candidates
- transparent break-even examples with stated assumptions rather than universal thresholds;
- cost-per-good-part models including yield/rework/inspection;
- bridge-manufacturing cases;
- near-net + finish-machining cases;
- process-chain comparison cases;
- supplier/tooling lead-time effects;
- design-change flexibility versus dedicated-tooling lock-in;
- cases where a bridge process masked a serial-route failure mechanism.

## Readiness
Source map: IN PROGRESS — BRIDGE MANUFACTURING BACKBONE CAPTURED
Critical claims identified: YES
Primary-source backbone: YES
Volume/tooling direction: YES, quantitative generalization intentionally avoided
Bridge-manufacturing evidence: CAPTURED
Cost-boundary model: DEFINED
Quantitative process-chain cases: OPEN
Podcast Ready: NO