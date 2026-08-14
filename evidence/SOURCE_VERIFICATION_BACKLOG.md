# Source Verification Backlog — Knowledge Backbone V1

Status: ACTIVE — FINAL QA
Purpose: prevent backbone maturity from being confused with publication-ready evidence.

## 1. Rule

No episode-critical factual or normative claim becomes PODCAST READY merely because it appears in a NEAR PODCAST READY P2 package.

Every publishable claim must be classified, sourced, applicability-scoped and reviewed according to its evidence class.

Canonical pipeline:

Claim → Claim class → Required source authority → Applicability → Exact support → Quantitative check if applicable → Technical review → Episode source note → Publication status

## 2. Verification classes

### V1 — Normative / standards / regulatory claim
Examples:
- what ISO/IEC/ISA/ASTM/ASME/AIAG or another standard requires;
- required test/qualification/control behavior;
- legal/regulatory obligation;
- definitions presented as normative.

Required evidence:
- primary standard/regulator/standards-body source whenever accessible;
- exact edition/status;
- clause/table/figure or other precise location when publication use depends on it;
- jurisdiction and applicability statement;
- distinction between SHALL/requirement and guidance/recommendation.

Hard rule: secondary summaries may help discovery but must not silently become the authority for a normative claim.

### V2 — Authoritative technical guidance
Examples:
- NIST, NASA, FDA, FAA, GAO, government laboratory guidance;
- recognized industry-body technical manuals;
- authoritative manufacturer technical guidance where product-specific.

Required evidence:
- original publication/source;
- publication date/version;
- applicability boundary;
- separation of source statement from our synthesis.

### V3 — Quantitative engineering claim / worked example
Examples:
- takt, capacity, OEE, break-even, NPV, capability, yield, rework recursion;
- Sentinel Node numerical examples.

Required evidence:
- equations and units;
- input assumptions;
- source/evidence class for each non-invented input;
- independent arithmetic check;
- explicit label when numbers are pedagogical assumptions rather than measured industrial data;
- sensitivity where conclusion depends strongly on uncertain assumptions.

### V4 — Case-study factual claim
Examples:
- Samsung Note7 failure populations;
- Hydro cyber-attack production effects;
- Tesla Model 3 ramp facts;
- FDA warning-letter findings;
- Boeing system facts used in the systems/configuration stress test.

Required evidence:
- prefer regulator, company filing/report, official investigation or other primary record;
- exact date/time period;
- distinguish established fact from allegation, interpretation or later commentary;
- avoid causal claims stronger than the investigation/source supports;
- record what lesson is our synthesis rather than the source's conclusion.

### V5 — Academic / research claim
Examples:
- reliability relationships;
- process/material mechanisms;
- manufacturing/automation empirical findings.

Required evidence:
- peer-reviewed or otherwise technically credible source;
- method/population/context;
- limitations and transferability;
- avoid converting correlation or one study into a universal rule.

### V6 — GNR / canonical synthesis
Examples:
- Hardware Evolution Ladder;
- DEV/LVP/SVP Lens;
- QUALITY CHAIN 8;
- RAMP 10;
- ECON 10;
- SUPPLIER 10;
- AUTOMATE 10;
- TRACE/ATLAS/SECURITY listener tools.

Required treatment:
- label as our framework/synthesis unless directly adopted from a named source;
- every embedded factual/normative premise still inherits its own V1–V5 verification requirement;
- do not imply a framework is an ISO/IEC/AIAG requirement because its components are source-informed.

## 3. Priority tiers

### P0 — Publication blocker
Must be verified before an episode containing the claim is marked PODCAST READY:
- normative SHALL/required claims;
- safety-critical claims;
- regulatory/legal statements;
- numeric claims that drive a recommendation;
- causal claims in case studies;
- claims that determine pass/fail/release/requalification decisions.

### P1 — High-value technical support
Must normally be verified during episode research-pack preparation:
- recognized best practice;
- authoritative technical definitions;
- industrialization methodology;
- non-safety quantitative benchmarks;
- explanatory case facts.

### P2 — Context / enrichment
Can be verified during show-note/script finishing:
- historical context;
- non-decision anecdotes;
- optional examples;
- supporting statistics that do not drive the engineering conclusion.

## 4. Canonical verification record

Each verification item should capture:

| Field | Required |
|---|---|
| Claim ID | yes |
| P2/domain/episode mapping | yes |
| Claim text | yes |
| Claim class V1–V6 | yes |
| Priority P0–P2 | yes |
| Source title/owner | yes for V1–V5 |
| Primary-source URL/reference | yes where available |
| Edition/date/version | when applicable |
| Exact support location | required for P0 normative claims |
| Applicability statement | yes |
| Assumptions/units | quantitative claims |
| Source says vs synthesis says | yes |
| Verification owner/status | yes |
| Technical reviewer | before PODCAST READY |
| Episode source-note link | before publication |

Statuses:
`UNVERIFIED → SOURCE LOCATED → VERIFIED → TECHNICALLY REVIEWED → PACKAGED`

## 5. Backbone-level P0 verification backlog

### P2.01 — Readiness / hardware evolution
- NASA/GAO/manufacturing-readiness language used as authoritative support.
- Any formal readiness-level terminology presented as external rather than our DEV/LVP/SVP synthesis.

### P2.02 — Configuration & change control
- configuration identification/status accounting/change/effectivity claims attributed to NASA or formal CM guidance;
- regulatory/industry-specific change/requalification claims when used.

### P2.03 — Quality chain
- AIAG/APQP/Control Plan/PFMEA/MSA/SPC/PPAP normative or quasi-normative claims;
- capability-statistic conditions and interpretation;
- sample-size caveats and any threshold recommendation;
- measurement-system acceptance criteria if numeric thresholds are taught.

### P2.04 — Pilot / capacity / ramp
- external definitions of production readiness/run-at-rate where attributed;
- all Sentinel takt/capacity/rework calculations independently checked;
- distinguish our RAMP 10 gate from external requirements.

### P2.05 — Economics
- NPV/IRR/payback methodology support;
- all Sentinel cash-flow/break-even examples independently checked;
- assumptions explicitly pedagogical vs empirical;
- maintenance/economic empirical claims sourced.

### P2.06 — Supplier industrialization
- AIAG PPAP wording/applicability;
- FAI vs PPAP distinction;
- CQI-19/sub-tier/pass-through-characteristic claims;
- Nadcap examples clearly industry-specific;
- supplier-change/requalification decision tree labeled synthesis unless directly required.

### P2.07 — Automation / OEE / safety
- OEE formula/interpretation source;
- current editions/status/applicability for ISO 12100, ISO 13849 series, IEC 62061, ISO 10218 series, IEC 60204-1 and collaborative-operation references;
- jurisdictional legal statements separated from standards guidance;
- no “cobot=safe” implication;
- RELEASE 12 labeled synthesis.

### P2.08 — Manufacturing Atlas
- ISA-95/IEC 62264 hierarchy and information-model claims;
- OPC UA claims and companion-specification boundaries;
- Digital Thread claims sourced to NIST/authoritative references;
- our relational schema/object model explicitly labeled synthesis;
- Applicability Statement example verified against the selected concrete standard before being used as a standards example.

### P2.09 — OT/ICS cybersecurity
- current edition/status and scope of IEC 62443-2-1, 2-4, 3-2, 3-3, 4-1, 4-2;
- Asset Owner / service provider / product supplier responsibility statements;
- zones/conduits/security-level terminology;
- NIST SP 800-82 Rev.3 claims;
- distinguish our SECURE RELEASE 12/RACI from normative IEC 62443 content.

### P2.10 — Case studies
- Samsung Note7: investigation facts and supplier/failure-population wording;
- Norsk Hydro: timeline, production/manual-operation/recovery figures;
- Boeing 737 MAX: only claims required for interaction/system evidence lesson, sourced to official investigation/regulator records;
- Tesla Model 3: ramp, bottleneck, automation and production-rate claims sourced to SEC/company filings and clearly dated;
- FDA/Bioptimal: exact warning-letter findings and response context;
- every case lesson separated into FACT / SOURCE INTERPRETATION / OUR FRAMEWORK LESSON.

## 6. Cross-cutting repair verification

The nine case-study repairs must be treated as synthesis until separately sourced:

1. FIELD EVIDENCE LOOP
2. MINIMUM CONTROLLED PRODUCTION MODE
3. INTERACTION CLAIM
4. MOVING CONSTRAINT LOOP
5. STAGED CAPEX OPTION
6. INDUSTRIALIZATION SUPPLIER
7. EFFECTIVENESS EVIDENCE
8. SIGNAL AGGREGATION
9. FIELD EVENT

For each repair, episode packaging must identify:
- which observed cases motivated it;
- which authoritative sources independently support its underlying engineering premise;
- where it maps into the canonical backbone;
- whether it is a named external concept or our name for a synthesized concept.

## 7. Verification anti-patterns

Reject these during review:
- “ISO says…” without edition/applicability/location;
- citing a vendor blog for a standards requirement when the primary source is available;
- using a case-study article to claim universal causation;
- presenting Sentinel invented numbers as field data;
- treating a framework acronym created in this repository as an industry standard;
- quoting a requirement outside its product/jurisdiction/process scope;
- using a successful final test to erase earlier failures/rework history;
- allowing a weighted score to override a safety/regulatory/evidence hard stop.

## 8. Freeze criterion contributed by this backlog

Knowledge Backbone V1 may freeze before every item in this backlog is VERIFIED because freeze baselines the architecture, not every future episode source note.

However, freeze requires:
1. all P0 categories are identified;
2. no known normative claim is falsely marked verified;
3. source-vs-synthesis boundaries are explicit;
4. every future episode has a defined path from backbone claim to verification record;
5. unresolved source work is visible rather than hidden behind “COMPLETE”.

Podcast Ready requires the relevant P0 items to be VERIFIED + TECHNICALLY REVIEWED + PACKAGED.

## 9. Next QA step

Re-run the audience/stage coverage audit against the refined mission:
- Audience A: founders/developers/early hardware teams that need to understand what each discipline requires now and what production will demand later;
- Audience B: new production/industrialization teams moving from first prototype into controlled initial production while upgrading prototype solutions into industrial components/processes.

The audit must test DEV → LVP → SVP continuity, entry points, prerequisite burden, actionable tools and whether the 68-episode map serves both audiences without assuming hidden manufacturing knowledge.
