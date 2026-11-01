# terra-x 🌾
> Modular Agricultural Intelligence & Autonomous Planting System

`terra-x` is a dual-module precision agriculture hardware system designed to combine drone-based land assessment with ground-based precision seeding and micro-fertilization.

---

## 🚀 Key Modules

### 1. Reconnaissance Module (Drone Attachment)
- **Terrain Scanning:** Uses ultrasonic telemetry to evaluate surface topology (flat vs. slanted vs. uneven).
- **Soil Analysis:** Drops to lower altitude to sample soil moisture levels (dry, optimum, wet) and transmits data to the farm management hub.
  <img width="4032" height="1908" alt="20261031_145110" src="https://github.com/user-attachments/assets/39d1d982-c856-4d39-bd52-aac308d6ffc1" />
<img width="4032" height="1908" alt="20261031_145121" src="https://github.com/user-attachments/assets/dc04791f-25fb-4370-8086-92d9750f37e9" />

## System Schematics & Explanation

### Module 1: Reconnaissance (Drone Attachment)
This module handles the terrain and soil scanning using an Arduino Uno. 

![Recon Pod Schematic](https://github.com/leulesisay05-hub/Terra-X-/blob/main/Terra-x/schematics/recon_pod_module1.png)

**Circuit Explanation:**
* **HC-SR04 Distance Sensor:** Connected to the Arduino digital pins to trigger and receive ultrasonic pulses for height detection.
* **Moisture Sensor:** Connected to an Analog pin (like A0) to read the changing voltage based on soil wetness.
* **OLED Display:** Uses I2C communication (SDA and SCL pins) to print out real-time stats locally.


## System Schematics & Explanation

### Module 2: Action (Rover / Gantry Attachment)
This module coordinates the mechanical digging, seed dropping, and watering system.

![Action Pod Schematic](https://github.com/leulesisay05-hub/Terra-X-/blob/main/Terra-x/schematics/Action_pod_module2.png)

**Circuit Explanation:**
* **Continuous Servo (Drill):** Spins 360 degrees to power the auger drill mechanism into the soil.
* **Standard SG90 Servo (Gate):** Moves from 0 to 180 degrees to open and close the seed dispenser chute.
* **5V Fluid Pump & Relay:** The relay acts as an electronic switch. The Arduino signals the relay, which safely connects the external power source to turn on the water pump without damaging the Arduino.


### 2. Action Module (Rover / Gantry Attachment)
- **Precision Seeding:** Uses an auger drill powered by a 360° continuous rotation servo to dig planting holes.
- **Automated Gate:** Actuates a 180° servo to dispense seeds cleanly.
- **Micro-Dosage:** Triggers a relay-controlled DC pump to apply precise water/fertilizer doses per seed.
  <img width="1908" height="4032" alt="20261031_145207" src="https://github.com/user-attachments/assets/8b5bbd7d-f107-44eb-b511-5308394ffe9a" />
<img width="4032" height="1908" alt="20261031_145141" src="https://github.com/user-attachments/assets/898a9662-a89e-4dcf-b180-54b8b31de4af" />


---

## 📁 Repository Navigation
- [`BOM.md`](./BOM.md) — Complete hardware components list.
- [`JOURNAL.md`](https://github.com/leulesisay05-hub/Terra-X-/blob/main/%23%20terra-x_Development_Journal%20%F0%9F%93%9D.md) — Hourly build log and technical progress notes.
- [`/firmware`](https://github.com/leulesisay05-hub/Terra-X-/tree/main/Terra-x/firmware) — Arduino code for Recon and Action modules.
- [`/schematics`](https://github.com/leulesisay05-hub/Terra-X-/tree/main/Terra-x/schematics) — Circuit connection maps and wiring layouts.

