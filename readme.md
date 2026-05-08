# ESP32 Camera Ball with GPT

An open ESP32-S3 spherical robot build based on the ESP-ROLL idea, extended with camera/audio input, distance and temperature sensing, a speaker, a laser module, and cloud-based voice Q&A.

This started as a learning project after reading discussions from pet owners about separation anxiety. The question I kept coming back to was simple: cameras let us watch pets when we are away, but can a small robot offer some kind of interaction too?

This repository collects the build notes, hardware choices, firmware direction, PCB files, 3D files, and demo media for the prototype.

## Demo

Demo video: coming soon

The original full-resolution video is large, so it is shared as a release asset instead of being committed directly into the repository.

## What It Does

- Rolls inside a 100mm transparent ball using a pendulum-drive mechanism
- Hosts its own Wi-Fi access point for local control
- Captures image and audio from the ESP32-S3 camera/mic setup
- Sends image/audio input to an AI model for voice Q&A
- Converts the response to speech and plays it through an onboard speaker
- Uses distance and temperature sensors for local awareness
- Supports mode switching between normal drive and voice Q&A

## Hardware

- XIAO ESP32-S3
- DRV8833 motor driver
- Two DC motors
- 3D printed PLA/TPU wheels
- VL53L0X distance sensor
- MLX90614 IR temperature sensor
- DFRobot I2S speaker amplifier
- Small speaker
- 3.3V PWM laser module
- AMS1117 3.3V regulator
- 1000mAh LiPo battery
- Custom 2-layer PCB
- 100mm transparent plastic ball

## Project Structure

```text
.
├── firmware/        # ESP32 firmware and control logic
├── hardware/        # Schematics, PCB files, BOM
├── 3d-models/       # Printable parts and mechanical files
├── docs/            # Build notes, wiring notes, setup notes
├── media/           # Small images or compressed preview assets
└── README.md

Demo video: Coming soon
