# 2.2.11 CNC Prototype Decision Trees

provenance: [GNR, SYN]
status: Researching

## 2.2.11.1 CNC vs Polymer AM
1. Is production-grade bulk material behavior part of the test?
   - Yes -> Prefer CNC when machinable stock exists, unless the production process itself must be represented.
   - No -> Continue.
2. Is complex internal geometry or very rapid low-cost iteration more important than bulk-material fidelity?
   - Yes -> Evaluate polymer AM.
   - No -> Continue.
3. Are tight bores, bearing seats, seal lands or controlled interfaces central to the prototype?
   - Yes -> CNC or hybrid AM + secondary machining is favored.
4. Is the final product injection molded and process-induced molding effects are being validated?
   - Yes -> Neither CNC nor AM alone is fully production-representative; bridge tooling or molded prototypes may be required.

## 2.2.11.2 3-axis vs 4/5-axis
1. Can all required features be reached in one or two simple orientations?
   - Yes -> 3-axis usually minimizes programming/setup complexity.
2. Does rotating the part eliminate multiple manual setups or preserve critical datum relationships?
   - Yes -> Evaluate 4-axis.
3. Are complex angled features, simultaneous tool orientation or deep multi-face access required?
   - Yes -> Evaluate 5-axis.
4. Does the added programming/simulation burden exceed the setup reduction benefit for a one-off?
   - Yes -> Simpler axis strategy may still win.

## 2.2.11.3 Hole finishing strategy
1. Is the hole only for clearance/noncritical passage?
   - Standard drilling or interpolation may be sufficient.
2. Is diameter/roundness/finish important for a fit?
   - Evaluate reaming or boring.
3. Is positional accuracy more important than finish?
   - Coordinate strategy, tool stiffness and inspection dominate; interpolation may be useful depending on size.
4. Is it a bearing/seal feature?
   - Explicitly define size, geometry, finish and inspection; consider finish machining after rough operations.

## 2.2.11.4 Thread strategy
1. Is the thread standard and easily accessible?
   - Tap/thread mill/turn as appropriate.
2. Is the thread large, blind, close to a shoulder or in difficult material?
   - Evaluate thread milling or turning and tool-access constraints.
3. Is repeated assembly in a soft plastic required?
   - Consider inserts rather than direct plastic threads.
4. Is thread depth being specified only because CAD permits it?
   - Recheck functional engagement; excessive depth can add tool/lead-time risk.

## 2.2.11.5 In-house vs outsource CNC
1. Is same-day/next-day learning materially valuable?
   - Yes -> In-house capability gains weight.
2. Is the part beyond internal machine envelope, axis capability, material handling, metrology or operator competence?
   - Yes -> Outsource.
3. Is special tooling/fixturing needed once only?
   - Often outsource unless internal learning justifies the setup.
4. Will the same family of parts repeat frequently during development?
   - In-house soft jaws/modular fixturing can become attractive.
5. Is independent dimensional evidence required?
   - Supplier metrology capability becomes part of selection.

## 2.2.11.6 Tolerance allocation
1. Does the dimension affect fit, sealing, alignment, motion or stack-up?
   - Yes -> determine required tolerance from function.
2. Can the selected machining and measurement system demonstrate it?
   - No -> redesign, change process or change inspection method.
3. Is the tight tolerance merely inherited from CAD/default drawing practice?
   - Remove or relax it.
4. Does the prototype need to mimic intended production capability?
   - If yes, avoid creating a prototype that passes only because CNC is much more precise than the intended production process.

## Relationships
- USES -> H2P-PW-173 Prototype Manufacturing Process Selection
- USES -> H2P-PW-055/056/057 Axis Strategy
- USES -> H2P-PW-063 Machining Tolerance Strategy
- USES -> H2P-PW-197 Hole Making Strategy
- USES -> H2P-PW-198 Thread Strategy
- USES -> CNC Make/Buy and Supplier Selection
