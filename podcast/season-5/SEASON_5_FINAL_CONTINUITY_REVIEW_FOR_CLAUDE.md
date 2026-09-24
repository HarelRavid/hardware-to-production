# Season 5 — Final Continuity Review for Claude Handoff

status: PASS — READY FOR HANDOFF MANIFEST / CLAUDE PROMPT GENERATION
review_date: 2026-09-19
scope: EP41–EP52
governed_by:
- podcast/OFFICIAL_PODCAST_DELIVERY_ROADMAP.md
- podcast/CLAUDE_EPISODE_HANDOFF_CONTRACT.md
review_type: final season continuity / duplicate ownership / two-character narrative / handoff-readiness review

## 1. Decision

Season 5 is technically and editorially coherent after the Wave 04 and Wave 05 publication packages.

No new research wave or architecture change is required before Claude handoff.

Result:
**PASS TO HANDOFF GENERATION.**

## 2. Final listener journey

EP41 When Not to Automate
→ EP42 Automation Business Case
→ EP43 Semi-Automation / Robotics / Vision
→ EP44 Automated Inspection / EOL Test
→ EP45 Automation Qualification / OEE / Maintenance
→ EP46 Scaling Without Automating Defects
→ EP47 Systems of Record
→ EP48 Product Genealogy / Recipes / Parameters / Measurements
→ EP49 Standards / Claims / Evidence Knowledge Graph
→ EP50 Manufacturing Atlas Decision System
→ EP51 OPC UA / ISA-95 / Semantic Integration
→ EP52 Engineering-Grade Manufacturing Data / OT Security

The season first asks whether and how to automate a controlled production system, then asks how to connect its information without losing engineering meaning, authority or security.

## 3. Two-character narrative strategy

Oz:
Lead Host / Systems Engineer.

Rona:
Practitioner / Challenger.

Season 5 challenge style:
- B pushes back on automation hype, software buzzwords and cyber overreach.
- A narrows the decision to process maturity, evidence, economics and consequence.
- B tests each framework on a realistic production scenario.
- both Oz and Rona keep physical production consequences visible even in data/semantic episodes.

B should repeatedly ask:
- “What problem are we actually solving?”
- “Does this improve accepted output or just a dashboard metric?”
- “Who owns the truth?”
- “What happens when this system fails or writes back?”

## 4. Automation arc ownership

### EP41
Owns:
whether automation is justified at all.

Must not:
- become anti-automation ideology;
- duplicate full economics of EP42;
- prescribe a maturity score.

### EP42
Owns:
business case / lifecycle economics / sensitivity / staged CAPEX.

Must not:
- treat payback alone as decision authority;
- duplicate general process-economics episode depth unnecessarily;
- assume labor reduction, uptime or yield improvement.

### EP43
Owns:
function-level automation boundary, robotics and machine vision.

Must not:
- say “cobot = safe”;
- treat robot repeatability as process capability;
- become machinery-safety standards course.

### EP44
Owns:
automated inspection/test as measurement/release decision system.

Must not:
- duplicate Wave 02 MSA depth;
- treat 100% test as zero escape risk;
- allow retest-to-pass logic to erase failure history.

### EP45
Owns:
automation acceptance / qualification / OEE / maintenance / recovery.

Must not:
- treat FAT/SAT as production capability;
- treat OEE as root cause or system capacity;
- use universal OEE benchmark.

### EP46
Owns:
scale-readiness and replicated-cell equivalence.

Must not:
- assume identical equipment = equivalent process;
- assume two cells = double accepted throughput;
- duplicate EP45 maintenance depth.

## 5. Connected-manufacturing arc ownership

### EP47
Owns:
information-object authority / systems-of-record boundaries.

Must not:
- prescribe one mandatory PLM/ERP/MES stack;
- use ISA-95 as cyber segmentation.

### EP48
Owns:
physical/unit production genealogy with recipe/parameter/measurement context.

Must not:
- duplicate EP35’s quality/affected-population principle;
- imply serial number alone is genealogy;
- turn UUID into provenance.

### EP49
Owns:
claim/source/evidence/applicability relationships.

Must not:
- require graph database;
- treat AI/search confidence as evidence maturity;
- reproduce protected standards text.

### EP50
Owns:
context-aware decision workflow through Manufacturing Atlas.

Must not:
- present Atlas as external standard;
- allow weighted scores to override hard stops;
- turn Atlas into competing master-data system.

### EP51
Owns:
semantic integration, ISA-95 context and OPC UA information-model boundary.

Must not:
- equate connectivity with semantics;
- equate ISA-95 levels with security zones;
- imply protocol security = OT security.

### EP52
Owns:
decision-grade manufacturing datasets plus OT security/recovery.

Must not:
- prescribe one IEC 62443 topology/security level;
- say read-only = safe;
- reduce OT security to RBAC;
- call machine restart full manufacturing recovery.

## 6. Cross-episode callback map

EP41 → EP42:
technical readiness does not answer whether investment is rational.

EP42 → EP43:
business case sets the automation opportunity; EP43 chooses the right function boundary.

EP43 → EP44:
automation of work becomes automation of quality/release decisions.

EP44 → EP45:
trustworthy automated decision needs qualified/sustainable equipment.

EP45 → EP46:
one stable cell is not automatically a scalable fleet.

EP46 → EP47:
once physical production scales, information ownership becomes a production-control problem.

EP47 → EP48:
system ownership must support reconstructable product history.

EP48 → EP49:
physical history becomes useful when linked to engineering claims/evidence.

EP49 → EP50:
linked knowledge becomes a decision system.

EP50 → EP51:
decision system needs semantic integration across authoritative sources.

EP51 → EP52:
meaningful connectivity must also be fit for engineering use and controlled in OT.

## 7. Terminology lock

Use consistently:
- automation readiness;
- technical feasibility;
- accepted sustainable throughput;
- OEE as loss lens;
- abnormal state / recovery;
- system of record;
- genealogy;
- durable identity;
- claim / evidence / applicability;
- Manufacturing Atlas;
- semantic integration;
- read-only vs write-back authority;
- OT / IACS;
- trustworthy production recovery.

Avoid:
- “smart factory” as maturity label;
- “world-class OEE”;
- “single source of truth” without object/authority context;
- “digital thread” as marketing synonym;
- “secure because encrypted.”

## 8. Standards / source strategy

Season 5 contains many named standards but the audio should remain decision-first.

Use current source locks for:
- machinery risk/safety context;
- robot/application safety;
- OEE open-source definition;
- ISA-95 public integration context;
- OPC UA public architecture;
- NIST digital thread/traceability;
- NIST SP 800-82;
- IEC 62443 public role/system boundaries.

Exact clause-level design/security requirements remain out of generic narration.

## 9. Revision-watch controls

At final dialogue/publication freeze:
- recheck ISO 12100 revision status if materially named;
- recheck ISO 13849-2 revision status if materially named;
- recheck IEC 62061 current consolidated edition;
- recheck ISO/TS 15066 replacement status if materially named;
- recheck IEC 62443-2-1:2024 current status;
- recheck NIST SP 800-82 current-final status.

Draft/revision projects must never be treated as published normative authority.

## 10. Quantitative continuity

EP42:
only audited lifecycle-economic examples/assumptions.

EP45:
locked Sentinel OEE arithmetic may be used:
Availability 90.00%;
Performance ≈93.25397%;
Quality ≈95.95745%;
OEE ≈80.53571%.

Equal-OEE example:
80.3682% from different loss structures.

EP46:
capacity/replication examples must preserve accepted-throughput and moving-constraint logic.

No universal benchmark/threshold.

## 11. Audio density and visuals

EP43:
robot/task/vision boundary diagram.

EP44:
test architecture / drift / false-pass-fail flow.

EP45:
OEE decomposition / recovery-state diagram.

EP46:
replication-equivalence matrix.

EP47:
system-of-record object map.

EP48:
Unit Evidence Thread.

EP49:
source → claim → applicability → evidence graph.

EP50:
ATLAS 10 decision path.

EP51:
context-to-data semantic map.

EP52:
secure data path / trust-boundary diagram.

Claude should not overexplain spatial/architecture visuals in audio.

## 12. Source/evidence state

EP41–46:
Wave 04 packages PASS.

EP47–52:
Wave 05 packages PASS.

All twelve have:
- claim locks;
- technical reviews;
- outlines;
- full draft references;
- script reviews;
- source notes.

Existing drafts are reference material only under the current handoff authority hierarchy.

## 13. Handoff-generation decision

**SEASON 5 FINAL CONTINUITY REVIEW: PASS**

Next:
1. create 12 Handoff Manifests;
2. create 12 Claude Writing Prompts;
3. validate paths;
4. run Season 5 exit audit;
5. advance to Season 6.
