# STM32 Industrial Automation Controller with Multi-Interface & Relay Outputs

An advanced, multi-layer industrial automation controller powered by the **STM32F030CCT6TR** 32-bit ARM Cortex-M0 microcontroller[cite: 13]. Designed from scratch using **Altium Designer**[cite: 11], this board integrates multi-rail power management, robust industrial communication protocols (RS232 & RS485), analog infrared sensing, and high-reliability relay outputs[cite: 11, 12, 13].

## 🚀 Project Overview
This hardware prototype successfully integrates multiple complex electronic blocks onto a single optimized PCB layout[cite: 11]:
1. **Processing Core:** Centered around the **STM32F030CCT6TR** microcontroller[cite: 13], paired with an external high-precision 14.318 MHz crystal oscillator[cite: 13].
2. **Industrial Communication Module:** Equipped with **RS232** (via MAX3232)[cite: 12], **RS485** (via SN65HVD3082E for robust long-distance industrial networking)[cite: 12], and USB connectivity[cite: 13].
3. **Multi-Rail Power Management Stage:** Features independent AC rectification and regulation stages (**L7805**, **LM7812**, and **LM1117**) providing stable +5V, +12V, and +3.3V power rails.
4. **Analog Front-End (AFE) Sensing:** Infrared (IR) proximity sensor channels conditioned using **LM358** operational amplifiers for accurate signal processing.
5. **Relay Switching Bank:** Integrates 12V electromechanical relays (G5LE-1-E) driven by SBC847 NPN transistors equipped with 1N4007 flyback diodes[cite: 13].

---

## 🛠️ Key Technical Specifications
* **Design Tool:** Altium Designer[cite: 11]
* **Microcontroller:** STM32F030CCT6TR (ARM Cortex-M0, 48 MHz)[cite: 13]
* **Communication Interfaces:** RS232, RS485, USB[cite: 12, 13]
* **Power Supply Rails:** +12V, +5V, and +3.3V regulated rails
* **Sensing & Control:** LM358 operational amplifiers (AFE) and electromechanical relay outputs[cite: 13]

---

## 📷 PCB Visualizations & Renders

### 3D Board View
<img width="533" height="538" alt="3D_View" src="https://github.com/user-attachments/assets/2b83272e-f556-408a-91f9-44c8e85d9eba" />

### Top Layer View
<img width="500" height="526" alt="Top_View" src="https://github.com/user-attachments/assets/2ec081e1-04a7-49f7-a8dd-4254c1f6c9f6" />

### Bottom Layer View
<img width="489" height="471" alt="Bottom_View" src="https://github.com/user-attachments/assets/92263497-3278-411d-88ff-ca87297be35c" />

### Track Layer View
<img width="458" height="481" alt="Track Layout" src="https://github.com/user-attachments/assets/379e624a-0577-491d-b590-0e8862f5b03b" />

---

## 📂 Repository Structure
```text
STM32-Industrial-Automation-Controller/
│
├── Documentation/            # Design exports, PDFs, and PCB renders
│   ├── Schematic.pdf
│   ├── 3D_View.png
│   ├── Top_View.png
│   └── Bottom_View.png
│
├── Hardware/                 # Altium Designer source files & manufacturing outputs
│   ├── Altium_Project/       # Main.PrjPcb, Power Supply, Analog Front-End, MCU & Relays, Communication & Display .SchDocs & .PcbDoc[cite: 8, 9, 10, 11, 12]
│   └── Outputs/              # Gerber files, NC Drill files, and BOM.csv
│
└── README.md                 # Project documentation
