# Smart Home Automation System

## Overview
In today's rapidly advancing technological landscape, smart home automation has become a vital component of modern living, offering convenience, efficiency, and improved quality of life. This project demonstrates the design and implementation of a Smart Home Automation System utilizing microcontroller-based components and efficient software design principles.

Our system integrates various hardware and software modules to handle essential tasks seamlessly. GPIO and NVIC drivers are used to manage input and output signals, enabling the control of devices and interaction with sensors. The ADC module processes analog values, allowing the system to interpret data from environmental sensors such as temperature or light. Timers are utilized to manage delays and counters, ensuring precise timing and synchronization across all operations.

To enhance user interaction, the system includes a display screen for real-time feedback and a UART interface for communication with external devices. This combination of technologies enables effective monitoring and control of home appliances, making the system both intuitive and practical. 

With its robust and scalable architecture, this smart home automation system is a step towards simplifying daily life while embracing the future of IoT-driven solutions.

## Modules & Usage

- **GPIO**: Used to control all the Input/Output ports.
- **NVIC**: Used to automate real-time operations such as handling button clicks, value changes, and more.
- **ADC**: Used to process analog values, such as from a potentiometer, to handle sensor data.
- **Timer**: Used to count passing time, perform specific operations, and delay others.
  
### Additional Modules:
- **UART**: Enables interaction with the user through communication with external devices.
- **DHT11**: Used for reading temperature data from a sensor.
- **Nokia5510 Screen**: Displays real-time information to the user.
- **Servo Motor SG90**: Simulates the functionality of an air conditioner.
- **LEDs & Buttons**: Provides visual indicators and user input interfaces.

## Applications & Functionalities

### LEDs
- **Flashing Green LEDs**: Indicate a correct password when the user enters their home.
- **Flashing Red LEDs**: Indicate a wrong password when the user enters their home.
- **Yellow LEDs**: Simulate house lights.

### Screen (Nokia5510)
- **TV App**: Controlled by the potentiometer value read by the ADC module to change TV channels.
- **Temperature App**: Displays the current temperature value read by the DHT11 sensor.

### UART and Buttons
- Handle real-time operations and interact with user actions.

### Buttons and Screen
- Used to handle real-time operations and interact immediately with user actions.

### ADC
- Reads analog values from the potentiometer to change the TV channel.

### Timer
- Manages counting and timing operations without stopping or delaying other processes.

### Channel Changing
- The ADC module reads analog inputs (such as the potentiometer) and converts them to digital values, which are then used to change the TV channel displayed on the screen.

### Delays
- Delays are used in operations that require stopping processor actions, such as waiting for user inputs or sensor readings.

### Counters
- Multiple counters are employed to manage different time periods and execute various operations:
  - One counter reads values from the ADC every 1 second.
  - Another counter reads temperature data from the DHT11 sensor every 2 seconds.
  - A separate counter controls the flashing of the Red and Green LEDs.

### UART
- Simulates a scenario where the homeowner enters a password via UART. If the password is correct, the system unlocks and activates various applications; otherwise, the process is terminated, ensuring security.

### DHT11
- The DHT11 module reads temperature values and is used in the temperature app to provide real-time environmental data.

### Servo Motor SG90
- Simulates an air conditioner with multiple adjustable levels, controlled by the user via the system.

## Features
- Real-time monitoring of environmental data like temperature.
- Interactive control of home appliances through UART and GPIO.
- Efficient timing and synchronization of operations using timers and NVIC.
- Display of system status and feedback on a Nokia5510 screen.
- Security feature with password verification via UART.

## Installation
- Clone this repository:
   ```bash
   git clone git@github.com:ahmedbahy2026/Smart-Home-Project-with-TM4C123GH6PM.git
