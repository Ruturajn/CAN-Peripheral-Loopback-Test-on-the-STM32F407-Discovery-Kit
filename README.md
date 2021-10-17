# CAN-Peripheral-Loopback-Test-on-the-STM32F407-Discovery-Kit

This project is aimed to run a Loop back test on the CAN Peripheral available on the STM32F407 Discovery Kit using Bare-Metal Programming. The MCU has a in-built CAN controller,
but a CAN tranceiver needs to be connected externally. The CAN tranciever used here is SN65HVD230 module. A 120 ohm termination needs to applied between CAN_H and CAN_L. This also
needs to be connected externally. The connections between the STM32F407 and the tranceiver are as follows:

| STM32F407 | SN65HVD230 |
| ---- | ---- |
| 3V | VCC |
| GND | GND |
| PB8 | RX |
| PB9 | TX |
