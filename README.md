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


### 2. Action Module (Rover / Gantry Attachment)
- **Precision Seeding:** Uses an auger drill powered by a 360° continuous rotation servo to dig planting holes.
- **Automated Gate:** Actuates a 180° servo to dispense seeds cleanly.
- **Micro-Dosage:** Triggers a relay-controlled DC pump to apply precise water/fertilizer doses per seed.
  <img width="1908" height="4032" alt="20261031_145207" src="https://github.com/user-attachments/assets/8b5bbd7d-f107-44eb-b511-5308394ffe9a" />
<img width="4032" height="1908" alt="20261031_145141" src="https://github.com/user-attachments/assets/898a9662-a89e-4dcf-b180-54b8b31de4af" />


---

## 📁 Repository Navigation
- [`BOM.md`](./BOM.md) — Complete hardware components list.
- [`JOURNAL.md`](./JOURNAL.md) — Hourly build log and technical progress notes.
- [`/firmware`](https://github.com/leulesisay05-hub/Terra-X-/tree/main/Terra-x/firmware) — Arduino code for Recon and Action modules.
- [`/schematics`](./schematics/) — Circuit connection maps and wiring layouts.
- [`/images`](./images/) — Build photos and demonstration media.
