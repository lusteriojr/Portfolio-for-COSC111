# Arduino LED PWM Control

This Arduino project controls multiple LEDs using Pulse Width Modulation (PWM) to create a fading effect. The LEDs gradually increase in brightness one by one.

## 📌 Features
- Controls 5 LEDs connected to Arduino.
- Uses **PWM** for smooth brightness transitions.
- Implements a loop that fades LEDs in sequence.

# 🛠️ Components Used
- Arduino Board(Uno, Mega, etc.)
- 5 LEDs
- Resistors (220Ω)
- Jumper Wires

## 🔧 How It Works
1. The program initializes LED pins as **output** in `setup()`.
2. Inside `loop()`, it gradually increases the brightness of each LED using `analogWrite()`.
3. Once one LED reaches full brightness, it moves to the next.
