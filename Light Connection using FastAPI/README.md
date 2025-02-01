# Light Arduino Project

## Overview
This Arduino-based project controls an LED light using FastAPI. A Python backend communicates with an Arduino via serial connection to toggle the LED on and off.

## Components Used
- **Arduino Board**
- **LED (Digital Pin)**
- **Python FastAPI Backend**
- **Serial Communication via `pyserial`**

## API Endpoints
- `POST /led/on` → Turns the LED ON
- `POST /led/off` → Turns the LED OFF

## Setup Instructions
1. Upload the `light_arduino.ino` file to your Arduino board.
2. Run `connection.py` using FastAPI and ensure `pyserial` is installed.
3. Use API calls to control the LED.

## Running the FastAPI Server
1. Install dependencies:  
   ```sh
   pip install fastapi uvicorn pyserial
   ```
2. Start the FastAPI server:  
   ```sh
   uvicorn connection:app --reload
   ```
3. Ensure the Arduino is connected to the correct COM port.
