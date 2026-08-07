# 2.2.5 CNC Machining Parameter Principles

provenance: [GNR, GOV, IND, SYN]
status: Researching

## 2.2.5.1 Scope
This entry explains parameter-selection logic for prototyping. It is intentionally not a universal feeds-and-speeds cookbook.

## 2.2.5.2 Main variables
- cutting speed / spindle speed
- feed per tooth or feed per revolution
- axial depth of cut
- radial engagement / width of cut
- tool diameter and flute count
- tool overhang
- coolant/lubrication strategy
- material grade and condition
- machine/spindle dynamics
- workholding and part stiffness

## 2.2.5.3 Core rule
Parameters must be selected as a coupled system. Raising spindle speed without considering stability, tool wear, heat, chip evacuation, rigidity or machine acceleration can reduce reliability instead of improving lead time.

NIST high-speed machining research identifies system dynamics, tool-wear-based parameter definition, high feed/acceleration capability, intelligent path generation and pre-process verification as enabling requirements for rapid CNC prototype production.

## 2.2.5.4 Dynamic/adaptive roughing
Modern CAM can reduce radial engagement while increasing axial engagement, allowing more consistent tool load and potentially higher material removal rate. Vendor demonstrations are useful as process examples but should not be treated as universal performance guarantees.

## 2.2.5.5 Prototype optimization target
For low-volume development, optimize elapsed learning time rather than only cycle time. A slightly slower but robust process can be superior if it reduces tool failure, scrap, rework or special-tool procurement.

## 2.2.5.6 Practical sequence
1. Identify material and condition.
2. Select tool geometry/coating suitable for the material group.
3. Check tool reach and rigidity.
4. Start from validated manufacturer/tool-library data.
5. Reduce parameters for weak workholding, thin features or long overhang.
6. Simulate tool/holder/fixture.
7. Prove out conservatively.
8. Capture stable parameters in the build record for repeat builds.

## 2.2.5.7 Do not generalize
A cutting speed published for one insert, coating, hardness range or tool geometry is not a generic material limit. Parameter records must preserve tool and workpiece context.

## Relationships
- GUIDES -> H2P-PW-058 CAM for Prototyping
- GUIDES -> H2P-PW-065 CNC Tooling Selection
- DEPENDS_ON -> H2P-PW-064 Prototype Machining Material Selection
- DEPENDS_ON -> H2P-PW-059 Prototype Workholding
- AFFECTS -> H2P-PW-066 Machining Surface Finish
- AFFECTS -> H2P-PW-199 CNC Prototype Cost Drivers

## Sources
- Schmitz et al., NIST, The Application of High-Speed CNC Machining to Prototype Production (2001)
- Davies, Schmitz & Dutterer, NIST, How to Succeed at High Speed Machining (2001)
- Kennametal dynamic milling technical guidance
- Seco Tools machinability guidance
