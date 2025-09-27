
# Product_Color_Sorting

## Author  
George Read  
LinkedIn: https://www.linkedin.com/in/george-yaccoup/

---

## Overview  
This repository implements a system for sorting products by color using a sorter, two robotic arms, and a color sensor, all coordinated via a PLC (Programmable Logic Controller). The project involves **5 production lines** for classifying products based on their colors. :contentReference[oaicite:0]{index=0}

---

## Features & Components

- Uses a color sensor to detect the color of incoming products  
- PLC logic to classify and route products accordingly  
- Two robotic arms for physical manipulation / sorting  
- Integration across 5 distinct production lines  
- FactoryIO simulation template included  
- Supporting files (PLCM, logs, system configuration, etc.) included  

---

## Contents

```

.
├── AdditionalFiles/PLCM
├── IM
├── Logs
├── System
├── Vci
├── XRef
├── Color Detection & Filling Boxes.factoryio
└── FactoryIO_Template_S7-1200_V16_V16.ap16

````

- **AdditionalFiles/PLCM** — PLC project/module files  
- **IM** — Instrumentation / measurement files  
- **Logs** — Logs generated during runs or tests  
- **System** — System-level configuration or scripts  
- **Vci**, **XRef** — Auxiliary linking or reference data  
- **Color Detection & Filling Boxes.factoryio** & **FactoryIO_Template_S7-1200_V16_V16.ap16** — FactoryIO simulation and template files  

---

## Getting Started

### Prerequisites

- FactoryIO (or compatible simulation environment)  
- PLC software (Siemens TIA Portal or equivalent, matching S7-1200)  
- Basic knowledge of ladder logic, PLC programming, and robotics integration  

### Installation & Setup

1. Clone the repository  
   ```bash
   git clone https://github.com/georgeyaccoup/Product_color_sorting-.git
   cd Product_color_sorting-


2. Open the PLC / controller project in your PLC development environment (e.g. TIA Portal) using the files in `AdditionalFiles/PLCM`.
3. Open the FactoryIO simulation file `Color Detection & Filling Boxes.factoryio`.
4. Link the PLC to the simulation via OPC UA / OPC DA or the matching interface defined in the simulation template.
5. Load / deploy the ladder logic to the PLC, and start the simulation.
6. Observe how products are classified and sorted through the production lines by color.

---

## Usage

* Run the simulation in FactoryIO
* Supply products (simulated) of different colors
* The PLC logic determines the color and signals the robotic arms to move the product to its corresponding path or bin
* Logs are captured under `Logs/` for debugging or analysis



