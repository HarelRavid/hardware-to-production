# 3.6.5 Milling

status: Researching
provenance: [GNR]

## Definition
Milling removes material using rotating multi-edge cutters while tool/workpiece motion generates prismatic, freeform and multi-axis geometry.

## Engineering meaning
In production, milling economics are often governed by setup count, accessibility, cutter reach/rigidity, stock removal, tool changes, workholding and inspection rather than geometry alone.

## DFM questions
- Can all critical features be machined from fewer orientations?
- Are internal radii compatible with standard cutters?
- Are pockets/deep features designed for rigid tool access?
- Can datum-critical features be completed in one setup?
- Does the part justify 5-axis simultaneous machining or merely indexed positioning?
- Can stock/near-net geometry reduce removed volume?

## Core objects
- 3-axis milling
- indexed 4/5-axis
- simultaneous 5-axis
- face/shoulder/slot/profile milling
- roughing vs finishing
- adaptive/high-efficiency toolpaths
- rest machining
- tool reach and holder clearance
- internal-radius strategy
- thin-wall machining
- fixture strategy
- probing and work offsets

## Production risks
- chatter/deflection
- recutting/chip evacuation
- tool-holder collision
- datum transfer between setups
- thin-wall distortion
- thermal drift
- tool-wear-induced dimensional drift

## Decision links
- 3-axis vs multi-axis
- machine from billet vs near-net preform
- standard fixture vs dedicated fixture
- machine feature vs redesign for another process

## Evidence backlog
ISO 230 machine performance, machining dynamics/chatter literature, toolpath research, workholding and thin-wall machining studies.