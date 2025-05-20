# ⚙️ 8-bit / 10-bit Capacitive DAC Design in Cadence Virtuoso

> Fully custom-designed capacitive DAC circuits implemented in Cadence Virtuoso, including 8-bit and 10-bit versions. Focused on layout efficiency, gain accuracy, and low-power operation using split capacitor architecture.

---

## 🧱 Project Summary

This repository contains the design, simulation, and layout of precision **capacitive digital-to-analog converters (DACs)**. Both 8-bit and 10-bit versions were created to ensure high resolution and compact layout, capable of operating at **1 MHz+ speeds** while driving a **10 pF capacitive load**.

- 🧮 **Architecture**: Binary-weighted charge-scaling DAC
- 🔋 **Supply Voltage**: 1.5 V
- 📦 **Output Load**: 10 pF
- 🏎 **Minimum Speed**: 1 MHz
- 🎯 **Design Focus**:
  - Split-capacitor optimization
  - Custom op-amp gain tuning
  - Single-ended output (differential upgrade discussed)

---

## 🧰 Key Features

- ✅ 8-bit and 10-bit DAC implementations
- ✅ Fully custom schematic and layout in Cadence Virtuoso
- ✅ Split capacitor array for area and parasitic reduction
- ✅ Op-amp gain tuning through tail current voltage control
- ✅ Power measurement via simulation calculator

---

## 🔧 8-bit DAC Design

![image](https://github.com/user-attachments/assets/3b246aaf-995b-4266-8f7b-987b33b96e41)

- Output voltage shows excellent linearity across all 256 codes
- Area-optimized layout using symmetrical routing
- Op-amp delivers stable gain across expected load and frequency range

---

## 🔢 10-bit DAC Implementation

![image](https://github.com/user-attachments/assets/93f005cc-4027-431a-8546-4521bb2ea281)

- 1024-code resolution enables high dynamic range
- Split capacitor strategy minimizes large-capacitor area growth
- Clean output swing and rapid settling time verified via simulation

---

## 📈 Simulation Results

### 🔹 Voltage Output Linearity (8-bit Example)

- 8bit
![image](https://github.com/user-attachments/assets/55e86750-1f23-4052-87c0-4e310e2e3560)


- 10 bit
![image](https://github.com/user-attachments/assets/60113f3e-5b9b-448c-8835-d37e5c5c5321)


 
- Ideal and measured voltages closely match
- **Gain error**: ~–5.15%
- **LSB size**: ~5.16 mV

---

### 🔹 Power Consumption

Average current drawn during operation was measured using the ADE calculator.

![image](https://github.com/user-attachments/assets/cca09c08-376f-4113-8332-849a6ded59ef)


---

