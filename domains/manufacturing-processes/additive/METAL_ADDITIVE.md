# 3.11.3 Metal Additive Manufacturing

status: Researching
provenance: [GNR]

## Process families
- laser powder bed fusion / PBF-LB / LPBF
- electron-beam powder bed boundary
- directed energy deposition
- wire-fed DED boundary
- binder jet + debind/sinter
- hybrid additive/subtractive

## Process objects
- powder/wire feedstock
- particle distribution/flowability
- build plate
- recoating
- layer thickness
- laser/beam power
- scan speed
- hatch/scan strategy
- energy input
- shielding/inert atmosphere
- oxygen/moisture control
- support structures
- thermal gradients
- residual stress
- distortion
- porosity/lack of fusion/keyhole-type defects

## Post-processing objects
- stress relief
- support removal
- heat treatment
- HIP where applicable
- machining
- grinding/polishing
- shot/abrasive finishing
- chemical/electrochemical finishing boundary

## DfAM questions
- Can supports be removed and critical internal features cleaned?
- Which surfaces/datums require machining allowance?
- Does build orientation expose a critical load direction to unfavorable process anisotropy?
- Can residual stress/distortion be controlled through design, support, scan strategy and thermal treatment?
- Can internal channels be inspected and verified?
- Is powder reuse/handling part of the qualified material state?

## Decision objects
### D-AM-MET-001 — LPBF, DED, binder jet, machining/casting/forging or hybrid?
### D-AM-ORI-001 — Select build orientation
### D-AM-POST-001 — Required post-processing chain

## Integrity rule
Machine name or nominal alloy designation alone does not define a qualified material condition. Feedstock, machine, parameter set, orientation, thermal history, post-processing and test condition belong to the evidence scope.