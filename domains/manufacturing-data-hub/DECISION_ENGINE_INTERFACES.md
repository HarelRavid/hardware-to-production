# 9.10 Decision-Engine Interfaces

status: Researching
provenance: [GNR]

## Purpose
Define how structured manufacturing knowledge and operational evidence can support engineering decisions without hiding assumptions, uncertainty or human accountability.

## Decision-engine input classes
- engineering question
- product/material/process context
- assumptions
- constraints
- candidate options
- Knowledge Objects
- Engineering Claims
- Standards/requirements
- operational observations
- supplier/resource capability
- cost/lead-time data
- open questions/conflicts

## Output contract
A decision-support response should return:
- decision/question ID
- interpreted context
- assumptions used
- candidate options
- relevant constraints
- supporting claims/evidence
- contradicting/conflicting evidence
- applicability limits
- operational evidence where relevant
- tradeoffs
- recommended next evidence/action
- confidence/evidence maturity
- human approval/owner boundary

## Decision Instance
A Decision Model is reusable logic. A Decision Instance records a specific application at a specific time with actual inputs/evidence and resulting disposition.

DecisionInstance -> instantiates -> EngineeringDecision
DecisionInstance -> uses -> Assumptions
DecisionInstance -> uses -> Claims/Evidence
DecisionInstance -> considers -> CandidateOptions
DecisionInstance -> records -> Outcome
DecisionInstance -> approvedBy -> Role/Person
DecisionInstance -> hasEffectivity -> Product/Process scope

## Engine modes
- navigation: find relevant knowledge
- comparison: structure candidate tradeoffs
- diagnostic: trace failure/defect hypotheses
- readiness: evaluate gate criteria/evidence gaps
- change impact: identify affected objects/evidence
- recommendation: propose options with explicit evidence and assumptions

## Guardrails
- AI synthesis cannot silently elevate GNR to verified knowledge;
- operational correlation cannot be promoted to causation without evidence;
- missing inputs should be surfaced rather than filled with hidden assumptions;
- normative requirements must preserve revision/applicability;
- a recommendation should preserve rejected alternatives and rationale where important;
- high-consequence decisions require explicit human ownership/approval.

## Decision objects
### D-DH-DE-001 — Which knowledge/evidence inputs are required for this decision class?
### D-DH-DE-002 — What evidence gap blocks a stronger recommendation?
### D-DH-DE-003 — Is this output navigation, analysis, recommendation or controlled approval?

## Integrity principle
The Decision Engine supports engineering judgment; it does not erase the distinction between evidence, inference and authority.