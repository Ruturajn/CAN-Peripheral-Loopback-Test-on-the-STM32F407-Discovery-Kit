# CAN-Peripheral-Loopback-Test-on-the-STM32F407-Discovery-Kit

![IMG_20211018_170210](https://user-images.githubusercontent.com/56625259/137723157-541065ff-e9ea-45bc-a20e-90724e46de18.jpg)

This project is aimed to run a Loop back test on the CAN Peripheral available on the STM32F407 Discovery Kit using Bare-Metal Programming. The MCU has a in-built CAN controller,
but a CAN transceiver needs to be connected externally. The CAN transciever used here is SN65HVD230 module. A 120-ohm termination needs to be applied between CAN_H and CAN_L. This
also needs to be connected externally. The connections between the STM32F407 and the transceiver are as follows:

| STM32F407 | SN65HVD230 |
| ---- | ---- |
| 3V | VCC |
| GND | GND |
| PB8 | RX |
| PB9 | TX |

For the 120-ohm termination, connect the CAN_H from the SN65HVD230 module to a point on the breadboard. Then take a resistor or a combination of resistors that make up 120-ohms 
and connect the other end to CAN_L, whih is brought onto the breadboard from the SN65HVD230 module.

