# 3.11 Additive Manufacturing — Domain Map

status: Researching
provenance: [GNR]

## 3.11.1 Scope
Additive manufacturing from prototype use through qualified production, including polymer, metal, ceramic/powder-boundary processes, DfAM, post-processing, inspection, economics and the decision not to use AM.

## 3.11.2 Process families
- Material extrusion: FFF/FDM
- Vat photopolymerization: SLA/DLP and related routes
- Powder bed fusion polymers: SLS
- Material jetting / powder-fusing industrial polymer routes including MJF boundary
- Metal powder bed fusion: LPBF/PBF-LB
- Directed energy deposition: DED
- Binder jetting
- Material jetting
- Sheet lamination boundary
- Hybrid additive/subtractive

## 3.11.3 Cross-cutting objects
- feedstock
- layer thickness
- build orientation
- support strategy
- scan/toolpath strategy
- build plate/nesting
- anisotropy
- thermal history
- residual stress
- distortion
- porosity
- surface condition
- dimensional accuracy
- post-processing
- heat treatment/HIP
- machining
- inspection/NDT
- powder/material reuse
- machine qualification
- build traceability

## 3.11.4 DfAM questions
1. Does AM create functional value or only avoid tooling?
2. Can part consolidation reduce assembly risk/cost?
3. Can internal channels/lattices/topology optimization create useful performance?
4. Is the geometry printable but difficult/impossible to inspect, clean or post-process?
5. Can critical datums and surfaces be machined after build?
6. Does orientation optimize the right combination of support, properties, distortion, surface and cost?
7. Is the prototype AM route representative of the intended production process?
8. Would machining, molding, casting, fabrication or a hybrid route be superior?

## 3.11.5 Master decision object
### D-AM-MASTER-001 — Should this component use additive manufacturing?
Inputs: material, geometry, functional complexity, internal features, consolidation opportunity, mechanical/environmental requirements, quantity, lead time, tooling avoidance, surface/tolerance, inspection, post-processing, qualification, supplier/machine capability and lifecycle cost.

Output: AM candidates + conventional/hybrid alternatives + evidence + assumptions + open questions.

## 3.11.6 Integrity rule
“Printable” is not equivalent to manufacturable, inspectable, qualified or economical. Quantitative capability remains process/material/machine scoped. AI synthesis remains GNR until verified.