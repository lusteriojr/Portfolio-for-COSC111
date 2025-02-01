# Photoresistor (LDR) Arduino Project

## Overview
This project uses a **photoresistor (Light Dependent Resistor - LDR)** to measure ambient light intensity and interact with an Arduino microcontroller. The program reads analog values from the LDR and can trigger actions based on the detected light levels.

## Components Required
- **Arduino Board** (Uno, Mega, or compatible)
- **Photoresistor (LDR)**
- **Resistor (typically 10kΩ)**
- **Jumper Wires**
- **Breadboard**
- (Optional) **LED or Buzzer** for visual/audio feedback

## Circuit Connection
1. Connect **one leg of the LDR** to **5V** on the Arduino.
2. Connect **the other leg of the LDR** to an **analog input pin (e.g., A0)** and also to **GND via a 10kΩ resistor** (voltage divider setup).
3. (Optional) Connect an **LED to a digital output pin** to turn on/off based on light levels.

## Code Explanation
The **photoresistor.ino** script performs the following tasks:
1. Reads the **analog value** from the LDR sensor.
2. Converts the analog reading into a light intensity level.
3. Displays the sensor readings in the **Serial Monitor**.
4. (Optional) Controls an LED or another actuator based on light conditions.

## Usage
1. **Upload** the `photoresistor.ino` file to your Arduino board using the Arduino IDE.
2. **Open the Serial Monitor** (`115200 baud rate` recommended) to observe real-time light intensity values.
3. Modify threshold values in the code to trigger different actions.

## Example Output
```
Light Level: 850
Light Level: 760
Light Level: 920
```

## Customization
- Adjust **threshold values** to make the LDR more or less sensitive.
- Modify the code to activate an **LED, buzzer, or relay** when light conditions change.
- Implement **data logging** to store readings over time.

## Troubleshooting
- If readings are always high or low, check the **resistor value** in the voltage divider.
- Ensure correct **analog pin connections** and that the **LDR is functioning properly**.
