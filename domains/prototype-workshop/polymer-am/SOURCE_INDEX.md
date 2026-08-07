# Polymer Additive Manufacturing — Source Sub-Index

This sub-index contains high-value sources used for the Polymer AM cluster. The repository-level `SOURCE_INDEX.csv` remains the global source register.

## Standards

### ISO/ASTM 52903-1:2020 — Material extrusion feedstock materials
Official source: https://www.iso.org/standard/67290.html
Use: FDM/FFF feedstock specification, including unfilled, filled and reinforced plastics.
Status: Published; under periodic review.

### ISO/ASTM 52911-2:2019 — Design for laser-based PBF of polymers
Official source: https://www.iso.org/standard/72952.html
Use: SLS/polymer PBF design guidance.
Status: Confirmed current in 2026.

### ISO/ASTM 52910:2018 — AM design requirements/guidance
Official source: https://www.iso.org/standard/67289.html
Use: General AM design framework.

## Government / research

### NIST — Material Extrusion
https://www.nist.gov/additive-manufacturing/research-areas/technologies/material-extrusion
Use: Independent process-science anchor for temperature, stress and material response in polymer extrusion AM.

### NIST — Measurement Science Roadmap for Polymer-Based Additive Manufacturing
https://doi.org/10.6028/NIST.AMS.100-5
Use: Polymer AM measurement, characterization and qualification framework.

### NIST — Additive Manufacturing Part Qualification
https://www.nist.gov/programs-projects/additive-manufacturing-part-qualification
Use: Accuracy, surface topography, internal geometry and qualification context.

## Current industrial material datasets — use as system-specific evidence, not universal material properties

### Ultimaker Method-series materials
https://ultimaker.com/materials/method-series-pla/
Useful current comparative data for PLA/Tough PLA, PETG, ABS/ABS-R, ASA, Nylon and other extrusion materials. Values are specific to the vendor's material/process system.

### Formlabs — High Temp Resin
https://formlabs.com/products/high-temp-resin/
Important evidence that SLA post-cure state materially changes mechanical/thermal performance.

### Formlabs — Tough 1000 Resin
https://formlabs.com/products/tough-1000-resin/
Example of highly ductile engineering photopolymer; published properties include exact printer/layer/cure conditions.

### Formlabs — Tough 1500 Resin
https://formlabs.com/products/tough-1500-resin/
Example of PP-like tough/compliant SLA material positioning with published standardized properties.

### Formlabs — Nylon 12 Powder
https://formlabs.com/products/nylon-12-powder-10/
Current SLS PA12 dataset including X/Y vs Z elongation, HDT, refresh rate and processing notes.

### Formlabs — Nylon 12 Tough Powder
https://formlabs.com/products/nylon-12-tough-powder/
Current ductile PA12-family dataset for snap fits, hinges, impact and low-warpage applications.

### Formlabs — Nylon 12 GF Powder
https://formlabs.com/products/nylon-12-gf-powder/
Current glass-filled PA12 dataset demonstrating stiffness/thermal/ductility tradeoff.

### EOS — PA 2200 / Process Data
https://www.eos.info/polymer-solutions/data-sheets/all-processes-and-materials?id=pa-2200
Important orientation-specific SLS PA12 data. Demonstrates that process parameter set can change isotropy, strength, ductility, surface and cost balance.

## Evidence-handling rule
Vendor TDS data is valuable for engineering decisions only when the exact material, machine/process, orientation, conditioning and post-process state are retained. Do not combine values from different systems into a generic “PLA”, “Nylon” or “SLA resin” property table without explicit normalization and caveats.
