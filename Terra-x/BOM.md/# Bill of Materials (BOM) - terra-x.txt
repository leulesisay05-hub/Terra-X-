# Bill of Materials (BOM) - terra-x 🌾

## Module 1: Reconnaissance (Drone Attachment)
| Component Name | Exact Part / Model | Quantity | Purpose in Project |
| :--- | :--- | :---: | :--- |
| Microcontroller | Arduino Uno Rev3 | 1 | Processes ultrasonic height sensor and soil moisture data |
| Distance Sensor | HC-SR04 Ultrasonic Sensor | 1 | Measures distance to ground to detect flat/slanted/uneven terrain |
| Moisture Sensor | Capacitive / Resistive Soil Moisture Sensor | 1 | Reads soil wetness level (Dry, Optimum, Wet) |
| Display | Grove OLED Display 0.96" | 1 | Shows real-time terrain and soil status locally |

## Module 2: Action (Rover / Gantry Attachment)
| Component Name | Exact Part / Model | Quantity | Purpose in Project |
| :--- | :--- | :---: | :--- |
| Microcontroller | Arduino Uno Rev3 | 1 | Coordinates seed digging, dropping, and watering sequence |
| Actuator (Drill) | 360° Continuous Rotation Servo | 1 | Powers the auger drill mechanism to dig holes |
| Actuator (Gate) | 180° Standard TowerPro SG90 Servo | 1 | Opens and closes the seed gate dispenser |
| Fluid Pump | 5V DC Micro Submersible Water Pump | 1 | Delivers micro-dosage of liquid fertilizer/water |
| Pump Control | 5V 1-Channel Relay Module | 1 | Switches external power to safe water pump operation |

## Power & Interconnects
| Component Name | Exact Part / Model | Quantity | Purpose in Project |
| :--- | :--- | :---: | :--- |
| Power Source | 9V Battery / USB Power Bank | 2 | Independent power for drone and rover microcontrollers |
| Wiring | Jumper Wires (Male-to-Male, Female-to-Female) | ~30 | Interfacing modules, sensors, and actuators |