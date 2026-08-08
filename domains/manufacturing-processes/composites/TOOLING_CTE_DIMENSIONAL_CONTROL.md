# 3.8.7 Composite Tooling, CTE & Dimensional Control

status: Researching
provenance: [GNR]

## Objects
- tooling material
- tool CTE
- laminate CTE
- cure shrinkage
- spring-in / spring-back
- thermal gradient
- tool thermal mass
- release system
- tool surface finish
- tool durability
- dimensional compensation
- datum strategy

## Engineering questions
- How does tool/part CTE mismatch affect cured geometry?
- When should tool compensation be based on trial data rather than CAD nominal?
- How are cure shrinkage and spring-in separated from fixture/location error?
- What tooling strategy fits prototype, bridge and serial volume?
- Which datums are stable before cure, after cure and after trim?

## Decisions
### D-COMP-TOOL-001 — Select tooling material and construction
### D-COMP-DIM-001 — Does the part require dimensional compensation?
### D-COMP-DATUM-001 — What datum strategy should control layup, cure, trim and inspection?

## Cross-links
Tool CTE <-> cure cycle
Tool CTE <-> dimensional stability
Dimensional compensation <-> process capability
Tool durability <-> volume/economics
Datums <-> trimming/inspection

Quantitative compensation values remain evidence/part-system specific.