# VTX-200 Wind Tunnel UI

A sleek, responsive React dashboard for real-time monitoring and recording of a laboratory wind tunnel’s sensor data, designed for the Simteq VTX-200 desktop wind tunnel.

<img width="1860" height="948" alt="image" src="https://github.com/user-attachments/assets/c8f2c247-0eab-4b3a-bece-273edb6bef0c" />

## Overview

The VTX-200 UI is a powerful web-based dashboard for real-time monitoring, data logging, and control of the VTX-200 wind tunnel system.
The web app is pre-installed on your wind tunnel hardware—no extra setup is needed.

## Features

- Live data visualization from ESP32 via WebSocket (strain gauges, pressure sensors, angle of attack, wind speed, etc.)
- Beautiful, modern dashboard layout with modular cards and charts
- Toggle between wall and floor readings for strain data
- Record and download CSV data for experiments with a single click
- Zero (tare) strain gauges remotely from the UI

## Accessing the Web App

1. **Power on your VTX-200 wind tunnel controller.**
2. **Connect your device (PC, Mac, tablet, or phone) to the WiFi network:**
    - **SSID:** `WindTunnel_AP`
    - **Password:** `12345678`
3. **Open a web browser** and go to:  
   [http://192.168.4.1](http://192.168.4.1)
4. The dashboard will load automatically.

## Dashboard Layout

- **Lift and Drag Card:**  
  Real-time chart of wall or floor balance readings.  
  Toggle between "Wall" and "Floor" with the buttons.
- **Pressure Card:**  
  Displays current pressure sensor reading (e.g., pitot tube).
- **Angle of Attack Card:**  
  Shows the current angle of attack (AOA).
- **Wind Speed Card:**  
  Displays real-time wind speed.

## Controls

- **Start Recording**  
  Begins logging sensor data for download.
- **Stop Recording**  
  Stops logging.
- **Download CSV**  
  Downloads your recorded data in CSV format for further analysis (Excel, MATLAB, etc.).
- **Zero Scales**  
  Tares the strain gauges (sets the current force reading as zero). Use when the model is stationary.

## Interpreting Data

- **Lift/Drag Values:**  
  Measured in grams (g) or Newtons (N), as configured on your device.
- **Pressure:**  
  Dynamic or static pressure from the tunnel’s sensors.
- **Angle of Attack:**  
  The model’s current orientation, in degrees (°).
- **Wind Speed:**  
  Measured in meters per second (m/s).

## Common Commands (Sent by the UI)

- `"tare"`: Sent when "Zero Scales" is clicked. The controller zeroes all strain gauges.

## Best Practices

- Always zero (tare) the strain gauges before starting a test.
- Wait for readings to stabilize before recording data.
- Download your CSV file after each recording session.

## Troubleshooting

- **Web app doesn’t load:**  
    - Make sure you are connected to `WindTunnel_AP` WiFi.
    - Ensure the controller is powered on.
    - Try refreshing your browser or a different device.
- **No live data:**  
    - Check that all hardware and sensors are properly connected.
    - Try zeroing the scales if readings are stuck.

## Contact & Support

For technical support, contact **Simteq Engineering**:  
[info@simteq.co.za](mailto:info@simteq.co.za)  
[www.simteq.co.za](https://www.simteq.co.za/)

## Changelog

- See the app dashboard for software version and update notices.


> **Note:** This software is packaged with the VTX-200 product and is intended only for use with authorized Simteq Engineering hardware.
