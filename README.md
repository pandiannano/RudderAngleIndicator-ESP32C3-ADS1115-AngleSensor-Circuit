# RudderAngleIndicator-ESP32C3-ADS1115-AngleSensor-Circuit

Rudder angle indicator built around an ESP32-C3, an ADS1115 external ADC, and a 0–360° Hall-effect angle sensor (ratiometric 0–3.3V output), powered from a 12V/24V DC marine bus via LM2596 (buck) → AMS1117-3.3 (LDO).

ADC channel assignment:
- **AIN0** — rudder angle sensor signal
- **AIN1** — floating sensor
- **AIN2** — sensor supply sense (Kelvin)
- **AIN3** — sensor ground sense (Kelvin)

See [`docs/HARDWARE-DESIGN.md`](docs/HARDWARE-DESIGN.md) for the full block diagram, per-stage component values, filter/protection circuits, and schematic sheet organization.
