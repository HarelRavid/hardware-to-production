# Section 8 — Automation & Scale — Domain Map

status: Researching
provenance: [GNR]

## Scope
Decision and engineering architecture for scaling manufacturing through semi-automation, robotics, machine vision, automated inspection/test, end-of-line systems and supporting maintenance/OEE infrastructure without automating unstable processes.

## WBS
8.1 When not to automate
8.2 Automation business case
8.3 Semi-automation
8.4 Robotics/cobots
8.5 Machine vision
8.6 Automated inspection/test
8.7 End-of-line systems
8.8 Automation qualification
8.9 OEE / maintenance / spare strategy
8.10 Scaling without automating defects

## Core state model
Manual stable process -> assisted/semi-automated process -> qualified automated cell -> integrated line/system -> monitored scalable production.

## Engineering principle
Automation should remove or control validated work content and variation. Automating an unstable or poorly understood process can increase the speed, cost and detectability delay of failure.

## Master decision object
### D-AUTO-MASTER-001 — Should this process be automated, and to what level?
Inputs: process stability, work-content repeatability, defect mechanisms, takt/capacity need, ergonomics/safety, product mix, change frequency, tooling, inspection, downtime risk, maintenance skills, integration complexity, CapEx, lifecycle cost and business continuity.

Output: no automation / assistive automation / semi-automation / full automation + prerequisites + evidence + risks + assumptions/open questions.

## Cross-links
Automation <-> Standard Work
Automation <-> PFMEA/control plan
Automation <-> MSA/test systems
Automation <-> line balance/takt
Automation <-> maintenance/OEE
Automation <-> Manufacturing Data Hub

## Integrity rule
Higher automation level is not inherently higher manufacturing maturity.