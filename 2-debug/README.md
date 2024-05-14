## printf()
If defined SWV (line 43), 
`#define SWV`,
the nucleo board prints "Hello world!" via SWV:

https://github.com/Dominik-Workshop/STM32_SR/assets/100617381/3ae85d60-bd3a-48a2-ae98-0b43b0738f1d


Else, 
`//#define SWV`,
the message is printed via UART, and it can be observed with a Serial Port monitor.

## Debuger
https://github.com/Dominik-Workshop/STM32_SR/assets/100617381/c5550bcd-ac92-4665-a584-f9b0bb222257



## Helpful notes
- If you don't see the `SWV ITM Data Donsole`, you can enable it here: 
![stm_SWV](https://github.com/Dominik-Workshop/STM32_SR/assets/100617381/c263a479-5910-48e8-bbb2-8b4086e3e014)
- To print float values, you have to enable it in project properties\
![printf_float_1](https://github.com/Dominik-Workshop/STM32_SR/assets/100617381/dff63d19-5dd8-4bac-bfb2-302df73c9133)
![printf_float2](https://github.com/Dominik-Workshop/STM32_SR/assets/100617381/4698f419-9d70-41a2-a182-ceae8b81aea2)

