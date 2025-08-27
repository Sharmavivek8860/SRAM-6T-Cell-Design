# 🧩 6T SRAM Cell Design  

## 📌 Project Overview  
This repository contains a comprehensive design and analysis of a **6-Transistor (6T) Static Random Access Memory (SRAM) cell**.  
The project, completed as part of my **VLSI and Digital IC Design coursework**, explores a fundamental building block of modern digital memory.  

The design was implemented using the **Cadence Virtuoso tool suite** and analyzed for its critical operational parameters.  

The primary goal of this project was to demonstrate a deep understanding of **transistor-level circuit design, layout, and performance analysis** for a foundational memory element.  
The design includes both the **schematic and physical layout** of the 6T cell.  

---

## ✨ Project Highlights  
- 🛠️ **Complete Design Flow** – From schematic capture and netlist simulation to physical layout and post-layout verification.  
- 📊 **Critical Parameter Analysis** – Static Noise Margin (SNM), Read/Write timing, and stability.  
- ⚡ **Technology Node** – Designed using industry-standard process technology (e.g., 180nm/90nm/45nm).  
- 🖥️ **EDA Tools** – Implemented using **Cadence Virtuoso** for schematic, layout, simulation, and verification.  

---

## 🧠 6T SRAM Cell Architecture  
The **6T SRAM cell** is a bistable circuit composed of six MOSFETs that can store **one bit of information**.  

- **Four transistors** form two cross-coupled inverters (the storage element).  
- **Two access transistors** act as pass gates to control read/write operations.  

👉 This architecture is widely used in **cache memory** because of:  
- Low standby power consumption  
- High-speed operation  

---

## 🔬 Methodology  

### 1️⃣ Schematic Design and Simulation  
- Created **transistor-level schematic** in Cadence Virtuoso.  
- Verified cell functionality with **testbenches** for:  
  - **Read Operation** – Ensure stable data is read without disturbance.  
  - **Write Operation** – Confirm new data can be stored.  
  - **Static Noise Margin (SNM)** – Measured SNM during read/hold using the **butterfly curve** method.  
  - **Timing Analysis** – Characterized **Read/Write delay**.  

### 2️⃣ Physical Layout  
- Created **layout of the 6T cell** in Virtuoso, optimized for density and performance.  
- **Verification Steps:**  
  - ✅ **Design Rule Check (DRC)** – Ensured compliance with process rules.  
  - ✅ **Layout vs. Schematic (LVS)** – Confirmed logical-physical consistency.  
  - ✅ **Post-Layout Simulation** – Extracted parasitics and validated real-world behavior.  

---

## 📊 Results and Analysis  

| Metric                     | Value         | Methodology |
|-----------------------------|---------------|-------------|
| **Read SNM**               | ~864 mV       | DC Sweep + Butterfly Curve |
| **Hold SNM**               | Similar to Read SNM | DC Sweep without access transistors |
| **Read Time**              | ~340 ps       | Transient simulation, WL → BL threshold |
| **Write Time**             | ~190 ps       | Transient simulation, WL+BL → Q/Qbar switch |

---

## ✅ Conclusion  
This project successfully demonstrates the **design and analysis of a 6T SRAM cell**, a **fundamental element in modern computing systems**.  

Key learnings include:  
- Deep understanding of **transistor-level memory design**.  
- Hands-on expertise with **Cadence Virtuoso** and VLSI design flow.  
- Exploration of trade-offs between **performance, power, and area** in custom IC design.  

---

## 📂 Repository Contents  
- `schematic/` – Transistor-level design in Cadence Virtuoso.  
- `layout/` – 6T SRAM layout files with DRC/LVS verification.  
- `simulation/` – Testbenches, waveforms, and analysis results.  
- `docs/` – Project report, screenshots, and methodology.  

---

## 🛠️ Tools & Technologies  
- **EDA Tool:** Cadence Virtuoso  
- **Languages:** Verilog-A (for testbenches, if used)  
- **Technology Nodes:** 180nm / 90nm / 45nm (specify)  

---

✍️ *Designed by Sharma Vivek – B.Tech, Electronics & Communication Engineering*  
