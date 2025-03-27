
# Folding Wing VTOL Drone

A folding wing VTOL drone powered by a Teensy 4 flight controller and running the DremFlight firmware. This project combines innovative folding wing design for portability with the versatility of VTOL flight—ideal for rapid prototyping, hobby projects, and advanced drone research.

## Overview

This repository contains the source code and build instructions for a folding wing VTOL drone. The drone features:
- **Folding Wing Design:** For easy transport and storage.
- **Vertical Take-Off and Landing (VTOL):** Seamlessly transition between hover and forward flight.
- **Teensy 4 Flight Controller:** A powerful 600 MHz microcontroller ensuring high-speed performance and precise control.
- **DremFlight Firmware:** An open-source flight controller software (based on the dRehmFlight framework) optimized for VTOL operations.

## Features

- **Compact & Portable:** Innovative folding wing design reduces size for transport without sacrificing performance.
- **Hybrid Flight Capabilities:** VTOL functionality with stable hover, transition, and forward flight modes.
- **Advanced Stabilization:** Implements DremFlight’s control algorithms for reliable and responsive flight.
- **Modular Design:** Easy to modify and expand hardware or software for custom drone applications.
- **Open-Source:** Code and documentation available for community collaboration and enhancements.

## Hardware Requirements

- **Main Controller:** Teensy 4.0 (or Teensy 4.1) microcontroller.
- **Inertial Measurement Unit (IMU):** (e.g., MPU6050 or MPU9250) for flight stabilization.
- **Electronic Speed Controllers (ESCs):** Compatible with OneShot125 or standard PWM protocols.
- **RC Receiver:** Supporting PWM, PPM, or SBUS protocols.
- **Folding Wing Airframe:** Custom-built or commercially available airframe that supports VTOL operation.
- **Additional Components:** Battery, wiring, connectors, and mounting hardware.

## Software Requirements

- **DremFlight Firmware:** This firmware is a customized version derived from dRehmFlight, optimized for VTOL and folding wing configurations.
- **Arduino IDE & Teensyduino Add-on:** For compiling and uploading the firmware.
- **Optional Tools:** Calibration utilities and flight simulation software for pre-flight testing.

## Getting Started

### Hardware Assembly

1. **Assemble the Airframe:**
   - Build your folding wing VTOL drone frame following your design specifications.
   - Ensure all moving parts (wings, actuators, etc.) are securely mounted.

2. **Install the Flight Controller:**
   - Mount the Teensy 4 board securely in the drone.
   - Connect the IMU sensor and other peripherals according to your wiring diagram.
   - Verify connections to the ESCs and RC receiver.

### Firmware Setup

1. **Clone the Repository:**
   ```bash
  git clone https://github.com/Shresth-Senwal/PBL.git
   ```

2. **Install Dependencies:**
   - Open the Arduino IDE.
   - Install the required libraries (e.g., the DremFlight library if provided, and any sensor libraries).

3. **Configure the Firmware:**
   - Open `dremflight_config.h` (or similar configuration file) and adjust the parameters to match your hardware setup.
   - Verify settings for IMU scales, motor outputs, and receiver type.

4. **Compile and Upload:**
   - Connect your Teensy 4 via USB.
   - Select the correct board and port in the Arduino IDE.
   - Compile and upload the firmware.

5. **Calibration & Testing:**
   - Open the Serial Monitor at 115200 baud.
   - Run calibration commands (`calimu`, `calradio`, etc.) as described in the firmware documentation.
   - Perform initial tests with the drone grounded before flight.

## Flight Instructions

1. **Pre-Flight Checks:**
   - Confirm all sensors and motor outputs are working.
   - Ensure the folding mechanism is secured in flight mode.
   - Check battery levels and perform safety tests.

2. **Arming & Flight:**
   - Use the configured arming procedure (e.g., low throttle then flip arm switch).
   - Start in hover mode, then test the transition to forward flight.
   - Always follow local regulations and fly in a safe, open area.

## Contributing

Contributions are welcome! If you have suggestions, improvements, or bug fixes, please:
- Fork the repository.
- Create a new branch for your changes.
- Submit a pull request with a clear description of your modifications.

## License

This project is open source and available under the [GPL-3.0 License](LICENSE).

## Acknowledgments

- Inspired by the dRehmFlight project and community efforts in open-source VTOL development.
- Special thanks to the developers and contributors of the Teensy and DremFlight ecosystems.
