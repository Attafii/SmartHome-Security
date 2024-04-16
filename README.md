# Home Surveillance IoT System

## Description
This project involves developing an Internet of Things (IoT) application using the STM32F407VG microcontroller to remotely monitor your home. The system components include various sensors and actuators.

## Components
- **STM32F407VG Microcontroller**
- **Analog Gas Sensor**
- **Digital Presence Sensor (connected to RA3)**
- **Digital Smoke Sensor (connected to RC2)**
- **Buzzer (connected to PB12)**
- **Two LEDs: Green (RA3) and Red (RD2)**
- **ESP8266 Shield**

## Functionality
1. **Startup**:
   - Upon startup, the green LED is lit, the red LED is off, and the buzzer remains inactive.

2. **Gas Monitoring**:
   - Continuously reads the gas value from the gas sensor.
   - If the gas value is equal to or greater than 20, the buzzer activates, the red LED turns on for 30 minutes, and the system sends the gas value to the central database (Cloud THINGSPEAK).

3. **Presence and Smoke Detection**:
   - Whenever presence or smoke is detected:
     - An alert is sent directly to the central database (Cloud THINGSPEAK).
     - The red LED turns on.
     - The buzzer activates for 5 minutes.

## Tasks
### Session 5:
- Choose pins for connecting inputs and outputs.
- Create a complete circuit diagram using simulation software.
- Design the system flowchart.
- Write C code to simulate startup behavior.

### Session 6:
- Define an Analog-to-Digital Converter (ADC).
- Identify the STM32F407VG pin(s) for ADC.
- Write C code for scenarios related to the gas sensor.

Feel free to customize this README with additional details specific to your project. Good luck! 🚀
