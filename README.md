# Smart-Temperature-Monitor

A basic Embedded Systems and IoT project built using Arduino UNO and a TMP36 temperature sensor. The system continuously monitors ambient temperature, displays readings on a 16×2 LCD, and generates visual and audio alerts when predefined temperature thresholds are exceeded.

## Overview

This project was developed to strengthen fundamental embedded systems concepts such as sensor interfacing, microcontroller programming, LCD communication, and threshold-based decision making.

The system reads temperature data from a TMP36 analog temperature sensor, converts it into degrees Celsius, and displays the value on an LCD screen. LEDs and a buzzer provide immediate feedback when the temperature moves outside the normal operating range.

## Components Used

* Arduino UNO
* TMP36 Temperature Sensor
* 16×2 LCD Display
* Green LED
* Red LED
* Piezo Buzzer
* 220Ω Resistors
* Breadboard and Jumper Wires

## Features

* Real-time temperature monitoring
* LCD temperature display
* High temperature alert
* Low temperature alert
* Visual indication using LEDs
* Audio indication using buzzer
* Serial Monitor output for debugging

## Circuit Connections

### TMP36 Sensor

| TMP36 Pin | Arduino |
| --------- | ------- |
| VCC       | 5V      |
| VOUT      | A0      |
| GND       | GND     |

### LCD Connections

| LCD Pin | Arduino Pin   |
| ------- | ------------- |
| RS      | 12            |
| E       | 11            |
| D4      | 5             |
| D5      | 4             |
| D6      | 3             |
| D7      | 2             |
| VSS     | GND           |
| VDD     | 5V            |
| RW      | GND           |
| VO      | Potentiometer |

### LEDs and Buzzer

| Component | Arduino Pin |
| --------- | ----------- |
| Green LED | 8           |
| Red LED   | 9           |
| Buzzer    | 10          |

## Working Principle

1. The TMP36 sensor measures ambient temperature.
2. Arduino reads the analog voltage from the sensor.
3. The voltage is converted into temperature in Celsius.
4. Temperature is displayed on the LCD.
5. The system compares the temperature against predefined thresholds:

   * Above 30°C → High Temperature Alert
   * Below 15°C → Low Temperature Alert
   * Between 15°C and 30°C → Normal Condition
6. LEDs and buzzer indicate the current status.

## Software

* Arduino IDE
* Embedded C/C++
* LiquidCrystal Library
* Tinkercad Circuits (for simulation)

## Future Improvements

* Wi-Fi connectivity using ESP32
* Cloud data logging
* Mobile application integration
* Temperature trend visualization
* Multi-sensor environmental monitoring

## Learning Outcomes

* Embedded Systems Fundamentals
* Arduino Programming
* Sensor Interfacing
* LCD Communication
* Analog-to-Digital Conversion
* Threshold-Based Control Systems
* Circuit Simulation and Testing


