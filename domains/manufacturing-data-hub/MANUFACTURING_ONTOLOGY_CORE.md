# 9.1 Manufacturing Ontology — Core Model

status: Researching
provenance: [GNR]

## Purpose
Define a stable semantic backbone that can connect manufacturing knowledge to product/process/resource/execution data without making application databases the ontology.

## Core entity classes
### Product/configuration
- Product
- Product Revision
- Part
- Part Revision
- Assembly
- BOM / EBOM / MBOM
- Configuration / Variant
- Requirement / CTQ

### Material/supply
- Material Specification
- Material Lot / Heat / Batch
- Purchased Part Lot
- Supplier
- Supplier Site
- Sub-tier Source
- Certificate / Supplier Evidence

### Process
- Manufacturing Process
- Process Definition
- Routing
- Operation Definition
- Operation Execution
- Recipe
- Recipe Revision
- Process Parameter Definition
- Process Parameter Value/Observation
- Intermediate Product State

### Resource
- Equipment Class
- Equipment Asset
- Tool / Fixture / Gauge
- Tool Revision
- Work Center
- Production Line / Cell
- Facility / Site
- Human Resource / Role
- Qualification / Authorization

### Quality
- Characteristic
- Measurement Definition
- Measurement Result
- Test Definition
- Test Execution
- Inspection
- Defect / Failure Mode
- Nonconformance
- Disposition
- Rework
- Deviation / Concession
- Quality Gate / Release

### Lifecycle/change
- Engineering Change
- Effectivity
- Qualification
- Calibration
- Maintenance Event
- Downtime Event
- Process Excursion

### Knowledge/evidence
- Knowledge Object
- Engineering Claim
- Engineering Decision
- Decision Instance
- Standard / Requirement
- Source / Evidence
- Assumption
- Open Question
- Knowledge Conflict

## Identity principle
Every durable semantic object requires stable identity independent of display name, file path or source-system key. Source-system identifiers are mappings, not ontology identity.

## Relationship examples
ProductRevision --hasMBOM--> MBOM
MBOM --requires--> PartRevision
Routing --contains--> OperationDefinition
OperationExecution --instantiates--> OperationDefinition
OperationExecution --transforms--> IntermediateProductState
OperationExecution --uses--> EquipmentAsset
OperationExecution --uses--> ToolRevision
OperationExecution --applies--> RecipeRevision
OperationExecution --consumes--> MaterialLot
OperationExecution --performedBy--> Person/Role
MeasurementResult --measures--> Characteristic
MeasurementResult --producedBy--> MeasurementSystem
Nonconformance --detectedAt--> OperationExecution
Nonconformance --suspectedCreatedAt--> OperationExecution
SerialUnit --hasGenealogyEvent--> OperationExecution
Claim --supportedBy--> Evidence
DecisionInstance --uses--> Claims / Assumptions / Observations

## Semantic anti-patterns
- one generic `document` entity for every controlled object
- one generic `event` without typed semantics
- encoding revisions only in filenames
- overwriting historical values
- using free-text supplier/equipment/process names as identity
- storing a current recipe without recording the revision used historically
- representing rework only as a note rather than an execution path

## Decision object
### D-DH-ONTO-001 — Is a concept a durable semantic object, an attribute, a relationship, an event/execution or only a navigation label?

## Integrity rule
Create ontology objects because they support distinct identity, evidence, lifecycle or decisions — not because a database table happens to exist.