# 2-bit Synchronous Counter with Static Timing Analysis (STA)

## 📌 Project Overview

This project implements a **2-bit synchronous binary counter** using Verilog and performs **Static Timing Analysis (STA)** using Intel Quartus Prime's **TimeQuest Timing Analyzer**. Timing constraints are applied via an SDC file, and setup/hold slack is analyzed to evaluate the circuit's performance.

---

## 🧠 Key Concepts

- RTL design using **Verilog**
- **Clock constraint** definition using `.sdc`
- Setup and hold timing **slack analysis**
- Timing constraint violation simulation
- Quartus Prime and TimeQuest usage

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `counter.v` | Verilog code for 2-bit synchronous counter |
| `counter.sdc` | SDC file with clock constraint (`create_clock`) |
| `sta-summary.png` | Screenshot of STA result (optional) |
| `README.md` | Project description (this file) |

---

## 🔧 Tools Used

- **Intel Quartus Prime Lite Edition**
- **TimeQuest Timing Analyzer**
- (Optional) **ModelSim / Waveform Viewer** for simulation

---

## ⏱️ Timing Constraints Used

```tcl
create_clock -name clk -period 10.0 [get_ports clk]
