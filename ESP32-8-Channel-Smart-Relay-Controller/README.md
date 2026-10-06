# ESP32-Based 8-Channel Smart Relay Controller

An enterprise-grade, IoT-ready 8-channel relay controller powered by the **ESP32-WROOM-32** microcontroller, featuring an integrated AC-to-DC power supply and modular relay switching banks[cite: 6, 7]. Designed from scratch using **Altium Designer**[cite: 6].

## 🚀 Project Overview
This hardware prototype integrates robust power management, wireless connectivity, and high-current load switching onto a single optimized printed circuit board[cite: 6, 7]:
1. **Power Management Module:** Utilizes a MeanWell **IRM-30-5** module for reliable 5V generation from mains AC, stepped down via an **AMS1117-3.3** LDO regulator for stable microcontroller logic[cite: 6].
2. **Control & Processing Module:** Centered around the **ESP32-WROOM-32** module, featuring onboard tactile push buttons (`SW1`–`SW8`), an MCP2221A USB-to-UART bridge for seamless programming, and breakout headers[cite: 6].
3. **Relay Switching Module:** Features **8 independent electromechanical relays (`K1`–`K8`)** driven by MMBT2222A NPN transistors, complete with 1N4148 flyback diodes for inductive spike protection and status indication LEDs (`LTST-C171KGKT`)[cite: 6].

---

## 🛠️ Key Technical Specifications
* **Design Tool:** Altium Designer[cite: 6]
* **Microcontroller:** ESP32-WROOM-32 (Wi-Fi & Bluetooth LE)[cite: 6]
* **Input Power:** AC Mains (converted to 5V DC via IRM-30-5 and 3.3V DC via AMS1117)[cite: 6]
* **Switching Capacity:** 8-Channel Relays (JS1-5V-F) driven by MMBT2222A transistors[cite: 6]
* **User Interface:** 8x Tactile push buttons for local manual control[cite: 6]

---

## 📂 Repository Structure
```text
ESP32-8-Channel-Smart-Relay-Controller/
│
├── Documentation/            # Design exports and PDFs
│   ├── Schematic.pdf
│   └── Track Layout.pdf
│
├── Hardware/                 # Altium Designer source files & manufacturing outputs
│   ├── Altium_Project/       # .PrjPcb, Power.SchDoc, Controller.SchDoc, Relays.SchDoc, .PcbDoc
│   └── Outputs/              # Gerber files, Drill files, and BOM
│
└── README.md                 # Project documentation