# 3.6.15 Machining Cost Drivers

status: Researching
provenance: [GNR]

## 3.6.15.1 Cost structure
Machining cost is modeled as fixed/NRE plus recurring cost per good part.

Fixed/NRE candidates:
- DFM/CAM programming
- fixture design and manufacture
- soft jaws / workholding preparation
- inspection programming
- special tooling
- process development and qualification

Recurring candidates:
- raw stock
- machine occupancy
- labor/tending
- cutting tools and consumables
- coolant/process media
- deburr/cleaning
- inspection
- secondary operations
- scrap/rework
- maintenance allocation

## 3.6.15.2 Major engineering cost drivers
- setup count
- number of orientations
- long-reach tooling
- deep holes/cavities
- high material-removal ratio
- difficult-to-machine material
- tight tolerances
- demanding surface integrity
- dedicated inspection
- custom tooling
- small batch size
- low unattended utilization

## 3.6.15.3 Cost per good part
A faster nominal cycle is not necessarily lower cost if it increases:
- tool consumption
- scrap risk
- dimensional drift
- machine downtime
- inspection/rework

Use good-part economics rather than cutting-time optimization alone.

## 3.6.15.4 Volume transition
Decision comparison must include:
- machine from billet indefinitely;
- standard extrusion + machining;
- forging + machining;
- casting + machining;
- additive near-net + machining;
- dedicated transfer/production machining.

Break-even volume is not a universal process number; it depends on geometry, material, tooling, supplier, capacity and business assumptions.

## 3.6.15.5 Decision objects
- D-MACH-COST-001: Which feature dominates cost?
- D-MACH-COST-002: Is dedicated fixturing economically justified?
- D-MACH-COST-003: When should the blank move to near-net shape?
- D-MACH-COST-004: Is automation justified by labor, utilization or capability?
- D-MACH-COST-005: Supplier quote delta — what design feature causes it?

## 3.6.15.6 Why projects fail
- unit price compared without NRE/tooling assumptions;
- quote accepted without understanding setup count;
- prototype stock strategy retained at production volume;
- material yield ignored;
- inspection and secondary operations absent from cost model;
- machine hourly rate treated as the only meaningful cost variable;
- automation justified only by direct labor savings.

Quantitative cost thresholds remain project/supplier-specific evidence, never universal Claims.