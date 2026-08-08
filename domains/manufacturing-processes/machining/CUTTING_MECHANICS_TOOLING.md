# 3.6.9 Cutting Mechanics, Tooling & Tool Life

status: Researching
provenance: [GNR]

## 3.6.9.1 Core objects
- Cutting speed
- Feed
- Depth of cut
- Chip thickness
- Chip formation
- Shear zone
- Cutting force
- Specific cutting energy
- Heat generation and partition
- Built-up edge
- Chatter / regenerative vibration
- Tool geometry
- Rake angle
- Clearance angle
- Edge preparation
- Nose radius

## 3.6.9.2 Tool-material system
Tool selection is modeled as a system, not a standalone catalog choice.

Workpiece material → operation → engagement → tool material/coating → geometry → cutting parameters → wear mode → capability/cost.

Tool families to populate:
- HSS
- Carbide
- Coated carbide
- Cermet
- Ceramic
- CBN
- PCD

## 3.6.9.3 Tool wear objects
- Flank wear
- Crater wear
- Notch wear
- Chipping
- Edge fracture
- Thermal cracking
- Plastic deformation
- Built-up edge

Tool life must be connected to dimensional drift, surface integrity, cycle time, tool-change strategy and cost per good part.

## 3.6.9.4 Production questions
1. Which variable limits productivity first: spindle power, rigidity, tool life, chip evacuation, surface integrity or dimensional capability?
2. Should tool changes be time/count based, condition based, or signature based?
3. Which tool-wear modes can create latent product risk before a dimensional inspection fails?
4. When does a faster cutting condition increase total cost per good part?

## 3.6.9.5 Decision objects
### D-MACH-TOOL-001 — Select tool system
Inputs: material, hardness, operation, geometry, reach, finish, volume, coolant strategy, machine capability.

### D-MACH-LIFE-001 — Tool replacement strategy
Candidate strategies: fixed part count, fixed cutting time, measured wear, process-signature monitoring, hybrid.

## 3.6.9.6 Relationships
Cutting parameters -> influence -> heat generation
Cutting parameters -> influence -> cutting force
Tool wear -> influences -> dimensional drift
Tool wear -> influences -> surface integrity
Tool overhang -> influences -> dynamic stiffness
Dynamic stiffness -> influences -> chatter risk
Tool-change policy -> influences -> OEE
Tool-change policy -> influences -> scrap risk

## 3.6.9.7 Evidence backlog
Populate quantitative relationships only from scoped machining handbooks, tool-maker technical references, NIST/academic research and applicable standards. All present explanatory chains are GNR until evidence-linked.