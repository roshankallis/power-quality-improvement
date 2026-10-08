# power-quality-improvement
to improve the quality of power using active filter
# ⚡ Power Quality Improvement Using Shunt Active Power Filter

## 📌 Project Overview

This project focuses on improving electrical power quality by using a **Shunt Active Power Filter (SAPF)**.

The system is designed to reduce harmonic distortion and improve the quality of current supplied to the load. The prototype uses a **DSPIC30F2010 microcontroller**, gate-driver/isolation circuits, a three-phase inverter, rectifier circuit, DC-link components, and sensing circuits.

The controller generates suitable switching pulses for the inverter so that the active filter can compensate for unwanted harmonic components in the load current.

---

## 🎯 Objectives

- Improve electrical power quality.
- Reduce current harmonics.
- Compensate for nonlinear load current.
- Generate appropriate switching pulses for the inverter.
- Improve source current waveform.
- Demonstrate the working of a Shunt Active Power Filter using a hardware prototype.

---

## 🏗️ Hardware Prototype

The developed prototype consists of the following major sections:

1. **dsPIC30F2010 Microcontroller**
2. **TLP250 Isolator / Gate Driver**
3. **Three-Phase Inverter Board**
4. **Rectifier Board**
5. **DC-Link Capacitor**
6. **Current/Voltage Sensing Circuit**
7. **Power Semiconductor Switching Devices**
8. **Inductor / Filter Components**
9. **Power Supply Circuit**
10. **Resistive / Nonlinear Load**

---

## 🔧 Major Components

| Component | Purpose |
|---|---|
| dsPIC30F2010 | Digital control and PWM generation |
| TLP250 | Gate isolation and MOSFET/IGBT driving |
| Three-Phase Inverter | Generates compensating current |
| Rectifier | Converts AC to DC |
| DC-Link Capacitor | Stores DC energy |
| Inductor | Filters/controls compensating current |
| Voltage Sensor | Measures system voltage |
| Current Sensor | Measures load/source current |
| MOSFET/IGBT | High-speed power switching |
| Control Circuit | Generates switching signals |

---

## ⚙️ Working Principle

The Shunt Active Power Filter is connected in parallel with the nonlinear load.

The basic operating sequence is:

```text
        AC SUPPLY
            │
            ▼
      ┌─────────────┐
      │ Nonlinear   │
      │    Load     │
      └──────┬──────┘
             │
             │ Harmonic Current
             ▼
      ┌─────────────┐
      │   SAPF      │
      │  Inverter   │
      └──────┬──────┘
             │
             │ Compensating Current
             ▼
        AC SOURCE
