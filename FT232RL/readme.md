# FT232RL USB-to-Serial Converter Circuit

This repository contains the schematic, PCB layout, and documentation for a USB-to-Serial converter circuit based on the **FTDI FT232RL** chip. This circuit provides a reliable interface between USB ports and UART-based microcontrollers or other TTL serial devices.

## 📦 Features

- USB to UART (TTL level) interface
- Baud rates from 300 bps to 3 Mbps
- 3.3V or 5V logic level operation
- Integrated EEPROM for USB descriptors
- Optional modem control signals (RTS, CTS, DTR, DSR)
- LED indicators for TX and RX
- Standard 6-pin UART header (compatible with Arduino, ESP8266, ESP32, etc.)

## 📁 Files Included

- `schematic/ft232rl_schematic.sch`: Circuit schematic (KiCad)
- `pcb/ft232rl_pcb.kicad_pcb`: PCB layout file
- `gerbers/`: Production-ready Gerber files
- `images/`: Circuit diagrams and board previews
- `docs/FT232RL_datasheet.pdf`: FTDI FT232RL datasheet

## 🧰 Required Components

| Component     | Value / Part Number |
|---------------|----------------------|
| U1            | FT232RL              |
| C1, C2        | 0.1 µF (ceramic)     |
| C3            | 10 µF (electrolytic) |
| R1, R2        | 470 Ω (LED current limiters) |
| D1 (TX LED)   | Red LED              |
| D2 (RX LED)   | Green LED            |
| USB Connector | USB Mini-B / Micro-B |
| Header        | 1x6 Female (GND, CTS, VCC, TXD, RXD, RTS) |

## 🔌 UART Pinout


