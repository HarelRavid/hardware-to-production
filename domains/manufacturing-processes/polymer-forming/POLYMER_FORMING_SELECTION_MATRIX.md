# 3.7.14 Polymer Forming Process Selection Matrix

status: Researching
provenance: [GNR]

## 3.7.14.1 Candidate Processes
- Injection molding (cross-reference)
- Extrusion
- Extrusion blow molding
- Injection blow / stretch blow molding
- Thermoforming / vacuum forming
- Pressure forming
- Rotational molding
- Compression molding
- Transfer molding
- Reaction injection molding
- CNC / additive manufacturing for comparison

## 3.7.14.2 Selection Criteria
The comparison must use scoped evidence and shall include:
- geometry family
- hollow vs open shell vs constant section
- part size
- wall-thickness behavior
- material family
- fiber/filler compatibility
- expected volume
- tooling cost
- tooling lead time
- cycle time
- labor content
- secondary operations
- dimensional capability
- surface/cosmetic capability
- automation potential
- scrap/material yield
- inspection strategy
- repair/rework
- production-process representativeness of prototypes

## 3.7.14.3 Qualitative Draft Matrix
All entries below are GNR placeholders pending evidence verification.

| Criterion | Extrusion | Blow Molding | Thermoforming | Rotomolding | Compression/Transfer | RIM |
|---|---|---|---|---|---|---|
| Natural geometry | continuous section | hollow body | formed sheet/shell | large hollow body | molded solid/filled composite | large molded reactive part |
| Tooling intensity | low–medium | medium | low–medium | low–medium | medium | medium |
| Secondary trim/operations | medium | medium | often high | medium | medium | medium |
| High-volume automation | high | high | high | medium | high | medium–high |
| Tight local interfaces | often secondary machining | neck/interface dependent | trim/secondary dependent | often secondary | process dependent | process dependent |
| Material orientation/process effects | high relevance | high relevance | high relevance | process specific | fiber/cure dependent | cure/mix dependent |

## 3.7.14.4 Master Decision Object
### D-POLYFORM-MASTER-001 — Which polymer-forming process should be used?

Inputs:
- functional geometry
- material and properties
- annual volume and ramp forecast
- product maturity
- tooling budget and lead time
- target unit cost
- dimensions/tolerances
- surface requirements
- environment
- secondary assembly
- inspection and validation
- automation strategy

Output structure:
1. Candidate processes
2. Disqualifying constraints
3. Key tradeoffs
4. Required evidence / unanswered questions
5. Prototype strategy before tooling commitment
6. NPI risks

## 3.7.14.5 Quality Gate Backlog
Before Podcast Ready:
- evidence-populate each comparison criterion
- add standards/source index
- add quantitative scoped DFM data
- add case studies
- build Top-20 questions/mistakes/decisions/myths/lessons
- perform GNR verification audit
