# STM32-Based Hardware Design in KiCad

## Overview
This project features a **custom hardware design based on the STM32F103C8T6 microcontroller**, developed using **KiCad**.
The design aims to enhance skills in **schematic creation, PCB layout, and embedded systems development** while adhering to best design practices for **power management, clocking, and peripheral integration**.

## Features & Key Components

### **Microcontroller:**

- **STM32F103C8T6** – 32-bit Arm Cortex-M3 running at **72 MHz**, featuring **USB, UART, I2C, SPI, ADC, and GPIOs**.

### **Power Management:**

- **VBAT and VDD** connected to **3.3V**.
  
- **Decoupling Capacitors:** 100nF per VDD and VBAT pin, plus a 10µF bulk capacitor.
  
- **VDDA (Analog Supply):** Additional filtering with a **120Ω Ferrite Bead** for noise reduction.
  
- **Linear Regulator:** Provides a **fixed 3.3V** output with input and output decoupling capacitors.
  
- **Power Indicator LED:** Indicates when the board is powered on.
  

### **Reset & Boot Configuration:**

- **NRST Pin:** Pulled high to ensure program execution; connected to a **100nF decoupling capacitor**.
  
- **BOOT0 Pin:** Used to **enable/disable** the internal bootloader for programming via UART, I2C, SPI, or USB.
  

### **Clock System:**

- **16MHz High-Speed Crystal Oscillator** for the system clock with **10pF load capacitors**.
  

### **USB Connectivity:**

- **Micro-USB Connector (USB_B_Micro)** for power and data communication.
  
- **VBUS Power Input** for external USB-powered applications.
  
- **1.5kΩ Pull-up Resistor** to ensure the device is detected as a USB peripheral.
  

### **Debugging & Programming:**

- **Serial Wire Debug (SWD)** for firmware development and debugging.
  

### **Peripheral Interfaces:**

- **UART Connector** for serial communication.
  
- **I2C Connector** for sensor or peripheral integration.

  ![image.alt](https://github.com/mypin99/STM32_Basic-Embedded-Hardware-Projects/blob/main/STM32-Basics/STM32-Based%20Schematic%20Design.png?raw=true)

  ![image.alt](https://github.com/mypin99/STM32_Basic-Embedded-Hardware-Projects/blob/main/STM32-Basics/STM32-Based%20Hardware%20PCB.png?raw=true)
  

## Possible Applications

Upon assembly, this STM32-based PCB can be used for:


1. **Embedded Systems Development** – A learning platform for STM32 firmware development and debugging.
   
2. **USB-to-Serial Adapter** – Interface between USB and UART-based devices.
   
3. **IoT Sensor Node** – Collect and process sensor data for IoT applications using UART or I2C peripherals.
   
4. **Custom Motor Controller** – Use PWM and GPIOs for motor control applications.
   
5. **USB HID Device** – Can be programmed to act as a USB keyboard, mouse, or joystick.
   
6. **Home Automation Controller** – Control smart home devices via UART or I2C communication.

## Future Enhancements

Potential improvements and additional features for future revisions:

1. **Battery Backup Support** – Adding a Li-Po battery management system for portable applications.
   
2. **Wireless Connectivity** – Integrating Bluetooth or Wi-Fi for remote data transmission.
   
3. **Additional GPIO Expansions** – Extending the number of I/O pins for more external peripherals.
   
4. **Custom Sensor Modules** – Adding built-in temperature, motion, or environmental sensors.
   

## Application Notes & References

- **AN2867** – Oscillator design guide for STM32 MCUs.
  
- **AN4879** – USB Hardware and PCB guidelines for STM32 MCUs.
  
