# Smart Home Automation System

## Overview
This project demonstrates a Smart Home Automation System that integrates microcontroller-based components and efficient software design. It uses GPIO and NVIC drivers to manage input/output signals, controls devices, and interacts with sensors. The ADC module processes analog values (e.g., temperature, light), and timers ensure precise operation timing. The system features a display screen for real-time feedback and UART for external communication, enabling intuitive control of home appliances. With a scalable architecture, this system enhances daily life and embraces IoT-driven solutions.

---

## Modules & Usage

- **GPIO**: Used to control all the Input/Output ports.
- **NVIC**: Used to automate real-time operations such as handling button clicks, value changes, and more.
- **ADC**: Used to process analog values, such as from a potentiometer, to handle sensor data.
- **Timer**: Used to count passing time, perform specific operations, and delay others.

---  

### Additional Modules:
- **UART**: Enables interaction with the user through communication with external devices.
- **DHT11**: Used for reading temperature data from a sensor.
- **Nokia5510 Screen**: Displays real-time information to the user.
- **Servo Motor SG90**: Simulates the functionality of an air conditioner.
- **LEDs & Buttons**: Provides visual indicators and user input interfaces.

---

## Applications & Functionalities

- **LEDs**: 
  - Green: Correct password.
  - Red: Wrong password.
  - Yellow: Simulate house lights.

- **Screen (Nokia5510)**: 
  - TV app: Changes channels via ADC-controlled potentiometer.
  - Temperature app: Displays current temperature from DHT11.

- **UART & Buttons**: Handle real-time operations and user interactions.

- **ADC**: Reads potentiometer values to change TV channels.

- **Timer**: Manages operations without delaying others.

- **Channel Changing**: ADC reads analog input to change TV channels.

- **Delays**: Used in operations requiring pauses (e.g., waiting for input).

- **Counters**: 
  - One for ADC value reading every 1 second.
  - One for DHT11 temperature reading every 2 seconds.
  - One for LED flashing.

- **UART**: Simulates password entry for security, unlocking system if correct.

- **DHT11**: Reads temperature for the temperature app.

- **Servo Motor SG90**: Simulates air conditioner with adjustable levels.

---

## Features
- Real-time monitoring of environmental data like temperature.
- Interactive control of home appliances through UART and GPIO.
- Efficient timing and synchronization of operations using timers and NVIC.
- Display of system status and feedback on a Nokia5510 screen.
- Security feature with password verification via UART.

---

## Development Environment

- **IDE**: Keil ARM
- **Microcontroller**: TM4C123GH6PM

---

## Team Members

1. Ahmed Bahy Youssef
2. Ahmed Ragab Mahmoud
3. Abdelrahman Mahmoud Mohammed

---

## Supervisors

- Dr. Lamiaa El Refaie
- Eng. Mahmoud Nawara

---

## Academic Details

- **Program**: Third-year Computer Engineering Mainstream
- **Academic Year**: 2024-2025
- **Course Code**: ELE334-Embedded-Systems

---

## Installation
- Clone this repository:
   ```bash
   git clone git@github.com:ahmedbahy2026/Smart-Home-Project-with-TM4C123GH6PM.git
