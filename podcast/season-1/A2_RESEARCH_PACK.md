# A2 Research Pack — Hardware Team Map: Which Disciplines Do You Actually Need?

status: RESEARCH PACK OPEN
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

The episode should prevent two opposite errors:
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

## 5. Claim register — draft
| ID | Claim | Class | Priority | Status | Note |
|---|---|---|---|---|---|
| A2-C01 | Hardware development is inherently multidisciplinary, and important responsibilities should have explicit ownership even when one person covers multiple disciplines. | V6 + V2/V5 | P0 | OPEN | General systems-engineering support useful. |
| A2-C02 | Org-chart titles are less useful than mapping decisions, interfaces, evidence and release responsibilities. | V6 | P0 | SYNTHESIS | Core practical thesis. |
| A2-C03 | Cross-discipline gaps often appear first at interfaces and verification boundaries rather than inside one component. | V5/V6 | P1 | OPEN | Link A3. |
| A2-C04 | Early teams can legitimately use generalists/external specialists, provided critical ownership and review remain visible. | V6 | P1 | SYNTHESIS | Avoid universal staffing prescriptions. |
| A2-C05 | Manufacturing, quality and supplier disciplines should enter before production launch when design decisions start constraining process, test, sourcing or industrialization. | V6 + P2.01/P2.06 | P0 | BACKBONE-SUPPORTED | Timing varies by product. |
| A2-C06 | Safety/regulatory responsibility cannot be inferred from “someone in engineering will handle it later.” | V2/V6 | P0 | OPEN | Product/jurisdiction applicability required. |
| A2-C07 | A decision can be outsourced; accountability for integrating its consequences cannot disappear. | V6 | P1 | SYNTHESIS | Useful contractor/consultant lesson. |
| A2-C08 | As teams move DEV→LVP→SVP, ownership shifts from learning/architecture toward release, process, supplier, quality and field accountability. | V6 | P1 | SYNTHESIS | DEV/LVP/SVP lens. |

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

## 9. Common failure modes
- Founder owns everything implicitly; nobody can reconstruct decisions.
- Mechanical/electrical teams optimize locally and discover connector/thermal/service conflict late.
- Compliance is treated as a certification purchase rather than architecture input.
- Supplier is asked to “make it manufacturable” without product/process ownership on the buyer side.
- Quality is hired after pilot and inherits undocumented acceptance logic.
- NPI becomes a late handoff instead of a development participant.

## 10. Applicability statement
This episode provides a general hardware responsibility map. It does not prescribe a universal team size, reporting structure, professional licensure model or regulated-industry staffing requirement. Actual required competence and sign-off depend on product, jurisdiction, risk and contractual obligations.

## 11. What this episode must NOT claim
- every startup needs a specialist for every discipline immediately;
- one job title maps to one discipline;
- NPI/manufacturing should control early product design;
- consultants are inherently risky;
- a RACI chart alone solves ownership;
- the listed discipline taxonomy is an external standard.

## 12. Research backlog before CLAIM SET STABLE
1. Add authoritative systems-engineering support for multidisciplinary responsibility/interface ownership.
2. Cross-check overlap with A3 so interfaces are not duplicated.
3. Validate LVP timing against P2.01 industrialization lifecycle.
4. Add one credible case/anonymized failure only if it improves narrative value.
5. Technical review from startup CTO + NPI perspective.

## 13. Current assessment
Episode structure: STRONG
Audience fit: STRONG
Navigation fit: STRONG
Standards burden: LOW
Quantitative burden: LOW
Backbone risk: LOW
Source verification: OPEN

Next status target:
`RESEARCH PACK OPEN → CLAIM SET STABLE`
