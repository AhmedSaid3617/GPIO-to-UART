# ASCII Character Transmitter

This project involves inputting the ASCII code of a character at GPIO PC15, which is then automatically transmitted via UART every 8 blinks of the LED. It's implemented on STM32F103C6 microcontroller.

## Overview

The purpose of this project is to input ASCII characters to GPIO using a push button and transmit the result via UART. This is an application of two essential peripherals in embedded systems.
## Features

- Use push button to input value to GPIO pin PC15.
- Each time the built in LED at PC13 blink, the input at PC15 is read and stored in a variable, like the falling edge of clock cycle.
- Each 8 blinks of the LED, the value at the variable is transmitted via UART.

## Proteus Simulation

The Proteus simulation file is provided in the repository. You can use it to simulate the behavior of the system without needing physical hardware. 

![image](https://github.com/AhmedSaid3617/GPIO-to-UART/assets/73287639/7b986617-821b-4ffc-b20f-2000207ed9ee)


## Setup

### Hardware Requirements
- STM32F1xx microcontroller
- Push button for input
- Connecting wires
- 3V Power source

### Software Requirements
- Development environment for programming the microcontroller (e.g., Keil, STM32CubeIDE)
- Proteus Design Suite (for simulation)

## Usage

1. Connect the necessary hardware components according to the circuit diagram.
2. Compile and flash the microcontroller with the provided code.
3. Power on the system.
4. Input the ASCII code of the character using the push button connected to GPIO PC15.
5. The ASCII character will be transmitted via UART every 8 blinks of the LED.

## License

This project is licensed under the [MIT License](LICENSE).
