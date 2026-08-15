# A2 Research Pack — Hardware Team Map: Which Disciplines Do You Actually Need?

status: CLAIM SET STABLE
season: Season 1 — Build the Right Thing
primary_audience: Audience A — founders / early hardware development teams
secondary_audience: engineering managers, technical co-founders, first hires, NPI leads
lifecycle: DEV-FIRST / CROSS-STAGE
entry_point: PRIMARY FOUNDATION / STANDALONE WITH LIGHT RECAP
technical_depth: foundation

## 1. Episode promise
Help an early hardware team identify the disciplines, ownership boundaries and missing capabilities required to turn a concept into a coordinated product-development program.

Canonical listener question:
> Who actually needs to own what, and which missing discipline will become an expensive integration problem later?

The episode prevents two opposite errors:
1. hiring a large organization before the work justifies it; and
2. assuming one strong generalist can permanently absorb every discipline without explicit ownership or review.

## 2. Navigation card
**You are here:** Requirements → Team/ownership → Architecture/interfaces.

**Best for:** founder, CTO, first hardware engineer, small multidisciplinary startup team.

**You should already know:** basic product intent. A1 helpful, not mandatory.

**You will leave with:** Hardware Discipline Map + Ownership Gap Review.

**Prototype shortcut:** one person may cover multiple disciplines in early DEV.

**Shortcut expires when:** critical decisions, interfaces, safety/compliance, supplier transfer, verification or production controls depend on expertise nobody explicitly owns or reviews.

**Next:** A3 System Architecture & Interfaces → A4 Prototype Technologies → A5/A6 serious prototypes.

## 3. Audience contract
### DEV takeaway
Map the work before hiring for job titles. One person can wear many hats, but each important engineering responsibility still needs an owner.

### Prototype shortcut
Use generalists and external specialists selectively while uncertainty is high.

### Shortcut expiration
When a decision becomes safety-critical, architecture-defining, supplier-facing, irreversible or qualification-driving, ownership and competence must become explicit.

### LVP change
NPI, manufacturing, quality, supplier and test responsibilities become first-class rather than “engineering support.”

### SVP evidence
Clear authority, change ownership, release responsibility and specialist competence must support repeatable production and field learning.

### Manufacturing-debt prevention
Do not let critical disciplines exist only as undocumented knowledge inside one founder or contractor relationship.

### Listener action
Create a one-page ownership map for the current product and mark RED any discipline with critical decisions but no explicit owner/reviewer.

## 4. Core discipline map
The exact team varies by product, but a general hardware program may need responsibility for:
- systems/product requirements;
- mechanical design;
- materials/process selection;
- electronics/PCB;
- embedded firmware/software;
- power/thermal;
- sensing/control;
- industrial/design-for-use factors;
- verification/test;
- reliability;
- safety/compliance/regulatory;
- manufacturing/process engineering;
- quality/metrology;
- supplier engineering/supply chain;
- configuration/change control;
- service/field support;
- manufacturing data/traceability as maturity increases.

This is a responsibility map, not a mandatory org chart.

## 5. Stable claim register
| ID | Claim | Class | Priority | Status | Publication note |
|---|---|---|---|---|---|
| A2-C01 | Hardware development is multidisciplinary; consequential responsibilities should be visible and owned even when one person covers several disciplines. | V6 + V2 | P0 | CLAIM STABLE / SOURCE VERIFICATION OPEN | Source support should establish multidisciplinary systems-engineering logic, not prescribe our discipline list. |
| A2-C02 | Mapping decisions, interfaces, evidence and release responsibility is more useful for an early team than assuming job titles uniquely define ownership. | V6 | P0 | SYNTHESIS STABLE | Internal practical thesis. |
| A2-C03 | Cross-discipline gaps commonly become visible at interfaces, integration and verification boundaries. | V6 + A3 | P1 | SYNTHESIS STABLE | A3 owns the technical depth. |
| A2-C04 | Generalists and external specialists are legitimate in DEV if critical ownership, review and integration remain explicit. | V6 | P1 | SYNTHESIS STABLE | No universal staffing prescription. |
| A2-C05 | Manufacturing, quality, supplier and test responsibility should enter while design decisions are still shaping process, sourcing, test and industrialization—not only after a prototype is declared complete. | V6 + P2.01/P2.06 | P0 | BACKBONE-SUPPORTED / STABLE | Timing remains product-specific. |
| A2-C06 | Safety/compliance responsibility must be explicitly scoped to product, risk and jurisdiction rather than deferred to an unnamed future owner. | V6 + V2 | P0 | CLAIM STABLE / APPLICABILITY VERIFICATION OPEN | Avoid legal/professional-licensure claims without jurisdiction. |
| A2-C07 | Work may be outsourced, but the product team still needs ownership of integration, acceptance and downstream consequences. | V6 | P1 | SYNTHESIS STABLE | Contractor/supplier lesson. |
| A2-C08 | DEV→LVP→SVP increases the importance of release, process, supplier, quality, configuration and field accountability. | V6 | P1 | SYNTHESIS STABLE | Internal lifecycle lens. |

Core claims: 8. Open P0 source items: 2 families (multidisciplinary systems-engineering support; product-specific safety/compliance applicability).

## 6. Listener tool — Hardware Discipline Map
For each discipline/responsibility capture:
| Field | Question |
|---|---|
| Responsibility | What work/decision must exist? |
| Current owner | Who owns it now? |
| Reviewer/backup | Who can challenge or cover it? |
| Current maturity | DEV / LVP / SVP relevance |
| Critical interfaces | Which other disciplines depend on it? |
| Evidence owned | What proof/output does this role create? |
| External support | Consultant/lab/supplier needed? |
| Expiration trigger | When is current coverage no longer adequate? |

## 7. Ownership Gap Review
Mark a gap RED when any of these are true:
1. architecture-critical decision with no owner;
2. safety/compliance assumption with no competent review;
3. supplier/process decision whose downstream owner is absent;
4. verification activity nobody owns end-to-end;
5. change decision has no authority/effectivity owner;
6. production release depends on undocumented founder knowledge;
7. one contractor owns a critical subsystem but no internal person owns integration/evidence.

## 8. Worked example — Sentinel Node team evolution
### Early DEV
One technical founder may own system, firmware and electronics; mechanical may be contractor-supported.

Potential hidden gaps:
- environmental/sealing assumptions;
- production test strategy;
- supplier lifecycle;
- calibration ownership;
- regulatory/EMC planning.

### Serious prototype
Need becomes explicit for:
- interface owner across PCB/enclosure/connector;
- verification owner;
- firmware/hardware configuration identity;
- compliance watchlist.

### LVP transition
Manufacturing/process, quality, supplier and test ownership become direct contributors to design/change decisions.

Lesson: the organization grows because evidence and interfaces grow, not because a maturity chart demands job titles.

## 9. Boundary with A3
A2 owns **responsibility visibility**: who owns a decision/evidence boundary and when current coverage expires.

A3 owns **interface technical definition**: what crosses the boundary, what variation/states matter and how compatibility is demonstrated.

A2 should not become an interface-engineering episode; A3 should not become an org-design episode.

## 10. Common failure modes
- Founder owns everything implicitly; nobody can reconstruct decisions.
- Mechanical/electrical teams optimize locally and discover connector/thermal/service conflict late.
- Compliance is treated as a certification purchase rather than architecture input.
- Supplier is asked to “make it manufacturable” without product/process ownership on the buyer side.
- Quality is hired after pilot and inherits undocumented acceptance logic.
- NPI becomes a late handoff instead of a development participant.

## 11. Applicability statement
This episode provides a general hardware responsibility map. It does not prescribe a universal team size, reporting structure, professional licensure model or regulated-industry staffing requirement. Actual required competence and sign-off depend on product, jurisdiction, risk and contractual obligations.

## 12. What this episode must NOT claim
- every startup needs a specialist for every discipline immediately;
- one job title maps to one discipline;
- NPI/manufacturing should control early product design;
- consultants are inherently risky;
- a RACI chart alone solves ownership;
- the listed discipline taxonomy is an external standard.

## 13. Evidence backlog after claim stabilization
Before EVIDENCE VERIFIED:
1. Attach authoritative systems-engineering support for multidisciplinary development and responsibility/interface management.
2. Verify any safety/compliance examples only in their product/jurisdiction context.
3. Technical review from startup CTO + NPI perspective.
4. Do not add a case study unless it improves the ownership lesson without adding unnecessary narrative burden.

## 14. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: LOW
Quantitative burden: LOW
Backbone risk: LOW
Claim set: STABLE
Source verification: CONTROLLED BACKLOG

Next status target:
`CLAIM SET STABLE → EVIDENCE VERIFIED`
