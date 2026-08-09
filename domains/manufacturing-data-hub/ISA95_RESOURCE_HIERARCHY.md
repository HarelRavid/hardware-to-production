# 9.2–9.3 ISA-95 Alignment & Equipment/Resource Model

status: Researching
provenance: [GNR]

## Purpose
Provide a manufacturing hierarchy that can map operational data consistently from enterprise/site level down to specific work centers, equipment assets, tooling and human resources without forcing every organization into one physical layout.

## ISA-95 / IEC 62264 alignment boundary
The Atlas should be able to map common hierarchy concepts such as:
- Enterprise
- Site
- Area
- Work Center / Line / Cell
- Work Unit / Equipment Asset

The exact hierarchy depth is implementation-specific; semantic meaning matters more than matching a fixed folder depth.

## Resource classes
### Equipment
- Equipment Class
- Equipment Asset
- Machine
- Furnace
- Robot
- Test Station
- Inspection Station
- Utility/Support Equipment boundary

### Tooling
- Tool
- Fixture
- Jig
- Gauge
- Mold/Die
- End Effector
- Consumable Tool boundary

### Human
- Person
- Role
- Skill
- Qualification
- Authorization
- Shift/Team boundary

### Spatial/organizational
- Enterprise
- Site
- Building/Area
- Line/Cell
- Work Center
- Storage/Supermarket boundary

## Type vs instance
Equipment Class -> Equipment Asset
Tool Type -> Tool Revision/Instance
Role -> Person assignment
Qualification Definition -> Qualification Instance

## Resource state objects
- available/unavailable
- qualified/unqualified
- maintenance due
- calibration due
- faulted
- changeover/setup state
- current recipe/product boundary
- utilization/downtime event

## Core relationships
Site --contains--> Area
Area --contains--> WorkCenter
WorkCenter --contains/uses--> EquipmentAsset
OperationDefinition --requiresResourceClass--> EquipmentClass/Role/ToolType
OperationExecution --uses--> EquipmentAsset/ToolRevision/Person
EquipmentAsset --hasMaintenanceEvent--> MaintenanceEvent
EquipmentAsset --hasQualification--> Qualification
Person --hasQualification--> QualificationInstance

## Engineering principle
The Atlas must distinguish what an operation requires from what resource actually executed it. This enables capability, genealogy, authorization and substitution analysis.

## Decision objects
### D-DH-HIER-001 — What hierarchy is needed for this site/process without creating artificial levels?
### D-DH-RES-001 — Which resource properties belong to class/type versus asset/instance?
### D-DH-SUB-001 — When are two resources truly interchangeable for a manufacturing decision?

## Integrity rule
Do not treat identical equipment model numbers as equivalent qualified resources without preserving site, configuration, qualification and maintenance state.