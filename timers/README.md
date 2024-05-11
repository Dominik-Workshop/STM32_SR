# PWM
Generates a 6kHz PWM signal on pin with LD2 LED, with duty cycles cycled with B2 button presses (0%, 12.5%, 66%, 100%)

### Calculations:
**PWM_FREQUENCY = TIM_CLK/((PSC+1) [Hz]**\
`PWM_FREQUENCY = 80 000 000 / (19 + 1) = 6000 Hz`

**PWM_DUTY_CYCLE = CCR/(ARR) * 100%**\
*CCR - Capture Compare Register\
`PWM_DUTY_12_5 = 417 / 3332 * 100% = 12,51%`\
`PWM_DUTY_66 = 2199 / 3332 * 100% = 65.98%`

https://github.com/Dominik-Workshop/STM32_SR/assets/100617381/1d289b59-7bd5-45ad-adb8-4ae4fa509a84

# Input capture
### **!!!!!!! Connect pins PC13 and PA0 !!!!!!**
Prints on serial port time between B2 button presses.\
It uses timer 5 which is being incremented every 250ns\
**(TIM_CLK/((PSC+1) [s] = 80MHz/(19+1)).**

https://github.com/Dominik-Workshop/STM32_SR/assets/100617381/7675cf0d-78af-4fd9-b636-df638808eafa

