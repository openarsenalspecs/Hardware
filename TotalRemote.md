# TotalRemote

**One remote for every TV.**

TotalRemote is an open-source universal control system for televisions and display devices. It unifies multiple control methods—IR, HDMI-CEC, Wi-Fi/LAN smart TV APIs, and extensible plugins—into a single modular platform.

It is designed as a **local-first, plugin-driven control engine**, not just a remote control app.

---

## Features

### 🧠 Unified Control System
- Single command interface for all devices
- Standardized commands across brands and protocols:
  - power_on / power_off
  - volume_up / volume_down
  - mute / unmute
  - input switching (HDMI, AV, etc.)
- Abstracts differences between manufacturers into one control layer

---

### 🔌 Plugin-Based Architecture
- Fully modular backend system
- Each control method is a plugin:
  - LG webOS TVs
  - Samsung Tizen TVs
  - Roku devices
  - Android TV / Google TV (ADB / network control)
  - HDMI-CEC
  - Infrared (IR blasters)
- Hot-swappable plugin support
- Community extensible architecture

---

### 🔍 Device Discovery
- Automatic detection of TVs and displays via:
  - mDNS / Bonjour
  - SSDP / UPnP
  - Local network scanning fallback
  - Bluetooth discovery (where supported)
- Device fingerprinting and auto-identification
- Persistent device profiles per household

---

### 🔁 Smart Fallback Control Chain
If one method fails, TotalRemote automatically retries using alternate layers:

1. Wi-Fi / LAN control
2. HDMI-CEC
3. Infrared (IR)

This ensures maximum compatibility across devices and environments.

---

### 📱 User Interface Features
- Universal adaptive remote interface
- Multi-TV dashboard (control all screens in one place)
- Gesture-based controls (swipe volume, channel switching)
- Favorite shortcuts (Netflix, HDMI 1, mute, etc.)
- Device-aware dynamic UI layouts

---

### 🏠 Smart Home Integration

TotalRemote is designed as a smart home control node, integrating directly with automation systems.

#### Home Assistant Integration
- Native integration via REST + MQTT
- TVs exposed as smart entities
- Real-time bidirectional state synchronization

#### MQTT Support
- Event publishing:
  - tv/{device}/power
  - tv/{device}/input
  - tv/{device}/volume
- Command subscription for automation systems

#### Automation Engine
Trigger workflows based on TV state changes:
- TV turns on → dim lights
- Input changes → switch room mode
- Playback pause → restore ambient lighting

#### Smart Scenes
- Movie Mode (TV + lighting + audio configuration)
- Game Mode (low latency + input switching)
- Night Mode (shutdown + environment reset)

#### Optional Voice Assistant Bridges
- Google Home integration (via bridge layer)
- Apple HomeKit integration (optional module)
- Voice commands for basic TV control

---

### 🌐 Network & Intelligence Layer
- Zero-config onboarding experience
- Real-time device state tracking
- WebSocket-based live updates
- Network topology awareness
- Local-first architecture (no cloud required)

---

### 🔐 Advanced Features
- Macro system (command sequences)
- REST + WebSocket API
- CLI tool (`totalremote ctl`)
- Full device state tracking engine
- Debugging console and logs
- Plugin health monitoring system

---

### 🔊 Hardware Expansion Support
- ESP32 IR blaster integration
- Multi-room IR node networks
- IR learning / capture mode
- Community-shared IR code library

---

### 🚀 Key Differentiators
- Smart fallback across multiple control methods
- Fully plugin-based TV ecosystem
- Unified cross-brand command system
- Multi-TV control dashboard
- Local-first privacy architecture
- Deep smart home integration (not just casting or mirroring)

---

## Architecture Overview

```text
User Interface
      ↓
Command Abstraction Layer
      ↓
Core Control Engine
      ↓
Device Plugins
   ├── IR Systems
   ├── HDMI-CEC
   ├── Smart TV APIs (LG / Samsung / Roku / Android TV)
      ↓
Smart Home Integration Layer
   ├── Home Assistant
   ├── MQTT Broker
   ├── Automation Engine
   └── Voice Assistant Bridges
   ```

## Getting Started (WIP)

Setup instructions, installation guides, and platform-specific builds will be added as the project reaches MVP stage.

Planned setup paths include:

- Local development environment (core engine + plugins)
- Docker-based deployment for home networks
- Raspberry Pi / low-power home hub setup
- Optional mobile client builds (iOS / Android)

---

## Project Vision

TotalRemote aims to become a **universal control layer for all television and display systems**, replacing fragmented remote ecosystems with a single, extensible open-source platform.

It is designed to unify:
- Smart TVs
- Legacy infrared-controlled TVs
- HDMI-connected devices
- Streaming devices and set-top boxes

into one consistent control experience.

---

## Specification Branding License (SBL)

### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/totalremote/](https://roxanneardary.com/totalremote/)

---

## License & Notice Requirements

TotalRemote is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- TotalRemote specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
