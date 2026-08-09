# DFM / DFA / DFT Foundations — Evidence Source Map

status: IN PROGRESS
campaign: A2
maps_to: MASTER_WBS Section 2; PODCAST_MAP Episodes 6–10
provenance: primary-source-first

## Purpose
Build the evidence backbone for cross-process design decisions that determine whether hardware can be manufactured, assembled, tested, tolerated, serviced and transitioned from prototype to production economically and robustly.

## Authoritative source backbone captured

### NIST — Incorporating Process Planning into Conceptual Design
Source: https://www.nist.gov/publications/incoporating-process-planning-conceptual-design
Authority: primary U.S. government manufacturing research
Use for:
- integrating process planning into conceptual/early design
- assessing manufacturability and manufacturing cost before design lock
- supporting the claim that design and manufacturing planning should communicate early
Key evidence direction: NIST explicitly states that major manufacturing costs are committed during product specification/design and that manufacturability and cost should be assessed as early as possible.
Applicability: broad manufacturing research; implementation details vary by industry/product.

### ASME Y14.5 — Dimensioning and Tolerancing
Primary standard/product page: https://www.asme.org/codes-standards/find-codes-standards/y14-5-dimensiones-y-tolerancias
Supporting ASME learning pages:
- https://www.asme.org/learning-development/find-course/essentials-y14-5-dimensioning-tolerancing
- https://www.asme.org/learning-development/find-course/asme-gd-t-fundamentals-asme-y14-5-course
Authority: primary standards body
Use for:
- GD&T as a standardized design language
- design-intent communication across design, manufacturing, tooling and inspection
- datum/tolerance/specification architecture
- product-realization communication and verification planning
Key evidence direction: ASME describes Y14.5 as the authoritative guideline for stating/interpreting GD&T and emphasizes form/fit/function/interchangeability and uniformity of specification/interpretation.
Applicability: exact invoked edition matters; ASME Y14.5 is not automatically the governing standard in every jurisdiction/customer environment.

### AIAG / automotive Core Tools
Use for:
- product/process risk linkage
- APQP/Control Plan/FMEA/MSA/SPC/PPAP relationships
- design/process development connection
Applicability: automotive-specific requirements; broader engineering logic must be separated from contractual requirements.

## Source families still being populated

### DFA — assembly simplification and mistake prevention
Target source families:
- Boothroyd-Dewhurst / academic DFA literature
- human factors / assembly error-proofing research
- industrial assembly case studies
Use for:
- part count/handling/orientation
- insertion/accessibility
- fastening/joining simplification
- mistake-proofing and verification
Status: authoritative source capture still open.

### DFT — testability / diagnostic access
Target source families:
- IEEE/IEC electronics test standards/guidance where applicable
- JTAG/boundary-scan primary specifications and vendor implementation guidance
- production-test architecture references
Use for:
- test access
- programming/calibration access
- fault isolation
- production-test coverage/time/cost tradeoffs
Status: primary source capture open.

### ISO GPS standards family
Use for:
- geometric specification architecture outside ASME-centric environments
- specification/verification vocabulary and applicability comparisons
Status: source capture open; clause-level work belongs to Pass 2.

### Materials/process-selection literature and databases
Use for:
- material/process compatibility
- manufacturing route consequences
- supply maturity and lifecycle tradeoffs
Status: source capture open.

### Serviceability/repairability literature
Use for:
- access/replacement architecture
- repair versus replace decisions
- service-induced calibration/alignment/sealing risk
Status: source capture open.

## Claim register

### C-DFX-001 — Manufacturability should be evaluated during design, not only after design release
status: STRONG
Evidence basis: NIST conceptual-design/process-planning work explicitly argues for early manufacturability and cost assessment because substantial manufacturing cost is committed during specification/design.
Podcast use: Episode 6.

### C-DFX-002 — DFM optimization of one part/process can worsen whole-product assembly/test/lifecycle performance
status: GNR SYNTHESIS
Need: systems/cost evidence and case studies.
Podcast use: Episodes 6–10.

### C-DFX-003 — DFA includes mistake prevention, handling/orientation, access and verification, not only reducing part count
status: MODERATE DIRECTION
Need: authoritative/academic breadth before promotion.
Podcast use: Episode 7.

### C-DFX-004 — Testability should be designed before production-test/EOL architecture is locked
status: GNR / HIGH PRIORITY
Need: electronics/system DFT sources and production examples.
Podcast use: Episode 8.

### C-DFX-005 — Tighter tolerances are not automatically better
status: STRONG ENGINEERING DIRECTION / QUANTITATIVE SUPPORT OPEN
Evidence basis: ASME Y14.5 establishes tolerance/GD&T as a language for design intent and product realization rather than a goal of minimizing numerical tolerance values. NIST early manufacturability/cost work supports the need to evaluate manufacturing consequences during design.
Boundary: the stronger economic statement — that unnecessary tightening increases cost or reduces yield — still needs quantitative/case evidence before Podcast Ready.
Podcast use: Episode 9.

### C-DFX-006 — Tolerance architecture should connect function, manufacturing interpretation and verification
status: STRONG
Evidence basis: ASME describes GD&T as communicating design intent across design, tooling/production and inspection, including form, fit, function and interchangeability.
Additional bridge needed: process capability/MSA evidence for statistical capability dimension.
Podcast use: Episode 9.

### C-DFX-007 — Material selection cannot be separated from manufacturing route and supply maturity
status: MODERATE/STRONG DIRECTION
Need: material/process-selection literature.
Podcast use: Episodes 6, 10, 11.

### C-DFX-008 — Prototype evidence transfers only across dimensions for which the prototype is representative
status: STRONG CONCEPTUAL SUPPORT from A0; non-aerospace depth open.
Podcast use: Episodes 6, 9, 10.

### C-DFX-009 — GD&T is a cross-functional product-realization language, not merely drafting notation
status: STRONG
Evidence basis: ASME explicitly connects Y14.5/GD&T to engineering design, manufacturing/tooling, production and inspection and describes it as a standardized method for communicating design intent.
Podcast use: Episode 9.

## Editorial conclusions already supportable
1. A CAD model that functions is not enough; the intended manufacturing route must be considered during design. citeturn211864search8
2. GD&T should be taught as communication of functional design intent across product realization, not as symbol memorization. citeturn211864search0turn211864search3
3. The podcast should reject the simplistic rule “tighter tolerance = better engineering”; exact quantitative cost/yield examples remain a Pass-2 target rather than an unsupported universal statement.

## DEV / LVP / SVP lens
### DEV
Optimize learning speed while recording which DFX constraints are intentionally deferred. Use prototype methods deliberately and document representativeness limits.

### LVP
Design must support repeatable manual/semi-automated assembly, practical inspection/test, controlled substitutions and economically sensible tolerances. Human access, orientation and error opportunities matter heavily.

### SVP
Design/process architecture must support capability, rate, scalable suppliers/tooling, automated or high-throughput test where justified, controlled variation and lifecycle/service strategy.

## Breadth gaps to close
1. authoritative DFA source family and empirical evidence;
2. DFT/test-access standards and industrial guidance;
3. quantitative tolerance-cost/capability evidence;
4. material/process selection sources;
5. serviceability/repairability evidence;
6. non-aerospace prototype representativeness case studies;
7. cross-process lifecycle-cost decision evidence;
8. top myths/mistakes/case studies for Episodes 6–10.

## Pass-2 candidates
- tolerance-cost quantitative examples;
- DFA case studies with measured assembly-time/error reduction;
- board/system DFT examples and test-coverage tradeoffs;
- material/process substitution failures;
- prototype-route mismatch case studies;
- standards/version applicability mapping.

## Readiness
Source map: ACTIVE
Critical claims identified: YES
Primary-source backbone: PARTIAL / STRONG FOR DFM+GD&T
Applicability conflicts visible: YES
Podcast Ready: NO