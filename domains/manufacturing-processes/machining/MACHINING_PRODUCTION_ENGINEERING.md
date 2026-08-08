# 3.6.12 Machining Production Engineering

status: Researching
provenance: [GNR]

## 3.6.12.1 Prototype-to-production transition
Prototype CNC success does not establish a serial-production process. The production model must additionally consider:
- setup reduction
- fixture repeatability
- datum control
- tool-life management
- chip/coolant management
- automated probing/metrology
- process capability
- operator dependency
- material/blank consistency
- traceability
- cycle-time balance
- preventive maintenance
- reaction plans

## 3.6.12.2 Workholding objects
- vise/chuck/collet
- soft jaws
- dedicated fixture
- modular fixture
- zero-point system
- palletization
- vacuum/magnetic workholding where applicable
- locating principle
- 3-2-1 constraint model
- clamping distortion
- fixture wear

## 3.6.12.3 Datum transfer
Design datum -> manufacturing datum -> fixture locator -> machine coordinate system -> inspection datum.

Misalignment between these layers is modeled as a potential source of variation and unnecessary setups.

## 3.6.12.4 Automation objects
- bar feeder
- pallet pool
- robot loading
- cobot tending
- automatic tool changer
- tool presetter
- broken-tool detection
- in-process probing
- automatic offset compensation
- chip management
- lights-out machining

## 3.6.12.5 Cost model objects
Cost per good part should consider:
- raw stock
- programming/NRE
- setup
- machine time
- tooling/consumables
- inspection
- deburr/cleaning
- scrap/rework
- handling
- secondary operations
- unattended utilization
- maintenance

## 3.6.12.6 Decision objects
### D-MACH-PROD-001 — Keep prototype process or industrialize it?
### D-MACH-SETUP-001 — One setup vs multiple setups?
### D-MACH-FIX-001 — Dedicated fixture justified?
### D-MACH-AUTO-001 — Automate machine tending?
### D-MACH-MAKEBUY-001 — In-house or outsource machining?

## 3.6.12.7 Why projects fail
- prototype cycle treated as production cycle
- unsupported tolerance copied from prototype drawing
- fixture introduced late
- datum strategy conflicts with machining sequence
- tool access forces avoidable setups
- inspection requirement is harder than machining requirement
- tool life not included in costing
- automation planned without chip/deburr/part-presentation strategy
- supplier selected on machine list rather than demonstrated capability

## 3.6.12.8 Evidence backlog
Populate economic and capability thresholds only with scoped shop/supplier data, industrial references and validated case studies. Present content is architecture/GNR.