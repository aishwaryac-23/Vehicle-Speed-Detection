# Vehicle Speed Detection System

This project implements a Vehicle Speed Detection System using an ESP32 microcontroller, infrared (IR) sensors, and an LCD display. The system measures the speed of vehicles passing between two IR sensors and alerts the user if the speed exceeds a predefined limit.

## Table of Contents
- [Hardware Requirements](#hardware-requirements)
- [Software Requirements](#software-requirements)
- [Installation Instructions](#installation-instructions)
- [Usage Instructions](#usage-instructions)
- [Schematic Diagram](#schematic-diagram)
- [Troubleshooting](#troubleshooting)
- [License](#license)

## Hardware Requirements
- **ESP32 Microcontroller**
- **IR Sensors** (2 pieces)
- **LCD Display** (I2C compatible)
- **Buzzer**
- **Breadboard and Jumper Wires**
- **Power Supply** (USB or Battery)

## Software Requirements
- **Arduino IDE**: Make sure to have the latest version installed.
- **LiquidCrystal_I2C Library**: This library is required for interfacing with the LCD. Install it via the Library Manager in Arduino IDE.

## Installation Instructions
1. **Install Arduino IDE**:
   - Download and install Arduino IDE from [Arduino's official website](https://www.arduino.cc/en/software).
  
2. **Install the LiquidCrystal_I2C Library**:
   - Open Arduino IDE.
   - Go to **Sketch > Include Library > Manage Libraries**.
   - Search for "LiquidCrystal_I2C" and install the library.

3. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/VehicleSpeedDetectionSystem.git
   cd VehicleSpeedDetectionSystem
   
4. **Open the Project**:
Open the Arduino IDE.
Navigate to File > Open and select the main source code file (e.g., vehicle_speed_detection.c).
Usage Instructions
Connect the components according to the wiring diagram provided in the schematic section.
Upload the code to the ESP32 microcontroller.
Open the Serial Monitor in the Arduino IDE to view any debug messages.
As a vehicle passes between the two IR sensors, the speed will be calculated and displayed on the LCD.
If the speed exceeds 50 Km/Hr, the buzzer will sound to indicate overspeeding.

6. **Schematic Diagram**
https://github.com/aishwaryac-23/Vehicle-Speed-Detection/blob/main/semantic_diagram.png

7. **Troubleshooting**
No display on LCD:

Ensure the I2C connections are correct.
Check the I2C address (0x27) in the code; it may vary based on your module.
Buzzer not sounding:

Check the buzzer connection and ensure it is functional.
Speed not calculated:

Verify that the IR sensors are correctly positioned and detecting the vehicle.
