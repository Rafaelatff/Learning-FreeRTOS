# Learning-FreeRTOS
Let's learn FreeRTOS using Tiva C Series TM4C1294

## Checking hardware compatibility

On [FreeRTOS](https://www.freertos.org/RTOS_ports.html) website, there is a list of the official RTOS ports.  These demos can be adapted to any microcontroller within a supported microcontroller family. 

For the Hardware Partner TI (Texas Instruments), the 	Supported Processor Families are: RM48, TMS570, ARM Cortex-M4F MSP432, MSP430, MSP430X, SimpleLink, Stellaris (ARM Cortex-M3, ARM Cortex-M4F). For the same hardware partner, the Supported Tools are: Rowley CrossWorks, IAR, GCC, Code Composer Studio.

The hardware I plan to use (same that I used during college), is: **EK-TM4C1294XL**.

  The TM4C1294 Connected LaunchPad Evaluation Kit is a low-cost development platform for **32-bit ARM® Cortex-M4F-based** microcontrollers. The Connected LaunchPad design     highlights the **TM4C1294NCPDT** MCU with its on-chip 10/100 Ethernet MAC and PHY, USB 2.0, hibernation module, motion control pulse-width modulation and a multitude of simultaneous serial connectivity.

More info can be found at:

https://www.ti.com/tool/EK-TM4C1294XL

https://www.ti.com/lit/ds/symlink/tm4c1294ncpdt.pdf?HQS=dis-mous-null-mousermode-dsf-pf-null-wwe&ts=1653887957312&ref_url=https%253A%252F%252Fwww.mouser.de%252F

It looks like a good start and no need for a new hardware.

## Downloading the FreeRTOS

I downloaded the version [FreeRTOS 202112.00](https://www.freertos.org/a00104.html).
