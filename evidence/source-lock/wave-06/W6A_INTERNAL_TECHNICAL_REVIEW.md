# Wave 06A Internal Technical Review — EP11

status: PASS TO SCRIPT OUTLINE WITH PROCESS-FAMILY GUARDRAILS
review_date: 2026-09-19
reviewer_type: internal technical/editorial review; independent external human review not claimed

inputs:
- SOURCE_LOCK_WAVE_06A_PROCESS_SELECTION_REGISTER.md
- W6A_EP11_CLAIM_LOCK.md
- EP11 Production Blueprint
- DFX source map
- Wave 03 economics
- Waves 01/02/03 capability/representativeness dependencies

## Decision

EP11 can advance to script outline without using unsourced process-family limits.

## Technical findings

### Process selection timing
PASS.
NIST directly supports early manufacturability/process/cost integration.

### Material/process coupling
PASS.
Do not allow an episode section that chooses material first and process later as independent decisions unless the product context genuinely permits it.

### Multi-attribute decision
PASS.
Do not present one weighted score as engineering truth; hard constraints remain non-compensable.

### Process chain
PASS.
Primary process alone is insufficient where secondary operations/inspection/state transformations materially affect final part.

### Economics
PASS.
Use Wave 03 system boundary and accepted-good-output logic.
Do not treat NIST Manufacturing Cost Guide as direct part-level calculator.

### Bridge process
PASS as internal lifecycle synthesis.
No universal quantity threshold.

### Prototype-to-production transfer
PASS.
Example must say which claims transfer and which production mechanisms remain unrepresented.

## Required script guards

1. no generic “injection molding above N units” rule;
2. no generic “CNC is for low volume” absolute;
3. no process tolerance or roughness values;
4. no single material/process ranking algorithm;
5. no supplier brochure capability as release evidence;
6. no assumption that mass-production route is more mature by definition;
7. no assumption process-selection decision is one-time; changes in volume/design/supply can reopen it.

## Boundary with EP12–19

EP11 owns:
- decision dimensions;
- evidence/economic envelope;
- bridge-route logic;
- process-chain thinking.

EP12–18 own:
- process physics;
- material state;
- defect mechanisms;
- detailed DFM/inspection/qualification.

EP19 owns:
- sequencing/interactions across operations.

Result: PASS — no overlap requiring merge.

**WAVE 06A INTERNAL TECHNICAL REVIEW: PASS**
