# Finite Element Simulation of a Microchip using Abaqus

> FEM-based thermal analysis of Flip Chip technology with heat sink, performed at the **Fraunhofer Institute for Solar Energy Systems ISE**.
>
> **Author:** Atharva Sinnarkar  
> **Affiliation:** Friedrich-Alexander University of Erlangen-Nuremberg — MSc. Computational Engineering (Computational Materials Science)

---

## Overview

This project implements a Finite Element Method (FEM) simulation of heat conduction in a microchip using **Abaqus**. The simulation models Flip Chip packaging technology and investigates thermal behaviour across the chip stack, with a focus on the STIM (Solder Thermal Interface Material) layer's thermal resistance.

The study is structured in four parts:

| Part | Topic |
|------|-------|
| FEM 1 | Introduction to Flip Chip Technology & Modelling Considerations |
| FEM 2 | Simulation Results (Temperature, Heat Flux, Conduction Axes) |
| FEM 3 | Analysis of Thermal Resistance of the STIM Layer in Excel |
| FEM 4 | Literature Reference |

---

## Simulation Details

### Problem Statement
Thermal analysis of a microchip assembly using Flip Chip technology with an attached heat sink. The model investigates steady-state heat conduction through the chip stack, including the STIM layer between chip and heat sink.

### Key Parameters
- **Surface temperature (Ts):** 63 °C  
- **Ambient temperature (Ta):** 27 °C

### Results Investigated
1. **Temperature Distribution** — Full thermal field across the chip assembly
2. **Heat Flux** — Magnitude and direction of heat flow
3. **Main Axis of Conduction** — Dominant conduction path through the stack
4. **STIM Layer Analysis** — Top and bottom surface thermal behaviour
5. **Average Heat Flux in Z-Axis** — Through-thickness flux investigation

---

## Repository Contents

```
📂 abaqus-microchip-fem/
├── README.md
├── Chip Simulation.cae          # Abaqus model file (no subscription required*)
├── FCP_HeatConduction.odb       # Abaqus output database (requires Abaqus license)
└── Presentation_Fraunhofer.pptx # Full results presentation (Fraunhofer ISE)
```

> **\* Note on the `.cae` file:** This model was built without an Abaqus subscription, which imposes a **limited number of mesh elements**. Results may differ slightly from the licensed `.odb` output. The `.odb` file contains the full high-fidelity simulation results and requires an active Abaqus license to open.

---

## How to Open the Files

### `.cae` — Abaqus Model (No License Required)
1. Install [Abaqus Student Edition](https://www.3ds.com/products-services/simulia/products/abaqus/abaqusexpress/) (free, element-limited)
2. Open Abaqus CAE
3. `File → Open` → select `Chip Simulation.cae`

### `.odb` — Output Database (Abaqus License Required)
1. Open Abaqus CAE or Abaqus Viewer with a valid license
2. `File → Open` → select `FCP_HeatConduction.odb`
3. Navigate to the **Visualization** module to inspect results

---

## Dependencies

| Software | Version | Notes |
|----------|---------|-------|
| Abaqus CAE/Viewer | 2022 or later recommended | `.odb` requires full license |
| Abaqus Student Edition | Any | `.cae` opens with element limit |
| Microsoft Excel | Any | For STIM thermal resistance analysis (FEM 3) |

---

## Literature

Michael I. Okereke, Yuxiao Ling —
*"A computational investigation of the effect of three-dimensional void morphology on the thermal resistance of solder thermal interface materials"*

---

## License

This project is shared for academic and educational purposes. If you use or reference this work, please credit the author and the Fraunhofer Institute for Solar Energy Systems ISE.
