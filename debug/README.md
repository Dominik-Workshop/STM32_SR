If defined SWV (line 43), 
`#define SWV`,
the nucleo board prints "Hello world!" via SWV:

https://github.com/Dominik-Workshop/STM32_SR/assets/100617381/3ae85d60-bd3a-48a2-ae98-0b43b0738f1d


Else, 
`//#define SWV`,
the message is printed via UART, and it can be observed with a Serial Port monitor.

### Helpful notes
If you don't see the `SWV ITM Data Donsole`, you can enable it here: 
![stm_SWV](https://github.com/Dominik-Workshop/STM32_SR/assets/100617381/c263a479-5910-48e8-bbb2-8b4086e3e014)
