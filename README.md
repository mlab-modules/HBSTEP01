# HBSTEP01 - Stepper motor driver

![HBSTEP01B](/doc/img/HBSTEP01B_top_big.jpg)

The HBSTEP01 is a bipolar stepper motor driver module built around the STMicroelectronics L6470 chip. It provides a complete microstepping motor control solution with SPI interface, allowing for precise motor control and advanced motion features.

## Features

* Microstepping up to 1/128 steps
* Operating voltage: 8 V to 45 V
* Maximum output current: 3 A RMS (7 A peak)
* Integrated non-dissipative current sensing
* Programmable speed profiles and position control
* Sensorless stall detection
* Built-in motion engine with acceleration/deceleration control
* Two levels of overtemperature protection
* Overcurrent and undervoltage protection
* SPI interface (5 Mbps max)

## Typical Applications

* Precision motorized stages
* Robotics
* 3D printers
* Industrial automation

## Electrical Specifications

| Parameter                 | Value        |
| ------------------------- | ------------ |
| Supply Voltage (VS)       | 8 V to 45 V  |
| Logic Voltage (VDD)       | 3.3 V or 5 V |
| Max Output Current (RMS)  | 3 A          |
| Max Output Current (Peak) | 7 A          |
| SPI Clock Speed           | up to 5 MHz  |

## Connectors and Interfaces

* **Motor Outputs**: 4 terminals for bipolar stepper motor
* **Power Supply**: VIN and GND (external 8–45 V supply)
* **Logic Interface**: SPI (SDI, SDO, CS, CK), STBY, SW, BUSY/SYNC, FLAG

## Control Interface

The module is controlled via SPI. The L6470 accepts a variety of commands:

* Motion commands: `Run`, `Move`, `GoTo`, etc.
* Positioning: absolute and relative
* Speed and acceleration profile programming

Refer to the [L6470 datasheet](https://www.st.com/resource/en/datasheet/l6470.pdf) for detailed command structure and register settings.

## Protections

* Overcurrent detection with programmable threshold
* Thermal warning and shutdown
* Undervoltage lockout
* Open-drain FLAG pin indicates fault conditions

## PCB Dimensions and Mounting

* Standard MLAB format
* Mounting holes compatible with other MLAB modules

## Resources

* [L6470 Datasheet (ST)](https://www.st.com/resource/en/datasheet/l6470.pdf)
* MLAB Wiki: [HBSTEP01](https://wiki.mlab.cz/doku.php?id=en:hbstep01)


