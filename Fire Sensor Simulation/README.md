# Fire Sensor Simulation

## Overview
This Arduino-based simulation monitors environmental conditions using a temperature sensor and a photoresistor to detect potential fire hazards. It processes sensor data and activates an LED alarm when thresholds are exceeded.

## Components Used
- **Temperature Sensor (Analog Pin A0)**: Reads environmental temperature.
- **Photoresistor (Analog Pin A2)**: Measures brightness levels.
- **LED Indicator (Pin 12)**: Activates when a fire condition is detected.

## Fire Detection Logic
- **Temperature Threshold**: 50°C
- **Brightness Threshold**: 220 (arbitrary scale)
- If both temperature and brightness exceed their set thresholds, the LED alarm is triggered.

## Serial Monitoring
The system outputs real-time temperature and brightness values to the Serial Monitor for tracking and debugging.

## How to Use
1. Upload the provided `.ino` file to your Arduino board.
2. Connect the temperature sensor and photoresistor to the appropriate analog pins.
3. Monitor the Serial output to see real-time readings.
4. If fire conditions are met, the LED will turn on.

