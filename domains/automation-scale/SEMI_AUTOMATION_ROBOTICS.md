# 8.3–8.4 Semi-Automation, Robotics & Cobots

status: Researching
provenance: [GNR]

## Semi-automation objects
- powered assist
- guided fixture
- error-proofed tooling
- automatic fastening/dosing boundary
- automatic measurement with manual load/unload
- pick-to-light / digital guidance boundary
- interlocked sequence control
- operator-machine shared cycle

## Robotics objects
- robot/cobot
- payload
- reach
- repeatability
- speed
- end effector
- gripper/tool changer
- part presentation
- vision guidance boundary
- safety system
- guarding/zone
- teach/program revision
- recovery state

## Engineering principle
The robot is only one component of the automated process. Part presentation, fixturing, end-of-arm tooling, sensing, safety, recovery logic and upstream/downstream variation usually determine real cell capability.

## Questions
1. Can parts arrive in a predictable state/orientation?
2. How does the cell recover after a missed pick, jam or partial cycle?
3. What happens to product identity/genealogy during robot handling?
4. Can the automation detect wrong variant or wrong orientation?
5. Is the task better solved by a simple fixture/poka-yoke than a robot?
6. How are end-effector wear and calibration controlled?
7. Can a trained operator safely clear faults without creating hidden process deviations?

## Decision objects
### D-AUTO-SEMI-001 — Which work elements should remain human versus automated?
### D-AUTO-ROBOT-001 — Robot/cobot applicability
### D-AUTO-EOAT-001 — End-of-arm tooling and sensing strategy
### D-AUTO-REC-001 — Fault recovery and safe restart strategy

## Cross-links
Robotics <-> material handling
Robotics <-> safety
Robotics <-> fixtures
Robotics <-> genealogy
Robotics <-> maintenance
Semi-automation <-> ergonomics

No universal robot utilization or payback threshold is asserted.