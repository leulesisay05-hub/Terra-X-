# terra-x Development Journal 📝

## Phase 1: Prototype Assembly & AI Integration (Hackathon Phase)
- **Goal:** Build a functional proof-of-concept dual-module system (Recon & Action) within 3 days.
- **What was accomplished:**
  - Configured Arduino Uno with Ultrasonic distance sensor to map terrain levels (flat/slanted).
  - Interfaced Soil Moisture sensor with OLED display for field diagnostics.
  - Assembled Action module using 360° servo for auger digging, 180° servo for seed release, and relay-driven water pump.
  - Leveraged AI assistance for rapid iteration of sensor thresholds and motor control logic.
- **Challenges Overcome:** Pin allocation conflicts between OLED display communication and servo control; resolved through pin mapping adjustments.

## Phase 2: Refinement & Repository Migration
- **Goal:** Clean up hardware schematics, isolate firmware modules, and document project architecture for public review.