# 3.6.13 Machining DFM Rules

status: Researching
provenance: [GNR]

## 3.6.13.1 Purpose
Define production-oriented DFM rules for machined parts without turning supplier-specific capability limits into universal laws.

## 3.6.13.2 Feature-access rules
Objects:
- tool access
- internal corner radius
- deep pocket
- narrow slot
- thin wall
- long-reach feature
- blind cavity
- undercut
- backside feature
- compound-angle feature

Principle: geometric manufacturability depends on tool access, rigidity, workholding, machine architecture and inspection access, not geometry alone.

## 3.6.13.3 Setup-oriented DFM
Questions:
1. Can critical features share one datum-controlled setup?
2. Can a feature be repositioned to avoid a second setup?
3. Can the part be clamped without distorting functional surfaces?
4. Can stock geometry support stable fixturing?
5. Is there room for jaws, locators, probes and cutters?

## 3.6.13.4 Tolerance-oriented DFM
Rules:
- allocate tight tolerance only to function-critical characteristics;
- separate size, form, orientation and position requirements;
- avoid using plus/minus dimensions where a functional datum relationship is the real requirement;
- ensure inspection method is feasible before releasing the requirement;
- consider thermal state, fixturing state and post-process state when defining acceptance.

## 3.6.13.5 Surface-oriented DFM
Define surface requirements according to function:
- sealing
- bearing/contact
- fatigue
- sliding/friction
- bonding/coating
- cosmetic

Do not use a generic low-Ra requirement where no functional need exists.

## 3.6.13.6 Material-removal efficiency
Objects:
- buy-to-fly ratio
- stock allowance
- near-net blank
- roughing volume
- chip volume
- material utilization

Decision: machine from billet vs cast/forged/extruded near-net blank.

## 3.6.13.7 Secondary-process strategy
Candidate secondary processes:
- grinding
- honing
- lapping
- heat treatment
- coating
- deburring
- polishing
- passivation/anodizing

The DFM question is whether the functional requirement should be achieved in the primary machining step or by a deliberately selected finishing process.

## 3.6.13.8 Why projects fail
- tolerances copied from prototype inspection instead of product function;
- hidden tool-access problem discovered after supplier RFQ;
- critical datum changes between machining and inspection;
- thin walls distort during unclamping;
- edge break/deburr omitted from drawing;
- cosmetic requirement conflicts with workholding marks;
- secondary finishing changes dimensions but is absent from tolerance stack;
- design optimized for cycle time while setup count dominates cost.

## 3.6.13.9 Decision objects
- D-MACH-DFM-001: Can this part be simplified for fewer setups?
- D-MACH-DFM-002: Should this requirement be machined directly or finished secondarily?
- D-MACH-DFM-003: Billet or near-net blank?
- D-MACH-DFM-004: Is the tolerance functionally justified?

Quantitative thresholds remain evidence-scoped and supplier/process-specific.