# 3.6.14 Tolerance, GD&T & Machining Interaction

status: Researching
provenance: [GNR, STD]

## 3.6.14.1 Purpose
Connect design requirements, machining strategy and inspection so tolerance is treated as a functional system rather than a drawing decoration.

## 3.6.14.2 Core objects
- size tolerance
- form tolerance
- orientation tolerance
- location tolerance
- profile tolerance
- datum feature
- datum reference frame
- feature of size
- MMC/LMC/RFS concepts
- bonus tolerance
- virtual condition
- pattern of features
- runout

## 3.6.14.3 Manufacturing relationship
Design datum -> manufacturing locating scheme -> machine coordinate system -> operation sequence -> inspection datum realization.

Potential mismatch between these layers must be treated as a manufacturing risk.

## 3.6.14.4 Capability questions
1. Is the characteristic controlled by machine motion, tool geometry, fixture location, thermal state, or a combination?
2. Is the tolerance expected within one setup or across setup transfer?
3. Does unclamping alter the measured geometry?
4. Does a later heat-treatment/coating/finishing operation shift the characteristic?
5. Can the measurement uncertainty support the acceptance decision?

## 3.6.14.5 Functional tolerance allocation
Tightening a tolerance is not a substitute for understanding:
- assembly stack-up
- sealing function
- bearing/fit requirement
- alignment
- motion clearance
- interchangeability
- measurement strategy

## 3.6.14.6 Decision objects
- D-GDT-MACH-001: Which datums should drive machining and inspection?
- D-GDT-MACH-002: Can critical features remain in one setup?
- D-GDT-MACH-003: Is this tolerance tighter than the functional requirement?
- D-GDT-MACH-004: Does this characteristic require process capability evidence?

## 3.6.14.7 Evidence anchors
Use the applicable ASME Y14.5 or ISO GPS ecosystem according to product/customer/jurisdiction. Do not merge their detailed rule sets silently.

Machine-tool test standards and part inspection standards must not be used as substitutes for product tolerance standards.

## 3.6.14.8 Why projects fail
- datum scheme selected after CAM rather than from function;
- inspection datum differs from manufacturing datum without analysis;
- universal +/- tolerance added to every dimension;
- profile or position requirement converted into unnecessarily tight feature-size tolerance;
- measurement method cannot resolve the specified tolerance;
- process capability inferred from one first-article result.

Detailed clause mapping remains evidence backlog.