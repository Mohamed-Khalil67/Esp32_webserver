# ESP32 WebSocket LED Control Project

This project implements a simple real-time LED control interface using an ESP32 microcontroller. It hosts a webpage via SPIFFS and uses WebSockets for communication between the ESP32 and a browser-based interface.

## 🔧 Features

- 📡 ESP32 as a WiFi Access Point
- 🧠 Real-time communication with WebSockets
- 💾 HTML/CSS served from onboard SPIFFS
- 💡 Toggle LED and visualize status via canvas
- 🔍 Serial debug output

---

## 🧰 Hardware Requirements

- ESP32 Dev Board  
- 1x LED  
- 1x 220Ω resistor (optional but recommended)  
- Breadboard + jumper wires

### Circuit

- **GPIO 23 → Anode** (longer leg of LED)
- **GND → Cathode** (shorter leg of LED, via 220Ω resistor)

---

## 📁 File Structure

```text
project-root/
├── data/
│   ├── index.html     # Web interface
│   └── style.css      # Optional styling
├── src/
│   └── main.cpp       # ESP32 firmware
├── platformio.ini     # PlatformIO config (if used)
└── README.md          # This file
