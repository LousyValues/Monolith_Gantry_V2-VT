# Monolith Gantry for Voron 2.4 and Trident [BETA]
![1](Images/monolith_render.PNG)
## What's this?
This is a performance-oriented, configurable gantry system for Voron 2.4 and Trident. It brings VZbot AWD simplicity and Voron space efficiency together.
## Updates
### 14.09.2023: I added the STLs for all of the existing combinations. Huge thanks to **krankydonkey** for remixing all of the Archetype belt clamps for this flipped belt path (CAD/STLs added).
### 11.09.2023: I added the complete X-axis CAD with motor mount clearances to help with toolhead compatibility checks and XY joint and/or toolhead carriage remixing.

A lot of the usable hardware combinations are also included: pins, standoffs, shoulder bolts, etc.

Front rail: belt location from the X-beam is yet to be decided. I am open to suggestions on how we should make the flipped belt path compatible with existing Voron(mod) toolheads. XY joints CAD available for 6 and 9mm belts.

Top rail: the included VZ-Hevort CNC toolhead compatible 6 and 9mm XY joints are easy to remix for different top rail toolheads. Please make sure the layout matches your toolhead (eg. front right belt is upper or lower). Motor mounts will be compatible with both if they're printed accordingly (normal or mirrored).
## Prerequisites for Monolith AWD
- Z chain relocation on V2
- 5mm or double 3mm foam tape under the rear and the front panels, because there's a 3.6mm stepper protrusion
- OR a 4040 frame
- 9 stepper drivers (or CAN) on V2
- 8 stepper drivers on Trident
- Trident may need a bed relocation to get to the front of the bed (you can just move the PEI sheet for the same effect)
- VZ-Hevort CNC toolhead is recommended for no build volume loss (XY joints already available for 6 and 9mm belts)
- OR any toolhead that you make compatible with this gantry (top rail or flipped belt path front rail)
## BOM
### DISCLAIMER: A lot of this stuff is untested, so the BOM and files will change with more testing and feedback.
### Rails:
- Y rails: MGN9H
- X rail: MGN9H/MGN12H
### X axis:
- FRONT X RAIL: any stock-compatible X beam will work with the suitable mounting hardware (remixed XY joints may be required).
- TOP X RAIL: any stock-compatible X beam that can be rotated 90 degrees and can accommodate new XY joint holes will work.
### Belts:
If you don't switch belt sizes, the stock length will be enough.
### BOM note:
To keep the BOM lists relatively simple, I'm going to include all the hardware and motion parts for the motor mounts and XY joints (with the stock stuff included). X extrusion/tube mounting hardware is not included because that can vary based on the configuration.
### [V2.4|6mm|AWD] motor mounts and XY joints
|No.|Description|Qty|
|---|---|---|
|1.|NEMA17 motors (preferably identical)|4 pcs|
|2.|6mm GT2 20T drive pulley|4 pcs|
|3.|F695 flanged bearing|12 pcs|
|4.|6mm GT2 20T Idler|4 pcs|
|5.|6mm GATES GT2 belt|stock length|
|6.|Round aluminum M3 standoff 25x5mm (dowel pins or smooth rods will also work)|8 pcs|
|7.|5x20mm dowel pin/smooth rod (round aluminum M3 standoffs 20x5mm will also work)|2 pcs|
|8.|M5 1mm spacer|12 pcs|
|9.|M3x6 BHCS|4 pcs|
|10.|M3x10 BHCS|4 pcs|
|11.|M3x30 BHCS|8 pcs|
|12.|M3x8 FHCS|11 pcs|
|13.|M3x12 SHCS|2 pcs|
|14.|M3x35 SHCS|16 pcs|
|15.|M3x40 SHCS|2 pcs|
|16.|M3 washer (7mm OD max.)|2 pcs|
|17.|M3x5x4mm heatset inserts|10 pcs|
|18.|M5x10 BHCS|8 pcs|
|19.|M5x12 BHCS|4 pcs|
|20.|M5x16 BHCS|8 pcs|
|21.|M3 roll in T-nut|3 pcs|
|22.|M5 roll in T-nut|28 pcs|
|23.|M2 self tapping screw|2 pcs|

### [V2.4|9mm|AWD] motor mounts and XY joints
|No.|Description|Qty|
|---|---|---|
|1.|long shafted (S35/S55/S80) NEMA17 motors (preferably identical)|4 pcs|
|2.|9mm GT2 20T drive pulley|4 pcs|
|3.|F695 flanged bearing|12 pcs|
|4.|695 bearing|10 pcs|
|5.|9mm GT2 20T Idler|4 pcs|
|6.|9mm GATES GT2 belt|stock length|
|7.|Round aluminum M3 standoff 30x5mm (dowel pins or smooth rods will also work)|8 pcs|
|8.|5x20mm dowel pin/smooth rod (round aluminum M3 standoffs 20x5mm will also work)|2 pcs|
|9.|M5 0.5mm spacer|8 pcs|
|10.|M3x6 BHCS|4 pcs|
|11.|M3x10 BHCS|4 pcs|
|12.|M3x35 BHCS|8 pcs|
|13.|M3x8 FHCS|11 pcs|
|14.|M3x12 SHCS|2 pcs|
|15.|M3x45 SHCS|16 pcs|
|16.|M3x40 SHCS|2 pcs|
|17.|M3 washer (7 mm OD max.)|2 pcs|
|18.|M3x5x4 mm heatset inserts|10 pcs|
|19.|M5x12 BHCS|12 pcs|
|20.|M5x20 BHCS|8 pcs|
|21.|M3 roll in T-nut|3 pcs|
|22.|M5 roll in T-nut|28 pcs|
|23.|M2 self tapping screw|2 pcs|
|24.|M5 washer (10mm OD max.)|4 pcs|

### GE5C Z joints (only for 6mm belts)
|No.|Description|Qty|
|---|---|---|
|1.|GE5C bearing|4 pcs|
|2.|M3x16 SHCS|16 pcs|
|3.|M5x16 SHCS|4 pcs|
|4.|M5x20 SHCS|4 pcs|
|5.|M5 1mm spacer|4 pcs|

### Rigid Z joints (6 and 9mm belts)
|No.|Description|Qty|
|---|---|---|
|1.|M3x25 SHCS|16 pcs|
|2.|M5x40 SHCS|8 pcs|

### [VT|6mm|AWD] motor mounts and XY joints
|No.|Description|Qty|
|---|---|---|
|1.|NEMA17 motors (preferably identical)|4 pcs|
|2.|6mm GT2 20T drive pulley|4 pcs|
|3.|F695 flanged bearing|12 pcs|
|4.|6mm GT2 20T Idler|4 pcs|
|5.|6mm GATES GT2 belt|stock length|
|6.|Round aluminum M3 standoff 25x5mm (dowel pins or smooth rods will also work)|8 pcs|
|7.|5x20mm dowel pin/smooth rod (round aluminum M3 standoffs 20x5mm will also work)|2 pcs|
|8.|M5 1mm spacer|16 pcs|
|9.|M3x6 BHCS|4 pcs|
|10.|M3x10 BHCS|4 pcs|
|11.|M3x30 BHCS|8 pcs|
|12.|M3x8 FHCS|11 pcs|
|13.|M3x12 SHCS|2 pcs|
|14.|M3x35 SHCS|16 pcs|
|15.|M3x40 SHCS|2 pcs|
|16.|M3 washer (7mm OD max.)|2 pcs|
|17.|M3x5x4mm heatset inserts| 10 pcs|
|18.|M5x10 BHCS|24 pcs|
|19.|M5x12 BHCS|8 pcs|
|20.|M3 roll in T-nut|3 pcs|
|21.|M5 roll in T-nut|32 pcs|
|22.|M2 self tapping screw|2 pcs|

### [VT|9mm|AWD] motor mounts and XY joints
|No.|Description|Qty|
|---|---|---|
|1.|long shafted (S35/S55/S80) NEMA17 motors (preferably identical)|4 pcs|
|2.|9mm GT2 20T drive pulley|4 pcs|
|3.|F695 flanged bearing|12 pcs|
|4.|695 bearing|10 pcs|
|5.|9mm GT2 20T Idler|4 pcs|
|6.|9mm GATES GT2 belt|stock length|
|7.|Round aluminum M3 standoff 30x5mm (dowel pins or smooth rods will also work)|8 pcs|
|8.|5x20mm dowel pin/smooth rod (round aluminum M3 standoffs 20x5mm will also work)|2 pcs|
|9.|M5 0.5mm spacer|8 pcs|
|10.|M3x6 BHCS|4 pcs|
|11.|M3x10 BHCS|4 pcs|
|12.|M3x35 BHCS|8 pcs|
|13.|M3x8 FHCS|11 pcs|
|14.|M3x12 SHCS|2 pcs|
|15.|M3x45 SHCS|16 pcs|
|16.|M3x40 SHCS|2 pcs|
|17.|M3 washer (7 mm OD max.)|2 pcs|
|18.|M3x5x4 mm heatset inserts| 10 pcs|
|19.|M5x12 BHCS|32 pcs|
|20.|M3 roll in T-nut|3 pcs|
|21.|M5 roll in T-nut|32 pcs|
|22.|M2 self tapping screw|2 pcs|
|23.|M5 washer (10mm OD max.)|8 pcs|