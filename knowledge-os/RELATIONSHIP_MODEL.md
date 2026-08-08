# Knowledge OS Relationship Model

**Baseline: v1.0**

## 1. Purpose

Relationships are first-class knowledge claims. A relationship must describe why two entities are connected, not merely that they are related.

Each relationship record contains:

```yaml
from:
relationship_type:
to:
inverse_type:
reason:
strength:
confidence:
provenance: [GNR]
evidence: []
applicable_context: []
assumptions: []
status:
```

AI-originated relationships retain `GNR` provenance permanently, even after external evidence is added.

## 2. Relationship Strength

- Mandatory — required dependency or normative link
- Strong — generally important or tightly coupled
- Medium — useful connection in many contexts
- Weak — contextual or optional connection
- Reference — navigational relationship with limited engineering dependency

## 3. Confidence

- High — direct authoritative evidence or well-established technical relationship
- Medium — multiple credible sources or strong professional consensus
- Low — plausible but insufficiently validated; research required

## 4. Controlled Relationship Vocabulary

### A. Knowledge Origin & Evidence

| Forward | Inverse | Meaning |
|---|---|---|
| DERIVED_FROM | SOURCE_FOR_DERIVATION | conclusion or artifact derived from another entity |
| BASED_ON | BASIS_FOR | method, concept or claim uses another as its foundation |
| INFERRED_FROM | SUPPORTS_INFERENCE | conclusion inferred rather than explicitly stated |
| SUPPORTED_BY | SUPPORTS | evidence supports a claim/object |
| VALIDATED_BY | VALIDATES_EVIDENCE_FOR | externally validated by evidence or method |
| CONTRADICTED_BY | CONTRADICTS | conflicting evidence or interpretation |
| SUMMARIZES | SUMMARIZED_BY | condensed representation of another source/object |
| QUOTES | QUOTED_BY | direct quoted support |
| INTERPRETS | INTERPRETED_BY | provides interpretation of source material |
| SUPERSEDES | SUPERSEDED_BY | newer authoritative replacement |

### B. Questions, Assumptions & Conflict

| Forward | Inverse | Meaning |
|---|---|---|
| ANSWERS_QUESTION | ANSWERED_BY | entity helps answer an Engineering Question |
| OPENS_QUESTION | OPENED_BY | evidence/claim reveals a new unresolved question |
| RESOLVES_QUESTION | RESOLVED_BY | evidence/claim closes an Open Question within stated scope |
| DEPENDS_ON_ASSUMPTION | ASSUMED_BY | conclusion/decision depends materially on an explicit assumption |
| PARTICIPATES_IN_CONFLICT | CONFLICT_CONTAINS | entity is one side/evidence element in a Knowledge Conflict |
| RESOLVES_CONFLICT | RESOLVED_BY | synthesis/evidence resolves a Knowledge Conflict within stated scope |

### C. Dependency & Lifecycle

| Forward | Inverse | Meaning |
|---|---|---|
| REQUIRES | REQUIRED_BY | cannot normally proceed without target |
| DEPENDS_ON | DEPENDENCY_OF | meaningful dependency, not always mandatory |
| PRECEDES | FOLLOWS | normally occurs earlier in a process/lifecycle |
| ENABLES | ENABLED_BY | makes another activity/capability possible |
| TRIGGERS | TRIGGERED_BY | causes initiation of another event/process |
| BLOCKS | BLOCKED_BY | prevents progress until condition is resolved |
| INPUT_TO | RECEIVES_INPUT_FROM | provides an input to another object |
| PRODUCES | PRODUCED_BY | generates an output/deliverable |
| CONSUMES | CONSUMED_BY | uses another object as input/resource |
| GATES | GATED_BY | defines a formal readiness/approval gate |

### D. Engineering Analysis & Design

| Forward | Inverse | Meaning |
|---|---|---|
| CALCULATES | CALCULATED_BY | calculates a quantity or result |
| MEASURES | MEASURED_BY | measures an attribute or phenomenon |
| ESTIMATES | ESTIMATED_BY | predicts/approximates a quantity |
| MODELS | MODELED_BY | represents behavior mathematically or physically |
| VERIFIES | VERIFIED_BY | checks conformance to specified requirements |
| VALIDATES | VALIDATED_BY_METHOD | demonstrates intended use/need is satisfied |
| ANALYZES | ANALYZED_BY | performs structured analysis |
| OPTIMIZES | OPTIMIZED_BY | improves target according to defined objective |
| CONTROLS | CONTROLLED_BY | regulates target behavior/process |
| MONITORS | MONITORED_BY | observes target over time |
| DETECTS | DETECTED_BY | identifies condition, feature or failure |
| MITIGATES | MITIGATED_BY | reduces risk or impact |

### E. Manufacturing & Assembly

| Forward | Inverse | Meaning |
|---|---|---|
| MANUFACTURES | MANUFACTURED_BY | process/equipment makes target |
| MACHINES | MACHINED_BY | removes material to make target |
| PRINTS | PRINTED_BY | additive process produces target |
| CUTS | CUT_BY | cutting process/equipment acts on target |
| FORMS | FORMED_BY | forming process creates geometry |
| JOINS | JOINED_BY | joining method connects target parts |
| ASSEMBLES | ASSEMBLED_BY | assembly process combines target |
| FIXTURES | FIXTURED_BY | fixture locates/restrains target |
| AUTOMATES | AUTOMATED_BY | automation performs target operation |
| INSPECTS | INSPECTED_BY | inspection evaluates target |
| TESTS | TESTED_BY | test method evaluates performance/conformance |
| CALIBRATES | CALIBRATED_BY | establishes measurement accuracy/traceability |
| REWORKS | REWORKED_BY | corrects nonconforming product/process |
| REPAIRS | REPAIRED_BY | restores function after failure/damage |
| MAINTAINS | MAINTAINED_BY | sustains equipment/process capability |

### F. Materials & Compatibility

| Forward | Inverse | Meaning |
|---|---|---|
| MADE_OF | USED_IN | object is composed of material |
| COMPATIBLE_WITH | COMPATIBLE_WITH | technically compatible under stated conditions |
| INCOMPATIBLE_WITH | INCOMPATIBLE_WITH | known incompatibility under stated conditions |
| PROCESSES_MATERIAL | PROCESSED_BY | process can act on material |
| REQUIRES_MATERIAL_PROPERTY | REQUIRED_BY_APPLICATION | property required for application/process |
| COATED_WITH | COATING_FOR | coating applied to target |
| BONDED_WITH | BONDING_AGENT_FOR | adhesive/bonding agent joins target |

### G. Quality, Risk & Documentation

| Forward | Inverse | Meaning |
|---|---|---|
| IDENTIFIES_RISK | RISK_IDENTIFIED_BY | method identifies risk/failure |
| CONTROLS_RISK | RISK_CONTROLLED_BY | control reduces/prevents risk |
| GENERATES_REQUIREMENT | REQUIREMENT_GENERATED_BY | creates a requirement |
| DOCUMENTED_BY | DOCUMENTS | information/process is formally documented by target |
| REFERENCES | REFERENCED_BY | formal or useful reference relationship |
| TRACES_TO | TRACED_FROM | traceability relationship |
| DEFINES_ACCEPTANCE_FOR | ACCEPTANCE_DEFINED_BY | defines acceptance/rejection criteria |
| NONCONFORMANCE_OF | HAS_NONCONFORMANCE | deviation belongs to product/process |
| CAUSES | CAUSED_BY | causal relationship supported by evidence |
| CONTRIBUTES_TO | CONTRIBUTED_TO_BY | contributory but not sole cause |

### H. Standards & Governance

| Forward | Inverse | Meaning |
|---|---|---|
| DEFINED_BY | DEFINES | term/process formally defined by target |
| REQUIRED_BY_STANDARD | REQUIRES_COMPLIANCE_WITH | normative requirement imposed by target |
| REGULATED_BY | REGULATES | legal/regulatory governance |
| RECOMMENDED_BY | RECOMMENDS | non-mandatory authoritative recommendation |
| PROHIBITED_BY | PROHIBITS | explicitly disallowed |
| EXEMPTED_BY | PROVIDES_EXEMPTION_FOR | exemption/exception relationship |
| COMPLIES_WITH | COMPLIED_WITH_BY | conformance relationship |

### I. Alternatives, Comparison & Selection

| Forward | Inverse | Meaning |
|---|---|---|
| ALTERNATIVE_TO | ALTERNATIVE_TO | viable alternative under some conditions |
| PREFERRED_OVER | LESS_PREFERRED_THAN | selection preference under stated criteria |
| REPLACES | REPLACED_BY | functional/process replacement |
| COMPLEMENTS | COMPLEMENTS | works together to improve outcome |
| COMPARED_WITH | COMPARED_WITH | explicit comparison pair |
| SUITABLE_FOR | SUITED_BY | appropriate for use case/application |
| UNSUITABLE_FOR | UNSUITED_BY | poor/invalid choice for use case/application |

### J. Organization & Responsibility

| Forward | Inverse | Meaning |
|---|---|---|
| OWNED_BY | OWNS | accountable owner |
| PERFORMED_BY | PERFORMS | activity normally executed by role/team/equipment |
| APPROVED_BY | APPROVES | formal approval authority |
| REVIEWED_BY | REVIEWS | reviewer relationship |
| HANDED_OFF_TO | RECEIVES_HANDOFF_FROM | transfer of responsibility/work |
| COLLABORATES_WITH | COLLABORATES_WITH | cross-functional collaboration |

### K. Podcast & Navigation

| Forward | Inverse | Meaning |
|---|---|---|
| EXPLAINED_IN | EXPLAINS | core topic explained in episode |
| EXPANDED_IN | EXPANDS | secondary/deeper treatment |
| PREREQUISITE_FOR | HAS_PREREQUISITE | prior knowledge recommended |
| TAGGED_WITH | TAGS | listener navigation tag |
| CASE_STUDY_FOR | USES_CASE_STUDY | case demonstrates concept |

## 5. Relationship Creation Rule

A relationship should be created when it conveys a statement that would still be meaningful if written as a sentence.

Bad: `CNC → related to → Aluminum`

Good: `CNC Milling → PROCESSES_MATERIAL → Aluminum Alloys`

## 6. Evidence Requirements

Relationships that imply regulation, causation, mandatory dependency, technical compatibility, performance, preference, chronology or conflict should carry evidence whenever possible.

Relationships used only for navigation may use Project Synthesis as evidence, but AI-originated navigation logic still retains `GNR` provenance.

## 7. Inverse Relationships

Every controlled relationship should define an inverse. Symmetric relationships use the same type in both directions.

Inverse relationships are logical views of the same claim and should not be treated as separate evidence unless implementation requires duplicate storage.

## 8. Conflict Handling

When sources conflict, do not delete one side. Create explicit `CONTRADICTED_BY` links and a Knowledge Conflict record when the disagreement is decision-relevant. Capture context, assumptions and applicability conditions.

## 9. Assumption Handling

If a relationship is true only under an assumption (for example annual volume, service environment or target tolerance), link that assumption explicitly using `DEPENDS_ON_ASSUMPTION` rather than hiding it in prose.

## 10. Context Matters

Compatibility, preference, suitability, causation and sequencing often depend on conditions. The relationship reason/applicable context must state important scope such as material, volume, tolerance, industry, regulatory context or lifecycle phase.

## 11. Architecture Freeze

Knowledge OS v1.0 freezes this controlled relationship model as the baseline. New relationship types should be added only when existing types cannot express a recurring engineering statement precisely, and material extensions require an ADR. Avoid vague relations such as `RELATED_TO`.