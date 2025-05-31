
# Knight Rider LED Chaser Project

## 1. Introduction

The Knight Rider LED chaser is a classic electronics project that creates a running LED light effect, mimicking the visual style from the famous Knight Rider TV show. This project is ideal for beginners in embedded systems and PCB design, and serves as a foundation for learning about:

- Basic circuit design
- Timing with 555 Timer or microcontrollers
- PCB layout and routing
- LED interfacing and current limiting

---

## 2. Project Overview

This project implements a Knight Rider-style LED effect using a PCB designed in **Altium Designer**. The board includes:

- Multiple LEDs aligned in a row
- Resistors to limit current
- Either a 555 timer with a CD4017 decade counter **or** microcontroller-based logic to drive the LEDs in sequence

The PCB was fully designed using **Altium**, and Gerber files were exported for manufacturing.

---

## 3. Circuit Diagram / Schematic

The schematic was created in **Altium Designer**, and it includes the LED array, resistors, and control logic.

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
