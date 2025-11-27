# 8051 Microcontroller Project: Monitoring Analog Signals
## Project Overview
This project demonstrates interfacing an 8051 microcontroller with ADC0809, three analog sensors, and a 16×2 alphanumeric LCD. The system reads and displays the following parameters:

- Resistance (via a potentiometer)
- Temperature (using a temperature sensor)
- Light Intensity (using an LDR)

The ADC0809 converts the analog signals from the sensors into digital values, which are processed by the 8051 microcontroller. These values are displayed in real-time on the LCD.
## Features
- Real-time monitoring and display of three analog signals.
- User-friendly interface using a 16×2 LCD.
- Efficient analog-to-digital conversion using ADC0809.
- Modular code structure for easy updates and enhancements.
## Hardware Components
- Microcontroller: AT89S52 (8051 family)
- Analog-to-Digital Converter (ADC): ADC0809
- LCD Display: LM016L (16×2 alphanumeric display)
- Sensors:
  - Potentiometer for resistance
  - Temperature sensor (e.g., LM35)
  - LDR for light intensity
  - Power Supply: 5V DC
## Pin Connections

| Component            | 8051 Pins   | Additional Info               |
|-----------------------|-------------|--------------------------------|
| ADC0809              | P2.0–P2.7   | Data out pins of ADC        |
|                      | P3.7,3.6,3.2| ALE, SOC and EOC         |
| LCD (16×2)           | P1.0–P1.7   | Data pins                     |
|                      | P3.3–P3.5   | E, RS, RW                     |
| Potentiometer (IN0)  | ADC0808 IN0 | Analog input channel 0        |
| Temperature sensor   | ADC0808 IN1 | Analog input channel 1        |
| LDR                  | ADC0808 IN2 | Analog input channel 2        |

## Software Requirements
- Assembler: ASEM-51 (for assembly code)
- Simulator: Proteus 8.17 (for hardware simulation)
- Programming Language: Assembly

## Circuit Diagram
![Circuit Diagram](https://github.com/Keshab-Github/Embedded-Systems-project/blob/main/Circuit_Diagram.png?raw=true)
