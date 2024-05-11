# STM32 basic projects

These projects are designed for the Robot Controllers lab, implemented during the 6th semester.

![Microcontroller](https://img.shields.io/badge/Board-NUCLEO_L476RG-white) 
![Platform](https://img.shields.io/badge/Platform-STM32cubeIDE_1.4.0-darkcyan)

## Project structure
Each lab project has a corresponding folder. In it, alongside the project files,
there is a README providing more details.

### Projects list and description:
1. **Blink** - `sr_lab01`:
    - Digital IO, external interrupts
    - If defined BLINK, LD2 is blinking, else it is toggled
      by pressing B1 or pulling D2 pin (PA10) to ground.
		  There is software debouncing on pin D2, and for B1, though
		  the onboard button has hardware debouncing (RC circuit)
		  on the NUCLEO board, so sofware debouncing may be redundant there.

2. **Debug** - `sr_lab02`:
    - Debugger, printf() using UART and SWV
    - This program gives opportunity to play around with the debugger.
		  There are two global variables: msb and lsb.
		  Function foo() is called every second, and it each time it
		  increments the lsb, and every 5 times it increments the msb.
		  Additionally each second the LD2 (onboard LED) is toggled
		  on/off, and a depending if SWV is defined (line 43), it prints
		  a message on serial port, or using SWV (Serial Wire Viewer).
3. **Timers** - `sr_lab03`:
    - Time base generator:
      - Blinks the LD2 LED using timer interrupts, avoiding blocking delays 
        and allowing other operations in the meantime.
    - Input capture:
      - Measures the time between button presses and prints that measurement with UART.
    - PWM:
      - Generates a PWM signal with a specified frequency on the pin with LD2 LED. 
        The duty cycle is cycled through different values by pressing the B1 button.

4. **ADC, DAC, DMA** - `sr_lab4`:
    - To be continued...

5. **PID** - `sr_lab4b`:
    - To be continued...
