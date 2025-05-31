
# Knight Rider LED Chaser Project

## 1. Introduction
Hi! In this repository, I’ve designed a cool Knight Rider LED chaser circuit that creates the iconic back-and-forth LED effect from the Knight Rider TV show. I used a [CD4017 decade counter IC](https://www.ti.com/product/CD4017B) to count from 0 to 10 and light up LEDs in sequence, paired with a [555 Timer IC](https://www.ti.com/product/NE555) for precise clock pulses to control the timing. I tested the circuit’s functionality with simulations in [MultiSim](https://www.ni.com/en-us/shop/electronic-test-instrumentation/multisim.html) and [Tinkercad](https://www.tinkercad.com/), and designed the PCB layout using [Altium Designer](https://www.altium.com/altium-designer). This project is great for beginners.

It’s a fun and easy way to get started with electronics and PCB design!

---

## 2. Project Overview

This project creates a Knight Rider-style LED chaser effect using a custom PCB designed in Altium Designer. The circuit features:

- Multiple LEDs arranged in a circular pattern for a visually appealing sequential blinking effect.
- Basic passive components, including resistors and capacitors, to manage clock delays and limit LED current.
- A 555 Timer IC paired with external resistors and capacitors to generate precise clock pulses.
- A CD4017 decade counter IC that receives clock pulses from the 555 Timer to drive the LEDs in sequence (counting from 0 to 10).
- Upon powering the circuit, the LEDs blink sequentially in a circular pattern, mimicking the iconic Knight Rider effect.

The PCB was fully designed in Altium Designer, and Gerber files were exported for manufacturing.


<div align="center">
  <img src="https://github.com/ShravanaHS/knight/blob/main/knight%20rider/screenshots/Screenshot%202025-05-31%20150848.png" alt="3D diagram" width="900">
  <p><strong>Figure 0:Knight Rider LED Chaser 3D </strong></p>
</div>

---

## 3. Simulation

To verify the functionality of the Knight Rider LED Chaser circuit, I simulated it using [MultiSim](https://www.ni.com/en-us/shop/electronic-test-instrumentation/multisim.html) and [Tinkercad](https://www.tinkercad.com/). The simulations included the following components:

- **LEDs**: Arranged to demonstrate the sequential lighting effect in a circular pattern.
- **Resistors**: Used for current limiting to protect the LEDs.
- **Capacitors**: Configured with the 555 Timer to set the clock pulse frequency.
- **555 Timer IC ([Datasheet](https://www.ti.com/lit/ds/symlink/ne555.pdf))**: Generates precise clock pulses.
- **CD4017 Decade Counter IC ([Datasheet](https://www.ti.com/lit/ds/symlink/cd4017b.pdf))**: Drives the LEDs by counting from 0 to 10.

Both simulations confirmed the circuit’s behavior, showing the LEDs blinking in the iconic Knight Rider pattern. Below are screenshots of the simulations from MultiSim and Tinkercad:

<div align="center">
  <img src="https://github.com/ShravanaHS/knight/blob/main/knight%20rider/screenshots/Screenshot%202025-05-23%20213528.png" alt="MultiSim Simulation" width="900">
  <p><strong>Figure 1: MultiSim Simulation of Knight Rider LED Chaser</strong></p>
</div>
<br>
</br>
<div align="center">
  <img src="https://github.com/ShravanaHS/knight/blob/main/knight%20rider/screenshots/counter%20shs.png" alt="Tinkercad Simulation" width="900">
  <p><strong>Figure 2: Tinkercad Simulation of Knight Rider LED Chaser</strong></p>
</div>

📁 **File**: **([Tinker cad Simulation link](https://www.tinkercad.com/things/2YcT8pzfolp-counter-shs))**
📁 **File**: **([MultiSim Simulation](https://github.com/ShravanaHS/knight/blob/main/knight%20rider/simulation%20files/simulation.ms14))**

---

## 4. Circuit Diagram / Schematic

The schematic for the Knight Rider LED Chaser was designed in [Altium Designer](https://www.altium.com/altium-designer).

After simulating the circuit in [MultiSim](https://www.ni.com/en-us/shop/electronic-test-instrumentation/multisim.html) and [Tinkercad](https://www.tinkercad.com/), I used Altium Designer’s Manufacturer Part Search to find component footprints, 3D models, and symbols. For components not available in Altium’s library, I sourced simulation SPICE files, models, symbols, and footprints from [SnapEDA](https://www.snapeda.com/), which also provided ERC (Electrical Rule Check) support.



<div align="center">
  <img src="https://github.com/ShravanaHS/knight/blob/main/knight%20rider/screenshots/Screenshot%202025-05-31%20150752.png" alt="Knight Rider Schematic" width="900">
  <p><strong>Figure 3: Schematic of Knight Rider LED Chaser in Altium Designer</strong></p>
</div>

📁 **File**: `KnightRider.SchDoc`

---

## 5. PCB Layout

After creating the schematic in [Altium Designer](https://www.altium.com/altium-designer), I designed the PCB layout with a focus on aesthetics and simplicity. Key design considerations included:

- Short traces to minimize signal delay and improve efficiency.
- Proper LED alignment to achieve a visually appealing circular pattern.

To ensure a robust and manufacturable design, I implemented the following:

- **Design Rule Checks (DRC)**: Applied DRC in Altium Designer to verify the layout against industry standards.
- calculated trace parameters using [DigiKey’s Trace Width Calculator](https://www.digikey.com/en/resources/conversion-calculators/conversion-calculator-pcb-trace-width) and following the [IPC-2221 standard](https://www.ipc.org/standards).
- **Trace and Via Parameters**:
  - Set electrical clearance to 0.25 mm and trace width to 0.2 mm.
  - Adjusted via hole size to 0.4 mm and via diameter to 0.5 mm for reliable connectivity.
- **Layer Stack Configuration**:
  - Used the Layer Stack Manager in Altium Designer to define:
    - Dielectric thickness of 0.8 mm using FR4 material.
    - Top layer thickness of 0.1 mm (CF-003).
    - Solder mask layer thickness of 0.05 mm (SM-001).

Component footprints and 3D models were sourced from Altium’s Manufacturer Part Search and [SnapEDA](https://www.snapeda.com/) to ensure accuracy. The final PCB layout was exported as Gerber files for manufacturing.

Below are images of the PCB layout showing the top layer, bottom layer, and 2D view:

<div align="center">
  <img src="https://github.com/ShravanaHS/knight/blob/main/knight%20rider/screenshots/Screenshot%202025-05-31%20150824.png" width="900">
  <p><strong>Figure 4: Top Layer of Knight Rider LED Chaser PCB</strong></p>
</div>

<div align="center">
  <img src="https://github.com/ShravanaHS/knight/blob/main/knight%20rider/screenshots/Screenshot%202025-05-31%20150836.png" width="900">
  <p><strong>Figure 5: Bottom Layer of Knight Rider LED Chaser PCB</strong></p>
</div>

<div align="center">
  <img src="https://github.com/ShravanaHS/knight/blob/main/knight%20rider/screenshots/Screenshot%202025-05-31%20150803.png" alt="PCB 2D View" width="900">
  <p><strong>Figure 6: Knight Rider LED Chaser PCB</strong></p>
</div>

📁 **File**: `KnightRider.PcbDoc`

---

## 6. Design Rule Check (DRC)

To ensure the PCB layout meets industry standards and is free of errors, I performed Design Rule Checks (DRC) in [Altium Designer](https://www.altium.com/altium-designer). The DRC process verified electrical clearances, trace widths, via sizes, and other parameters defined in the design rules. After careful adjustments, I achieved **0 DRC errors**, confirming the layout is ready for manufacturing.

Below is a screenshot of the DRC results showing 0 errors:

<div align="center">
  <img src="https://github.com/ShravanaHS/knight/raw/main/knight%20rider/screenshots/Screenshot%202025-05-31%20150951.png" alt="DRC Results" width="900">
  <p><strong>Figure 7: DRC Results Showing 0 Errors in Altium Designer</strong></p>
</div>

---

## 7. Bill of Materials (BOM)

The Bill of Materials (BOM) lists all components required to assemble the Knight Rider LED Chaser circuit. The complete BOM is available in the `Outputs/` folder as a CSV file for reference during procurement and manufacturing.

📁 **File**: `Outputs/KnightRider_BOM.CSV`

| No. | Part Number          | Description                                                                 | Reference Designator | Footprint             | Component ID         | Quantity |
|-----|----------------------|-----------------------------------------------------------------------------|----------------------|-----------------------|----------------------|----------|
| 1   | RCER71E226MWM1H03A  | Capacitor, Ceramic, 22 µF, 25 V, X7R, Radial, RoHS                          | C1, C2               | FP-RCEWM1-MFG         | CMP-06035-003622-1  | 2        |
| 2   | OD103JE             | Resistor, Carbon Composition, 10 kΩ, ±5%, 250 V, 2-Pin THD, RoHS, Bulk      | R3                   | OMTE-RES7X2.5-2      | CMP-2000-06865-1    | 1        |
| 3   | NE555P              | Precision Timer IC, 4.5–16 V, 0–70 °C, 8-Pin DIP, Pb-Free, Tube             | U2                   | P0008A               | CMP-2000-04954-1    | 1        |
| 4   | MFR-25FBF52-1M      | Resistor, Axial, 1 MΩ, ±1%, 250 mW, -55–155 °C, 2-Pin THD, RoHS, Bulk       | R1                   | RESA60-630X240       | CMP-1659-00070-1    | 1        |
| 5   | HLMP-1719           | LED, Yellow, Diffused, T-1, Through-Hole, RoHS                              | LED1–LED10           | FP-HLMP-1719-MFG     | CMP-2000-06410-2    | 10       |
| 6   | CD74HC4017E         | Decade Counter/Divider IC, High-Speed CMOS, 10 Decoded Outputs, 16-Pin DIP   | U1                   | N0016A               | CMP-1623-00548-2    | 1        |
| 7   | 3296Y-1-253LF       | Trimmer Potentiometer, Cermet, 25 kΩ, ±10%, 500 mW, 0–70 °C, 300 V, RoHS    | R2                   | 3296Y_MFG            | CMP-00059-00574897-1| 1        |
| 8   | 22-27-2021          | Male Header, 2.54 mm Pitch, 1x2 Position, 11.7 mm Height, 3.56 mm Tail, RoHS | J1                   | MOLX-22-27-2021_V    | CMP-2000-05537-1    | 1        |


---

## 8. Gerber Files for PCB Manufacturing

The Gerber files required for manufacturing the Knight Rider LED Chaser PCB were generated from the PCB layout designed in [Altium Designer](https://www.altium.com/altium-designer). These files provide all necessary information for PCB fabrication, including copper layers, solder masks, silkscreen, drill data, and board outline. They are stored in the `Outputs/Gerber/` directory and have been verified to comply with industry standards for manufacturing.

📁 **Directory**: `Outputs/Gerber/`

| File Extension | Description                     |
|----------------|---------------------------------|
| `.GTL`         | Top copper layer                |
| `.GBL`         | Bottom copper layer             |
| `.GTS`         | Top solder mask                 |
| `.GBS`         | Bottom solder mask              |
| `.GTO`         | Top silkscreen                  |
| `.GBO`         | Bottom silkscreen               |
| `.TXT`         | Drill file (NC drill data)      |
| `.GML`         | Board outline/mechanical layer  |
| `.DRD`         | Drill drawing data              |

These files are ready for submission to a PCB manufacturer to produce the Knight Rider LED Chaser board.

---

## 9. Project Files

| File Type            | Description                    | Path |
|----------------------|--------------------------------|------|
| **Schematic**        | Altium schematic design         | `KnightRider.SchDoc` |
| **PCB Layout**       | Altium PCB design               | `KnightRider.PcbDoc` |
| **BOM**              | Bill of Materials in CSV        | `Outputs/KnightRider_BOM.CSV` |
| **Gerber ZIP**       | For fabrication                 | `Outputs/Gerber/*.zip` |

---

## 10. Future Improvements

- Add brightness control using PWM
- Switch to programmable IC (e.g., ATtiny85)
- Add sound or motion sensing

---

## References

| Creator / Resource       | Link                                                                 |
|--------------------------|----------------------------------------------------------------------|
| Audas                    | [YouTube](https://www.youtube.com/watch?v=6N2A6LtBWh0&t=498s)        |
| Elonics - Electronics Projects on Breadboard  | [YouTube](https://www.youtube.com/watch?v=Dggk8SIrwZU) |
| Robert Feranec   | [YouTube](https://www.youtube.com/watch?v=PqFtSpAXB9Q&list=PLXvLToQzgzdduBaD4horowdWgcG5uGUW4)|
