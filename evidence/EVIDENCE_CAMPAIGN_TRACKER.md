# Phase 2 — Evidence Campaign Tracker

status: ACTIVE
started_on: 2026-08-09

## Pass 1 — Breadth tracker

| Priority | Evidence package | Podcast leverage | Status |
|---|---|---|---|
| A0 | Early hardware development / Opening Arc | A1–A8 + bridge to Episodes 1–10 | IN PROGRESS — NEAR BREADTH COMPLETE |
| A1 | Product development / NPI / production readiness | Episodes 1–5 | IN PROGRESS |
| A2 | DFM / DFA / DFT foundations | Episodes 6–10 | QUEUED |
| A3 | Manufacturing process selection / lifecycle economics | Episode 11 + process arc | QUEUED |
| A4 | Quality foundations: PFMEA/control plan/MSA/SPC/capability | Episodes 23–24, 32 | QUEUED |
| A5 | Pilot/PVT/ramp/yield/capacity | Episodes 26–31 | QUEUED |
| A6 | Supplier industrialization / qualification / change control | Episodes 30, 37–40 | QUEUED |
| A7 | Automation business case / qualification / OEE | Episodes 41–46 | QUEUED |
| A8 | Manufacturing Data Hub standards / semantic integration | Episodes 47–52 | QUEUED |

## Current A0 findings
Primary-source backbone includes NASA Systems Engineering Handbook material on requirements, architecture, interfaces, V&V, test-article pedigree and configuration management, plus TRL material for prototype maturity boundaries.

Commercial corroboration includes official embedded/electronics guidance plus KiCad's native Git integration, which gives us a practical lightweight implementation pattern for early hardware configuration control.

NISTIR 7922 now provides a stronger cross-industry basis for the claim that engineering changes can force previously completed decisions/tasks to be revisited and can create substantial cost after build/delivery. We are explicitly rejecting folklore “10x/100x cost-of-change” multipliers unless independently evidenced.

Important applicability rule: the Opening Arc must not copy aerospace bureaucracy into startups. It should extract the engineering intent and scale the implementation for DEV, LVP and SVP.

Current remaining A0 gaps:
- mechanical prototype-to-production commercial case studies
- prototype representativeness outside aerospace
- stronger primary evidence for firmware/hardware co-configuration
- regulatory/product-safety discovery timing by product class
- empirical evidence specifically tying prototype-route choices to downstream manufacturing debt

## Current A1 findings
Primary-source backbone includes NASA TRL, NASA Production Readiness Review, NASA MRL material and NIST NPI/production-line research. Industry EVT/DVT/PVT terminology is treated separately from normative readiness frameworks.

## Campaign rule
Breadth pass does not attempt exhaustive research. Each package must first identify:
1. authoritative source families;
2. episode-critical claims;
3. claims with weak/GNR evidence;
4. applicability conflicts;
5. Pass-2 depth targets.

## Promotion rule
A package moves from IN PROGRESS to BREADTH COMPLETE only when all five items above are represented and the strongest primary sources are captured or explicitly unavailable.

## Immediate sequence
1. Finish remaining A0 breadth gaps.
2. Promote A0 to BREADTH COMPLETE.
3. Reconcile A0 findings into A1 where the bridge reaches production intent.
4. Continue to A2 — DFM / DFA / DFT foundations.