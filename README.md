# VTX-200 Wind Tunnel UI – User Manual

[![Docs Status](https://img.shields.io/badge/docs-stable-success)](#)
[![Docs Version](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2F<ORG>%2F<REPO>%2Fmain%2Fdocs%2Fversion.json&label=docs%20version&query=%24.version&prefix=v)](CHANGELOG.md)
[![Issues](https://img.shields.io/github/issues/<ORG>/<REPO>)](https://github.com/<ORG>/<REPO>/issues)
[![Discussions](https://img.shields.io/github/discussions/<ORG>/<REPO>)](https://github.com/<ORG>/<REPO>/discussions)
[![License](https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-informational)](LICENSE)

This repository is the **official instruction manual** for the VTX-200 Wind Tunnel Web App, developed by **Simteq Engineering**.  
> **Note:** This repository contains **documentation only**. The VTX-200 UI software is proprietary and distributed with authorized hardware.

---

## Overview

The VTX-200 UI is a web-based dashboard for real-time monitoring, data logging, and control of the VTX-200 wind tunnel system.  
The web app is **pre-installed** on your wind tunnel hardware—no extra setup is needed.

---

## Accessing the Web App

1. Power on your VTX-200 wind tunnel controller.  
2. Connect to Wi-Fi:
   - **SSID:** `WindTunnel_AP`
   - **Password:** `12345678`
3. In a browser, open: `http://192.168.4.1`

---

## Dashboard Layout

- **Lift & Drag Card** – Real-time wall/floor balance readings; toggle “Wall/Floor”.
- **Pressure Card** – Dynamic/static pressure (e.g., pitot).
- **Angle of Attack Card** – Current AOA in degrees.
- **Wind Speed Card** – Real-time airspeed (m/s).

---

## Controls

- **Start Recording** – Begin logging sensor data.
- **Stop Recording** – Stop logging.
- **Download CSV** – Export recorded data for Excel/MATLAB/etc.
- **Zero Scales** – Tare strain gauges with the model stationary.

**Command sent by UI:** `"tare"` when “Zero Scales” is clicked.

---

## Interpreting Data

- **Lift/Drag** – grams (g) or Newtons (N) (device-configured).  
- **Pressure** – From tunnel sensors.  
- **AOA** – Degrees (°).  
- **Wind Speed** – m/s.

---

## Best Practices

- Tare (zero) before each test.  
- Let readings stabilize before recording.  
- Download CSV after each session.

---

## Troubleshooting

- **App doesn’t load** – Ensure Wi-Fi (`WindTunnel_AP`) and power; refresh or try another device.  
- **No live data** – Check hardware/sensor connections; try Zero Scales.

---

## Changelog & Versioning

- **Docs version badge** (top of page) tracks the file `docs/version.json` which is **automatically updated** when Simteq publishes a new software release.
- The **CHANGELOG** below lists user-facing changes that affect operation.

See: [Changelog](#) and [`CHANGELOG.md`](CHANGELOG.md).

---

## Community

- **Issues** – Report bugs, ask questions, and request features.  
- **Discussions** – Q&A, ideas, and announcements.

Before filing an issue, please read our [CONTRIBUTING](CONTRIBUTING.md) guide and [SUPPORT](SUPPORT.md).

---

## Contact & Support

**Simteq Engineering**  
📧 [info@simteq.co.za](mailto:info@simteq.co.za)  
🌐 https://www.simteq.co.za

---

## License (Docs Only)

Documentation is licensed under **CC BY-NC-SA 4.0**.  
The VTX-200 UI software is **not** open source and is distributed only with authorized hardware.
