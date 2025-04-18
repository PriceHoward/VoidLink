# 🌌 VoidLink

> “When the world goes quiet, let the void speak.”

**VoidLink** is a sci-fi inspired, LoRa-based mesh communication system built on ESP32 microcontrollers. Designed to function in off-grid environments (like festivals, wilderness treks, or emergencies), VoidLink enables direct device-to-device chat without cellular or internet infrastructure. With support for keyboard input, BLE-based discovery, and OLED message display, it’s your walkie-talkie’s smarter cousin from space.

---

## 🚀 Features

- 📡 LoRa-based mesh communication (no internet or cell service required)
- 🧠 Store-and-forward packet routing
- 🎛️ On-device UI: message input, history, recipient selection
- 🔋 Battery-powered with power-saving modes
- 📲 Bluetooth Low Energy (BLE) for mobile pinging & discovery
- 🔐 Optional AES or XOR encryption
- 💬 OLED display or serial fallback for messages

---

## 🛠️ Hardware Requirements

- ESP32 with LoRa support (e.g., TTGO LoRa32 or Heltec WiFi LoRa 32)
- OLED screen (optional, I2C)
- LiPo battery + BMS for mobile power
- Optional: small physical keyboard (matrix, I2C, or GPIO)
- Optional: BLE module (if ESP32 model lacks built-in BLE)

---

## 📦 Project Structure

This project is broken into 5 epics over 30 days of development. Each task can be tracked via GitHub issues or your preferred Kanban board.

### 📁 Epic 1: Hardware Setup & Communication
- Research and purchase ESP32 LoRa boards
- Flash "Hello World" LED sketch
- Test LoRa sender/receiver with hardcoded messages
- Log RSSI/SNR for signal diagnostics
- Begin BLE hardware setup

### 💬 Epic 2: Chat Functionality
- Add message input via serial or keyboard
- Chunk long messages for LoRa packets
- Display received messages via OLED or serial
- Add metadata (timestamps, usernames)
- Set up BLE pinging between mobile and device

### 🌐 Epic 3: Mesh Networking Logic
- Design packet structure
- Implement store-and-forward routing
- Prevent loops via packet ID tracking
- Test 3-node routing
- Add broadcast/direct messaging modes

### 🎛️ Epic 4: UX & Power Optimization
- On-device navigation/menu system
- Store message history in EEPROM/Flash
- Add deep sleep functionality
- Add battery support and status indicator
- Optimize BLE connection and power handling

### 🎥 Epic 5: Demo & Docs
- Record demo video
- Write full GitHub setup guide
- Write optional blog/devlog
- Implement encryption (XOR/AES)
- Add device discovery (BLE ping nearby)

---
