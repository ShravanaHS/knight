
# Knight Rider LED Chaser Project

## 1. Introduction
Hi! In this repository, I’ve designed a cool Knight Rider LED chaser circuit that creates the iconic back-and-forth LED effect from the Knight Rider TV show. I used a [CD4017 decade counter IC](https://www.ti.com/product/CD4017B) to count from 0 to 10 and light up LEDs in sequence, paired with a [555 Timer IC](https://www.ti.com/product/NE555) for precise clock pulses to control the timing. I tested the circuit’s functionality with simulations in [MultiSim](https://www.ni.com/en-us/shop/electronic-test-instrumentation/multisim.html) and [Tinkercad](https://www.tinkercad.com/), and designed the PCB layout using [Altium Designer](https://www.altium.com/altium-designer). This project is great for beginners.

It’s a fun and easy way to get started with electronics and PCB design!


## 2. Project Overview

This project creates a Knight Rider-style LED chaser effect using a custom PCB designed in Altium Designer. The circuit features:

- Multiple LEDs arranged in a circular pattern for a visually appealing sequential blinking effect.
- Basic passive components, including resistors and capacitors, to manage clock delays and limit LED current.
- A 555 Timer IC paired with external resistors and capacitors to generate precise clock pulses.
- A CD4017 decade counter IC that receives clock pulses from the 555 Timer to drive the LEDs in sequence (counting from 0 to 10).
- Upon powering the circuit, the LEDs blink sequentially in a circular pattern, mimicking the iconic Knight Rider effect.

The PCB was fully designed in Altium Designer, and Gerber files were exported for manufacturing.

---
# Knight Rider LED Chaser Project

## 3. Simulation

To verify the functionality of the Knight Rider LED Chaser circuit, I simulated it using [MultiSim](https://www.ni.com/en-us/shop/electronic-test-instrumentation/multisim.html) and [Tinkercad](https://www.tinkercad.com/). The simulations included the following components:

- **LEDs**: Arranged to demonstrate the sequential lighting effect in a circular pattern.
- **Resistors**: Used for current limiting to protect the LEDs.
- **Capacitors**: Configured with the 555 Timer to set the clock pulse frequency.
- **555 Timer IC**: Generates precise clock pulses to control the timing of the LED sequence.
- **CD4017 Decade Counter IC**: Drives the LEDs in sequence by counting from 0 to 10 based on the clock input.

Both simulations confirmed the circuit’s behavior, showing the LEDs blinking in the iconic Knight Rider pattern. Below are screenshots of the simulations from MultiSim and Tinkercad:

<div align="center">
  <img src="path/to/multisim-screenshot.png" alt="MultiSim Simulation" width="600">
  <p><strong>Figure 1: MultiSim Simulation of Knight Rider LED Chaser</strong></p>
</div>

<div align="center">
  <img src="path/to/tinkercad-screenshot.png" alt="Tinkercad Simulation" width="600">
  <p><strong>Figure 2: Tinkercad Simulation of Knight Rider LED Chaser</strong></p>
</div>
## 3. Circuit Diagram / Schematic

The schematic was created in **Altium Designer**, and it includes the LEDs, resistors, capacitors, 555 timer IC and CD4017 IC.


📁 **File:** `KnightRider.SchDoc`

---

## 4. PCB Layout

The PCB was laid out with aesthetics and simplicity in mind. Short traces and proper LED alignment were maintained.

📁 **File:** `KnightRider.PcbDoc`

---

## 5. Bill of Materials (BOM)

A full BOM is provided in the `Outputs/` folder, listing all components required to build the board.

📁 **File:** `Outputs/KnightRider_BOM.CSV`

| No. | Component         | Value     | Description          |
|-----|-------------------|-----------|----------------------|
| 1   | LEDs              | 8 or 10   | 5mm Red LEDs         |
| 2   | Resistors         | 330Ω      | For LED current limit|
| 3   | IC (optional)     | 555 / CD4017 | Timing + Logic     |
| 4   | Capacitor         | 10 µF     | Timing stability     |
| 5   | Power Supply      | 5V        | USB or Battery       |

---

## 6. Gerber Files for PCB Manufacturing

Gerber files for manufacturing are available in the `Outputs/Gerber/` directory. These include:

- Top/Bottom Layer
- Silkscreen
- Soldermask
- Drill file
- Board outline

📁 **Directory:** `Outputs/Gerber/`

| File Type | Description                  |
|-----------|------------------------------|
| `.GTL`    | Top copper layer              |
| `.GBL`    | Bottom copper layer           |
| `.GTS`    | Top soldermask                |
| `.GBS`    | Bottom soldermask             |
| `.GTO`    | Top silkscreen                |
| `.GBO`    | Bottom silkscreen             |
| `.TXT`    | Drill file                    |
| `.GML`    | Outline/mechanical layer      |
| `.DRD`    | Drill data                    |

---

## 7. How It Works

1. The circuit uses either:
   - A **555 timer + CD4017** IC to sequentially turn LEDs on and off.
   - A **microcontroller (e.g., ATtiny/ATmega)** running a simple chaser program.

2. LEDs are connected through resistors to prevent overcurrent.

3. The timing circuit ensures LEDs light up one by one, giving the running effect.

---

## 8. Applications and Learning Outcomes

- Understanding **timing circuits** (monostable/astable)
- Learning **digital logic sequencing**
- Introduction to **PCB layout tools** like Altium
- Useful as a **visual debugging aid**, **decoration**, or **intro project** for embedded systems

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
| GreatScott!              | [YouTube](https://www.youtube.com/watch?v=f3ptl9K2Zxg)                |
| Afrotechmods             | [YouTube](https://www.youtube.com/watch?v=EGxL8vYqIP0)                |
| EEVblog                  | [YouTube](https://www.youtube.com/watch?v=tbkD73I1T2Y)                |
