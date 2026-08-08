# 3.6 Machining — Engineering Claim Registry

All AI-originated synthesis remains marked `GNR` per ADR-003.

## H2P-CLM-MACH-001 — Machine positioning accuracy is not identical to finished-part accuracy
Statement: Axis positioning accuracy and repeatability are contributors to part accuracy, but finished-part error can also include dynamic contouring, thermal, tooling, workholding, cutting-force and process effects.
- Classification: Standard-supported project synthesis
- Confidence: Very High
- Provenance: [GNR, STD]
- Evidence: ISO 230-2:2014; ISO 230-12:2022

## H2P-CLM-MACH-002 — More stringent tolerances should be function-driven
Statement: Applying tight dimensional or geometric tolerances to nonfunctional features can add process, setup and inspection burden without improving product learning or performance.
- Classification: Industrial Best Practice / Project Synthesis
- Confidence: High
- Provenance: [GNR, SYN]

## H2P-CLM-MACH-003 — Tool access and rigidity can dominate nominal machine travel
Statement: A feature can lie inside the machine envelope yet remain impractical because cutter/holder access, stick-out, chip evacuation, deflection or workholding prevent a robust process.
- Classification: Engineering Principle
- Confidence: Very High
- Provenance: [GNR, IND, SYN]

## H2P-CLM-MACH-004 — Setup count is a first-order low-volume cost driver
Statement: In prototype and low-volume machining, an additional setup can materially increase elapsed lead time, datum-transfer risk, programming/workholding effort and inspection burden even when cutting time is short.
- Classification: Project Synthesis
- Confidence: High
- Provenance: [GNR, IND, SYN]

## H2P-CLM-MACH-005 — Surface texture and surface integrity are different engineering concepts
Statement: A measured surface texture parameter does not by itself describe subsurface metallurgical, residual-stress or damage conditions created by machining.
- Classification: Engineering Principle
- Confidence: High
- Provenance: [GNR, SYN]

## H2P-CLM-MACH-006 — Tool life is a process-economic variable, not merely a tooling variable
Statement: Tool wear can affect dimensional drift, surface condition, cycle interruption, scrap risk, automation stability and unit cost; tool-life strategy therefore belongs in process design.
- Classification: Engineering Principle
- Confidence: High
- Provenance: [GNR, SYN]

## H2P-CLM-MACH-007 — In-process measurement does not automatically replace independent inspection
Statement: On-machine probing can support setup and process control, but its uncertainty and shared machine-error sources must be understood before using it as final acceptance evidence.
- Classification: Government evidence / Project Synthesis
- Confidence: High
- Provenance: [GNR, GOV, SYN]

## H2P-CLM-MACH-008 — Cutting data are contextual
Statement: Cutting speed, feed, depth/width of cut and coolant recommendations are not universal material constants; usable values depend on tool geometry/material/coating, work material condition, machine dynamics, workholding and objective.
- Classification: Engineering Principle
- Confidence: Very High
- Provenance: [GNR, IND, SYN]

## H2P-CLM-MACH-009 — Near-net-shape plus machining can outperform all-machined production
Statement: At suitable volume and geometry, casting, forging, extrusion or additive near-net shapes followed by machining of functional interfaces can reduce material removal while retaining precision where needed.
- Classification: Project Synthesis
- Confidence: High
- Provenance: [GNR, SYN]

## H2P-CLM-MACH-010 — Process capability must be feature-specific
Statement: A generic supplier or machine tolerance statement should not be treated as proof that a specific feature, orientation, material, size and inspection condition can repeatedly meet the requirement.
- Classification: Quality Engineering Principle
- Confidence: Very High
- Provenance: [GNR, SYN]

## Open evidence gaps
- Peer-reviewed evidence for surface integrity by process/material family.
- Tool-wear/process-capability links.
- Quantitative setup-cost and lead-time studies.
- Production case studies comparing billet machining with near-net routes.