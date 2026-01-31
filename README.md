 
# 🤖 Arduino Nano Dual Motor Driver Board

The **Arduino Nano Dual Motor Driver Board** is a compact and reliable baseboard designed for small robotics projects. It combines the simplicity of the **Arduino Nano** with the proven **L293D dual H-bridge motor driver**, allowing safe and precise control of two DC motors from a single PCB.

This board is ideal for line-following robots, obstacle-avoidance bots, and general-purpose mobile platforms.

---

## 🚀 Overview

Robotics projects often fail due to unstable power caused by motor noise and current spikes. This board solves that problem by separating **logic power (5V)** from **motor power (VCC)**. A high-current battery powers the motors directly, while an onboard regulator provides clean, stable voltage to the Arduino and motor driver logic.

---

## ✨ Key Features

* **Dual H-Bridge Motor Control**
  Powered by the **L293DNE**, enabling bidirectional control of **two DC motors** with PWM speed regulation.

* **High-Current Power Input**
  Uses an **XT60 connector**, commonly found in LiPo battery systems, for secure and reliable power delivery.

* **Onboard 5V Voltage Regulation**
  An **LM7805 linear regulator** with input and output filtering ensures a stable 5V supply for logic circuitry.

* **Power Status Indicator**
  An onboard LED provides instant visual confirmation that the board is powered.

---

## 🛠️ How It Works

1. **Power Input**
   Battery power enters the board through the **XT60 connector (U4)**.

2. **Voltage Regulation**
   The **LM7805 (U3)** regulates the input voltage down to 5V for the Arduino Nano and L293D logic pins.

3. **Control Logic**
   The **Arduino Nano (U1)** generates direction and PWM signals (M1AIN, M1BIN, M2AIN, M2BIN).

4. **Motor Drive Stage**
   The **L293D (U2)** uses the high-current motor supply (VCC) to drive motors connected at **CN1** and **CN2**.

---

## 📋 Bill of Materials (BOM)

| Reference    | Component               | Quantity | Description                 |
| ------------ | ----------------------- | -------- | --------------------------- |
| **U1**       | Arduino Nano            | 1        | Microcontroller             |
| **U2**       | L293DNE                 | 1        | Dual H-Bridge Motor Driver  |
| **U3**       | LM7805                  | 1        | 5V Linear Voltage Regulator |
| **U4**       | XT60 Connector          | 1        | High-Current Power Input    |
| **C1, C2**   | Electrolytic Capacitors | 2        | Input / Output Smoothing    |
| **R1**       | Resistor                | 1        | LED Current Limiting        |
| **CN1, CN2** | 2-Pin Screw Terminals   | 2        | DC Motor Outputs            |

---

## 📂 Project Metadata

* **Designer:** Rahul
* **Organization:** PDE Workshop
* **Design Tool:** EasyEDA
* **Release Date:** 2026-01-31

---

## 📌 Applications

* Line-following robots
* Obstacle-avoidance robots
* Differential drive platforms
* Arduino-based motor control learning

---
 
