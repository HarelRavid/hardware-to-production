---
id: H2P-MP-JOIN-ADH-001
title: Structural Adhesive Bonding Overview
object_type: Knowledge Object
semantic_type: Manufacturing Process
domain: Manufacturing Processes
module: Joining Technologies / Adhesive Bonding
knowledge_path: 3.5.AdhesiveBonding
lifecycle: [Prototype, EVT, DVT, PVT, Pilot, Bridge Production, Serial Production, Sustainment]
status: Researching
evidence_maturity: L1
provenance: [GNR, STD]
tags: [adhesive-bonding, joining, surface-preparation, structural-adhesive]
questions_answered:
  - When should an adhesive joint be considered instead of mechanical fastening or welding?
  - Why is surface preparation part of the joining process rather than a secondary cleaning step?
  - Which joint properties must be validated before serial production?
related_decisions: []
open_questions:
  - Build material-family-specific durability guidance for metals, thermoplastics and composites.
assumptions: []
knowledge_conflicts: []
---

# Structural Adhesive Bonding Overview

## 1. Definition

Adhesive bonding joins adherends using an adhesive layer that transfers load across bonded surfaces after the defined application and cure process.

## 2. Engineering Meaning

The engineering system is not only the adhesive chemistry. Joint performance depends on the combination of:

- adherend material and surface condition;
- joint geometry and load path;
- surface preparation;
- adhesive selection;
- bondline thickness/control;
- application and cure process;
- environmental exposure;
- inspection and process control.

For production engineering, adhesive bonding therefore behaves as a controlled manufacturing process, not as a material-selection task alone.

## 3. Decision Impact

Adhesive bonding can be valuable when a design benefits from distributed load transfer, joining dissimilar materials, reduced local stress concentration, sealing plus joining, or cosmetic surfaces without visible fasteners.

It becomes higher-risk when reliable surface preparation, cure control, inspection, environmental durability or repairability cannot be established.

## 4. Surface Preparation

ISO 17212:2012 provides guidance for preparation of commonly encountered metal and plastic surfaces prior to structural adhesive bonding. This supports treating surface preparation as a defined process input with its own specification, verification and records.

Key manufacturing questions include:

- What contamination must be removed?
- Is mechanical abrasion required?
- Is chemical treatment / primer required?
- What is the allowable time between preparation and bonding?
- How will prepared surfaces be protected from recontamination?
- How will preparation be verified?

## 5. Fabrication Quality and Records

ISO 21368:2022 provides guidance for fabrication quality requirements and reporting procedures for adhesively bonded structures, including the importance of records for risk evaluation of bonded structures in service.

This connects adhesive bonding directly to:

- work instructions;
- operator/process qualification;
- traceability;
- material batch control;
- environmental process conditions;
- cure records;
- inspection and acceptance criteria.

## 6. Testing Context

A standard lap-shear test is useful for defined comparisons but must not automatically be converted into a universal joint design allowable.

ASTM D1002 explicitly cautions that apparent shear strength from a single-lap specimen is not suitable as a design allowable for differently configured structural joints without analysis of the joint and adhesive behavior.

This distinction is important for the Data Hub:

**coupon property ≠ joint allowable ≠ production capability.**

## 7. Durability

Adhesive qualification should consider environmental durability, not only initial strength. ISO 10354 uses a wedge rupture approach to characterize durability of structural adhesive bonded assemblies and can also help evaluate surface preparation effects for applicable adherend systems.

Relevant exposures may include:

- temperature / thermal cycling;
- humidity / water;
- chemicals;
- UV where exposed;
- creep / sustained load;
- fatigue;
- galvanic/environmental interaction between dissimilar adherends.

## 8. Common Failure Categories

- Adhesive failure at interface
- Cohesive failure within adhesive
- Substrate failure
- Inadequate cure
- Contamination / poor surface preparation
- Excessive peel or cleavage loading
- Bondline thickness variation
- Environmental degradation
- Assembly movement during cure
- Incorrect adhesive mixing / ratio where applicable

## 9. Prototype-to-Production Transition

Prototype bonding often succeeds with highly skilled manual preparation and generous cure time. Serial production may fail if those implicit controls are not converted into explicit process controls.

Transition work should therefore capture:

1. exact surface preparation;
2. adhesive identity / lot / shelf-life state;
3. dispense or mix method;
4. bondline control;
5. fixture strategy;
6. cure time / temperature / humidity;
7. inspection method;
8. acceptance criteria;
9. repair / rework rule;
10. traceability requirements.

## 10. Relationships

| Type | Target | Strength | Confidence | Provenance | Reason |
|---|---|---|---|---|---|
| ALTERNATIVE_TO | Mechanical Fastening | Medium | High | [GNR, SYN] | Both can join dissimilar components but differ in serviceability and load transfer |
| ALTERNATIVE_TO | Welding | Medium | High | [GNR, SYN] | Bonding can avoid fusion/HAZ but introduces surface/cure controls |
| REQUIRES | Surface Preparation | Mandatory | High | [GNR, STD] | Bond performance depends on controlled adherend surface preparation |
| DEPENDS_ON | Environmental Compatibility | Strong | High | [GNR, STD] | Durability depends on service environment and adhesive/adherend system |
| REQUIRES | Process Traceability | Strong | High | [GNR, STD] | Fabrication records support quality and risk evaluation |
| TESTED_BY | Joint Mechanical Testing | Strong | High | [GNR, STD] | Joint performance must be evaluated in representative test configurations |

## 11. Questions Answered

- Is adhesive bonding a material choice or a manufacturing process?
- Which variables must be controlled to scale a bonded prototype?
- Why can a lap-shear value not be used blindly as a design allowable?
- Which process records matter during NPI?

## 12. Sources

- ISO 17212:2012 — Structural adhesives — Guidelines for surface preparation of metals and plastics prior to adhesive bonding.
- ISO 21368:2022 — Adhesives — Guidelines for fabrication of adhesively bonded structures and reporting procedures suitable for risk evaluation.
- ISO 10354:1992 — Adhesives — Characterization of durability of structural-adhesive-bonded assemblies — Wedge rupture test.
- ASTM D1002 — Apparent shear strength of single-lap-joint adhesively bonded metal specimens.

## 13. Next Research

- Joint geometry: lap, scarf, stepped-lap, peel/cleavage reduction.
- Adhesive families: epoxy, acrylic/MMA, polyurethane, cyanoacrylate, silicone and structural tapes.
- Bondline thickness control.
- Surface treatment by substrate family.
- Cure-process capability and automation.
- Inspection/NDT limitations for bonded joints.
- Repair, disassembly and end-of-life implications.