> Industrial Smart Switch & LoRa Edge Gateway Node

A production-ready edge IoT smart socket controller built on **ESP32-S2** and **SX1278 LoRa** sub-GHz transceiver. Engineered for low-latency long-range control, opto-isolated AC relay load switching, and zero-data-loss fail-safe power recovery.

---

> Hardware Prototype & Enclosure

![Hardware Setup 1](industrial%20SW1.jpeg)
![Hardware Setup 2](industrial%20smart%20switch%202.jpeg

---

> Key Technical Features

- **Sub-1GHz Wireless Connectivity:** Integrated SX1278 LoRa node for long-range, non-line-of-sight telemetry.
- **Opto-Isolated AC Load Control:** High-voltage isolation driving a 10A relay module inside a standard modular switch box.
- **Fail-Safe State Persistence:** Built-in Non-Volatile Storage (NVS) logic—relays automatically restore their last known state post-power failure.
- **Embedded AC-DC Buck Module:** Direct 220V AC mains step-down power inside the switch enclosure.
- **Real-Time Diagnostics:** LED visual indicator & audio alert system for packet receipt and state toggles.

---

 > System Architecture

 [ Wireless LoRa Controller / Gateway ]
│
│ (Sub-1GHz Telemetry)
▼
[ SX1278 LoRa Module ]
│
│ (SPI Interface)
▼
[ ESP32-S2 Microcontroller ] ──► [ Opto-Coupled Relay Driver ] ──► [ AC Power Socket ]
│
└──► [ Status LED / Buzzer Alerts ]

---

> Hardware Configuration & Pinout

| Module | Protocol / Interface | Description |
| :--- | :--- | :--- |
| **ESP32-S2** | Main Controller | Core application execution & state management |
| **SX1278 LoRa** | SPI | Sub-1GHz RF Receiver / Node |
| **Relay Driver** | GPIO (Opto-Isolated) | Safe 220V AC switching driver |
| **Power Stage** | AC-DC Buck | Compact 220V to 5V DC step-down |

---

 > Getting Started

1. Clone the repository:
   ```bash
   git clone [https://github.com/Sk-sillicon7/ESP-32-lora-smart-switch-gateway.git](https://github.com/Sk-sillicon7/ESP-32-lora-smart-switch-gateway.git)
​2. Open with PlatformIO or Arduino IDE.
​3. Install required libraries: RadioLib, ArduinoJson.
​4. Flash the firmware via USB-C / UART interface to ESP32-S2.

---

​📜 License
​Distributed under the MIT License. See LICENSE for details.





   
