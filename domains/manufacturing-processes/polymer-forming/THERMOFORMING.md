# 3.7.11 Thermoforming & Vacuum/Pressure Forming

status: Researching
provenance: [GNR]

## 3.7.11.1 Process Families
- Vacuum forming
- Pressure forming
- Twin-sheet forming
- Plug-assist forming
- Matched-mold forming

## 3.7.11.2 Core Objects
- Sheet stock
- Heating
- Sag
- Mold
- Vacuum
- Forming pressure
- Plug assist
- Cooling
- Trim
- Scrap skeleton

## 3.7.11.3 DFM Principles
Thermoforming transforms a pre-made sheet, so design must account for draw depth, local stretching, corner thinning, draft, trim, sheet gauge and material orientation/history.

Questions:
- Can the part be generated from a sheet without unacceptable local thinning?
- Which side requires controlled cosmetic/tool surface?
- What trim datum establishes final geometry?
- Can undercuts be eliminated or handled with tooling strategy?
- Is the desired stiffness better achieved through geometry rather than excessive sheet thickness?

## 3.7.11.4 Failure / Variation Objects
- webbing
- excessive thinning
- bridging
- poor detail replication
- incomplete forming
- wrinkles
- sheet sag variability
- warpage
- trim variation
- cosmetic marks

## 3.7.11.5 Decision Objects
### D-THERMO-001 — Thermoform or injection mold?
### D-THERMO-002 — Vacuum or pressure forming?
### D-THERMO-003 — Plug assist justified?
### D-THERMO-004 — Form as one shell or split/assemble?

## 3.7.11.6 Production Engineering
- sheet incoming control
- heating-zone control
- sheet temperature measurement
- mold cooling
- trimming fixtures/CNC trimming
- scrap handling
- automated loading/unloading
- inspection of wall distribution and trim datum

## 3.7.11.7 Why Projects Fail
- CAD designed like an injection-molded part
- deep draws without thickness-distribution analysis
- trim strategy defined too late
- prototype thickness assumed representative of formed production thickness
- cosmetic surface and tool side not defined

## 3.7.11.8 Evidence Backlog
Quantitative draw ratios, draft values and thickness-retention claims require material/process/tool-specific evidence before publication.