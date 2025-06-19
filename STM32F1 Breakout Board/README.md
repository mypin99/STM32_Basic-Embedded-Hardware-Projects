## STM32F1 Breakout Board

This is a compact and minimalistic STM32F1 breakout board, designed to simplify prototyping and testing of STM32F103-based 
applications. It provides easy access to all essential MCU pins, onboard power filtering, reset circuitry, USB connectivity, 
and debug headers. The board is ideal for embedded system developers, students, and IoT engineers.

## Key Features

## MCU: 
STM32F103 in LQFP-48 package

## USB Interface:
Micro-USB (Würth 629105150521)

## Power Supply:
Onboard decoupling and filtering capacitors
Series inductor and ferrite bead for noise isolation

## Clock:

External 8MHz SMD crystal (5.0×3.2mm)

## Debug & Programming:

Full access to SWD/JTAG signals

Reset line available

## User Components:

2 × Status LEDs (0603)

Solder jumpers for boot mode selection

## Headers:

Dual 1x15 2.54mm pin headers for all GPIOs

## Compact Layout:

Designed using 0603/0402 passive components for high density

## Design Tools
KiCad: Schematic, layout, and 3D rendering

STM32CubeIDE: Firmware and pin mapping

3D Viewer: Integrated into KiCad for enclosure planning

![image.alt](https://github.com/mypin99/STM32_Basic-Embedded-Hardware-Projects/blob/main/STM32F1%20Breakout%20Board/STM32F1%20Breakout%20board%203D%20View.png?raw=true)

## Usage
Flash your STM32 code using ST-Link over SWD

Power via USB or header pins

Toggle boot mode using the solder jumper (e.g., to enter DFU)
