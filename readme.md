# Pimp My Ride - Part 3

## Arduino Speedometer and NeoPixel FastLED Strip

This project combines a speedometer functionality with an LED light controller for a bicycle or similar vehicle. It uses an Arduino board to read speed data from a magnetic sensor and control a series of LED light patterns.

## Project Progress Videos

[![Video Title](https://img.youtube.com/vi/NTwoWGXgmiA/0.jpg)](https://www.youtube.com/watch?v=NTwoWGXgmiA)


## Task List

Here's a task list for further development of the project:

* [x] iNtErgRaTiOn (just for making fun of myself bcz in a hurry i couldn't type "integration" properly)
* [x] Implement basic speedometer functionality
* [x] Set up LCD display for speed and distance
* [x] Integrate WS2812B LED strip control
* [x] Create multiple LED patterns
* [x] Implement brake light feature
* [ ] Optimize code for better performance
* [ ] Implement power-saving features
* [x] Create a PCB design for a more compact build
* [ ] Develop a weatherproof enclosure
* [ ] Add Bluetooth connectivity for mobile app control
* [ ] Implement data logging feature
* [ ] Create user manual and assembly instructions
* [x] ✨**ENJOY**✨

## Features

1. Speedometer
    * Calculates and displays current speed
    * Tracks total distance traveled
    * Shows total time in motion
2. LED Light Controller
    * Multiple light patterns for visibility and aesthetics
    * Turn signal and brake light functionality
    * Customizable LED colors and patterns

## Hardware Requirements

* Arduino board (e.g., Arduino Uno)
* LCD display (16x2 characters)
* Magnetic sensor (Hall effect sensor)
* WS2812B LED strip
* Buttons for mode selection and turn signals
* Appropriate resistors and wiring

For a complete list of parts, refer to `tinkerCADParts list.png` in the project root.

## Wiring Diagram and Schematic

* The circuit diagram can be found in `tinkerCAD circuit diagram.png`
* The schematic is available in `tinker_cad-schematics.png`
* For the PCB design, refer to `KiCAD PCB screenshot.png`

For the most up-to-date schematic and PCB design, open the following files in KiCad:

* Schematic: `intergration/integration-arduino-shield/integration.kicad_sch`
* PCB: `intergration/integration-arduino-shield/integration.kicad_pcb`

## Libraries Used

* FastLED
* LiquidCrystal

## Pin Configuration

* LCD: pins 13, 12, 11, 10, 9, 8
* Magnetic sensor: pin 7
* LED strip data: pin 3
* Right turn signal button: pin 4
* Left turn signal button: pin 5
* Brake signal: pin 2
* Mode selection button: pin 13
* Main control button: pin 12

## Setup

1. Connect all components according to the pin configuration.
2. Install the required libraries in your Arduino IDE.
3. Upload the provided code to your Arduino board.
4. Adjust the `Wheel_circumference_in_Cm` constant to match your wheel size.

## Usage

* The speedometer will automatically start tracking when motion is detected.
* Use the mode selection button to cycle through different LED patterns.
* Use the turn signal buttons to activate left or right turn signals.
* The brake light will activate automatically when the brake signal is received.

## Customization

You can customize the LED patterns by modifying the `Pattern1()` through `Pattern9()` functions in the code. Adjust colors, timing, and sequences to create your desired effects.

## Project Structure

``` bash
PimpMyRide/
│
├── intergration/
│   ├── integration-arduino-shield/ (run the .pcb & .sch files from here)
│       ├── integration.kicad_sch
│       ├── integration.kicad_pcb
│
├── intergration.ino (the main arduino file to run)
├── tinkerCAD circuit diagram.png
├── tinkerCADParts list.png
├── tinker_cad-schematics.png
├── KiCAD PCB screenshot.png
└── README.md
```

## Note

This project combines multiple functionalities and may require fine-tuning based on your specific hardware setup and requirements. Always ensure proper visibility and adhere to local regulations when using this on public roads.