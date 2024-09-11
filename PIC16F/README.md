# Tutorial for PIC16F1783

Refer to Microchip product [datasheet](https://www.microchip.com/en-us/product/pic16f1783) of PIC16F(L)1782/3.<br/>
<br/>

## 1.  Device and Clock Configuration

*  Datasheet page 39-70.
*  Configure register.
    - CONFIG1 - Page 40
    - CONFIG1 - Page 42
    - OSCCON - Page 68

```
// Register CONFIG1
#pragma config FCMEN = OFF        // Fail-safe clock monitor -> disable
#pragma config IESO = OFF         // Internal/External switchover -> disable
#pragma config CLKOUTEN = ON      // CLKOUT, clock out function on pin -> enable
#pragma config BOREN = OFF        // Brown-out reset -> enable
#pragma config CPD = OFF          // Data memory code protection -> disabled
#pragma config CP = OFF           // Flash program memory code protection -> disabled
#pragma config MCLRE = ON         // MCLR, master clear function on pin -> enable
#pragma config PWRTE = OFF        // Power-up timer -> disabled
#pragma config WDTE = OFF         // Watchdog timer -> disabled
#pragma config FOSC = HS          // Oscillator selection -> HS, High-speed crystal/resonator connected between OSC1 and OSC2 pins

// Register CONFIG2

```
<br/>
