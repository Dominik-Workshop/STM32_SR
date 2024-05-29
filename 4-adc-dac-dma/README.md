# ADC
  Prints measured voltage on pin PB0 via UART:\
  Measured value: <adc_raw>, <voltage> [V]
  e.g:\
  `Measured value: 4031, 3.25 [V]`\
  `Measured value: 0, 0.00 [V]`

  Uses interrupts to read ADC values.
  
# ADC DAC
### **!!!!!!! Connect pins PA4 and PB0 !!!!!!**
  Using DAC desired voltages are produced on pin PA4,
  and ADC measures these voltage using pin PB0.\
  These values are printed with UART, e.g:\
  `Set value: 0.00`\
  `Measured value: 0.00`\
  `Set value: 0.49`\
  `Measured value: 0.44`\
  `Set value: 1.70`\
  `Measured value: 1.64`\
  `Set value: 2.50`\
  `Measured value: 2.44`\
  `Set value: 3.30`\
  `Measured value: 3.22`

  Uses interrupts to read ADC values.

# DMA
### **!!!!!!! Connect pins PA4 and PB0 !!!!!!**
  Using DAC desired voltages are produced on pin PA4,
  and ADC measures these voltage using pin PB0.\
  DMA is used to set the DAC output.\
  `HAL_ADC_PollForConversion()` is used to get ADC values.