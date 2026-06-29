# Arduino Digital Forensics Evidence Extractor

A real-world forensic acquisition tool for Arduino microcontrollers. Extracts
EEPROM memory, GPIO pin states, and analog sensor readings over USB serial —
with automated chain-of-custody documentation and MD5/SHA-256 integrity hashing.

---

## Developed By
- **Er. Abdul Basit**
- Under Guidance of **Dr. Syed Nisar Hussain Bukhari** (Scientist-D, NDU Coordinator)
- NIELIT Deemed to be University — (Srinagar Campus)

---

## Features
- Full EEPROM dump (1 KB, ATmega328P) with hex + ASCII representation
- Digital GPIO snapshot (pins 2–13)
- Analog channel readings (A0–A5) with voltage conversion
- Automated MD5 + SHA-256 integrity hashing
- Complete Chain-of-Custody documentation (FIR No., IO details, examiner info)
- Dark-themed desktop GUI with dashboard, live acquisition, and reports screen
- Stats persistence across sessions (forensic_stats.json)
- Single-file Windows .exe available via build.bat

---

## Components

| File | Description |
|------|-------------|
| `firmware/arduino_forensics.ino` | Arduino firmware — upload this to the device |
| `cli/forensic_extractor.py` | Command-line acquisition script |
| `gui/forensic_gui.py` | Full desktop GUI application |
| `build.bat` | Builds a portable Windows .exe |

---

## Quick Start

### 1. Upload firmware
Open `firmware/arduino_forensics.ino` in Arduino IDE, select your board and port, click Upload.

### 2. Install Python dependency
