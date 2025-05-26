# MPU6050 Sensor Module PCB

This repository contains the design files for a custom PCB built around the **MPU6050** 6-axis motion tracking sensor. The PCB is designed to be compact and easy to integrate with microcontrollers via I2C. It includes necessary supporting components such as decoupling capacitors and pull-up resistors for stable operation.

## Features

- MPU6050 (3-axis gyroscope + 3-axis accelerometer)
- I2C interface (via header J1)
- Power LED indicator (LED1)
- Onboard decoupling capacitors (C1–C7)
- Pull-up resistors for I2C (R1, R2)
- Compact 2-layer PCB layout

## Components

- **U1**: MPU6050
- **J1**: I2C header for connection to a microcontroller
- **R1–R4**: Resistors (I2C pull-ups, LED resistor)
- **C1–C7**: Capacitors (decoupling and filtering)
- **LED1**: Power indicator
- **U2**: Optional footprint (e.g., voltage regulator or logic-level converter)

## Getting Started

1. Connect the module to your microcontroller via the I2C header (J1).
2. Provide 3.3V or 5V power (depending on configuration).
3. Use any MPU6050-compatible library (e.g., [Arduino MPU6050 library](https://github.com/jrowberg/i2cdevlib/tree/master/Arduino/MPU6050)) to begin reading sensor data.

## Schematic & PCB

The KiCAD/other EDA project files are located in the `hardware/` directory.

## License

This project is open-source under the MIT License.

