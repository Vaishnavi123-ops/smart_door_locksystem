# Iot Door Lock Using Arduino Uno, LCD I2C, 4x4 Keypad, and 12V Solenoid Door Lock

## Project Overview
This project demonstrates an **IOT Door Lock System** that uses an **Arduino Uno**, a **4x4 Keypad**, an **LCD I2C display**, and a **12V Solenoid Door Lock** for secure access control. The system allows authorized users to enter a predefined PIN code on the keypad to unlock the door. The status of the lock is displayed on the LCD screen. It’s a simple yet effective security system for home or office doors.

### Key Features
- **PIN-based Access**: Users enter a PIN code on the 4x4 keypad to unlock the door.
- **LCD Display**: Shows the status of the door (locked/unlocked) and any messages (e.g., "Access Granted").
- **12V Solenoid Lock**: Controls the locking mechanism of the door.
- **Secure Authentication**: Only users who input the correct PIN code can unlock the door.
- **Easy Setup**: The system is built using an Arduino Uno, which is easy to program and interface with other hardware components.

## Components Used
- **Microcontroller**: Arduino Uno
- **Keypad**: 4x4 Matrix Keypad (for PIN code input)
- **LCD Display**: 16x2 LCD with I2C interface
- **Locking Mechanism**: 12V Solenoid Lock
- **Relay**: Used to control the 12V solenoid lock with the Arduino (optional if using a transistor).
- **Power Supply**: 5V for Arduino and 12V for Solenoid Lock.
- **Wires and Jumper Cables**: For connecting components.

## Getting Started

### Prerequisites
- **Hardware**:
  - Arduino Uno
  - 4x4 Matrix Keypad
  - LCD 16x2 I2C Display
  - 12V Solenoid Lock
  - Relay module (if needed for controlling the solenoid lock)
  - Power Supply: 12V DC for the solenoid lock, 5V USB for Arduino
  - Jumper Wires

- **Software**:
  - Arduino IDE
  - Keypad library (`Keypad.h`)
  - LCD I2C library (`Wire.h`, `LiquidCrystal_I2C.h`)

### Setting Up the Hardware
1. **Keypad**: Connect the 4x4 matrix keypad to the Arduino. The rows and columns of the keypad are connected to specific digital pins on the Arduino.
2. **LCD I2C Display**: Connect the LCD to the Arduino via the I2C interface. Typically, the I2C pins are connected to the SDA and SCL pins of the Arduino.
3. **Solenoid Lock**: Connect the 12V solenoid lock to a relay or directly to the power supply if it’s a low-current lock. Use a transistor if required.
4. **Power Supply**: The Arduino Uno should be powered by a 5V USB or power adapter, while the solenoid lock requires a 12V power source.

### Wiring Diagram
Here’s a simple schematic:
- **Keypad Pins**: Connect the 4x4 keypad’s rows and columns to Arduino pins (for example, pins 2-9).
- **LCD I2C**: Connect the SDA and SCL pins of the LCD to the corresponding SDA and SCL pins of the Arduino (A4 and A5 on Arduino Uno).
- **Relay Module**: If using a relay, connect the control pin to an Arduino digital pin (e.g., pin 10) and connect the relay to the 12V solenoid lock.

### Software Setup
Install the required libraries in the Arduino IDE:
   - **Keypad Library**: `Sketch > Include Library > Manage Libraries` and search for `Keypad` to install.
   - **LiquidCrystal I2C Library**: `Sketch > Include Library > Manage Libraries` and search for `LiquidCrystal I2C` to install.
   
