# Printed Circuit Board (PCB) Fabrication information

- 4 layer board
   - See Material Table below
   - Board thickness is 1.59 mm (0.063 inch) +/- 2 mil)
   - Bounding box is 99.8 x 94.6 mm
- Design Rules
    - Minimum Trace / Space design rules
       - Outer layers: 0.127 mm (5.0 mil) / 0.127 mm (5.0 mil)
       - Inner layers: 0.127 mm (5.0 mil) / 0.127 mm (5.0 mil)
    - Outer dimension router tolerance: +/- 0.254 mm (10.0 mil)
    - Hole placement tolerance: +/- 0.075 mm (3.0 mil)
    - Inner tab routed slot tolerance: +/- 0.254 mm (10.0 mil)
- Drills
   - Drill Positional Tolerance: 0.051 mm (2.0 mil)
   - Drill Size tolerance: +/- 0.064 mm (2.5 mil)
- Plated/Un-plated holes
  - There are 6 un-plated (NPT) holes
  - There are 1477 plated through (PTH) holes
  - PTH minimum diameter: 0.254 mm (10 mil)
  - PTH minimum annulus: 0.102 mm (4 mil) radius
- Outline
  - Requires a 1.0 mm or smaller diameter routing bit
- Slots
  - There are no slots.
- Cutouts
  - There are no cutouts
- There are 3 fiducials on the top layer.
- Panel tabs
   - No requirements, besides try to minimize board protrusions
- If not otherwise specified, build to IPC 6012 Class 2 or better.

## Materials

- Controlled impedance
   - While this board is not controlled impedance, the stackup is critical
     for performance of high speed signals.
- Isola FR408HR or material with equivalent Dk.
- Board Surface treatment should be ENIG, althogh immersion Silver is acceptable.
- White silkscreen on top and bottom surface
- Taiyo PSR-4000 or equivalent soldermask on top and bottom

## Stack up

| Layer         | Thickness           | Notes                                        |
|---------------|---------------------|----------------------------------------------|
| Top Copper    | 0.043 mm /  1.7 mil |  Layer 1 foil, 1 oz Cu after plating         |
| prepreg       | 0.200 mm /  7.9 mil |  Prepreg - Isola FR408HR 2113                |
| Layer 2       | 0.018 mm /  0.7 mil |  Layer 2 foil, 0.5 oz Cu                     |
| Core          | 0.991 mm /   39 mil |  Core Isola FR408HR                          |
| Layer 3       | 0.018 mm /  0.7 mil |  Layer 3 foil, 0.5 oz Cu                     |
| prepreg       | 0.200 mm /  7.9 mil |  Prepreg - Isola FR408HR 2113                |
| Bottom Copper | 0.043 mm /  1.7 mil |  Layer 4 foil, 1 oz copper after plating     |
| **Total Stackup** | **1.588 mm / 62.5 mil** |                                      |

## Array / Panel Information

- Coordinate with Contract Manufacturer (CM) for optimal size of this panel.
- If no feedback from CM, then produce single boards (no panel).

## Fabrication Files in "fabrication" Folder

### PCB Artwork

| Filename          | Notes                                         |
| ------------------| --------------------------------------------- |
| -Edge_Cuts.gbr    | RS274X file for the dimension (outline) layer |
| -F_Silkscreen.gbr | RS274X file for the top silkscreen            |
| -F_Mask.gbr       | RS274X file for the top soldermask            |
| -F_Cu.gbr         | RS274X file for the top copper layer          |
| -In1_Cu.gbr       | RS274X file for the layer 2 copper            |
| -In2_Cu.gbr       | RS274X file for the layer 3 copper            |
| -B_Cu.gbr         | RS274X file for the bottom copper layer       |
| -B_Mask.gbr       | RS274X file for the bottom soldermask         |
| -B_Silkscreen.gbr | RS274X file for the bottom silkscreen         |
| -NPTH.drl         | Excellon file for non-plated through holes    |
| -PTH.drl          | Excellon file for plated through holes        | 

### Other Fabrication Information

| Filename            | Notes                                   |
| ------------------- | --------------------------------------- |
| -ipc2581.xml        | IPC-2581 board information file         |

