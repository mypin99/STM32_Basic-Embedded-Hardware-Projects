## STM32 Mixed-Signal Audio Analysis & Generation Board

This project is a USB-powered STM32-based mixed-signal PCB capable of low-frequency signal analysis and arbitrary waveform generation in the audio band (20Hz–20kHz). It integrates both ADC and DAC with optimized analog front-ends, and is tailored for audio, instrumentation, and embedded testing applications.


## Key Features

Single Channel ADC + DAC

High-resolution audio-band signal acquisition and generation

Sampling up to 40kHz (Nyquist limit)


## USB Type-C Powered

<500mA current consumption

USB 2.0 Full-Speed (12 Mbit/s) data stream


## Microcontroller

STM32 Cortex-M0 (STM32F103CBTx)

External crystal oscillator for USB accuracy

SWD Debug interface (with ESD & reset protection)


## Analog Signal Chain

Anti-aliasing and reconstruction filters (3rd-order Sallen-Key, Butterworth)

ESD, RF filtering, and high input impedance (>1 MΩ)

BNC (replaceable with SMA) for robust analog IO


## Power Architecture

Pi filters and RC filters to isolate USB noise

LDO for analog supply, buck converter for digital

Bias generation for single-supply AC coupling


## Auxiliary Features

RGB status LED with PWM control

Compact PCB form factor with proper ground and power separation

![image.alt](https://github.com/mypin99/STM32_Basic-Embedded-Hardware-Projects/blob/main/Mixed%20Signal%20PCB%20Design/PCB%20.png?raw=true)

![image.alt](https://github.com/mypin99/STM32_Basic-Embedded-Hardware-Projects/blob/main/Mixed%20Signal%20PCB%20Design/PCB%20Layout%201.png?raw=true)

![image.alt](https://github.com/mypin99/STM32_Basic-Embedded-Hardware-Projects/blob/main/Mixed%20Signal%20PCB%20Design/Power%20Supply%20Unit.png?raw=true)

![image.alt](https://github.com/mypin99/STM32_Basic-Embedded-Hardware-Projects/blob/main/Mixed%20Signal%20PCB%20Design/MCU.png?raw=true)

![image.alt](https://github.com/mypin99/STM32_Basic-Embedded-Hardware-Projects/blob/main/Mixed%20Signal%20PCB%20Design/ADC%20&%20Analog%20FrontEnd.png?raw=true)

![image.alt](https://github.com/mypin99/STM32_Basic-Embedded-Hardware-Projects/blob/main/Mixed%20Signal%20PCB%20Design/DAC.png?raw=true)


## Applications

Audio waveform generation and analysis

Mixed-signal embedded development and testing

Educational and academic lab tools

Signal processing algorithm prototyping


## Tools & References
KiCad 9 – Schematic and PCB design

STM32CubeIDE – Firmware pin mapping and setup

AN2867 / AN4879 / TA0357 – ST Application notes

http://sim.okawa-denshi.jp/ – Filter design calculators
