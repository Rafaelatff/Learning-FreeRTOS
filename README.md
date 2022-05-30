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

## How to start

**1 - Download the FreeRTOS**

I downloaded the version [FreeRTOS 202112.00](https://www.freertos.org/a00104.html).

**2 - Download CCS, TivaWare and ARM GCC compiler**

2-a - Install [CCS](https://software-dl.ti.com/ccs/esd/documents/ccs_downloads.html). 

Code Composer Studio was already installed (Version: 10.2.0.00009).

2-b - Using the CCS App Center inside Code Composer Studio, install the TivaWare Software (version 2.2.0.295). 

2-c - Using the CCS App Center inside Code Composer Studio, install the ARM GCC compiler (GNU compiler for ARM devices). 

**3 - Create new project in CCS**

3-a - Create a new project in CCS according to:
![image](https://user-images.githubusercontent.com/58916022/171048207-cfba4623-8411-44e2-b085-c413b1e23eaa.png)

3-b - Right click on the project at Project Explorer tree, then go to 'Properties' -> 'Resource' -> 'Linked Resource' and add the TivaWare path to the project. Do not forget to click in 'Apply and Close' button.

![image](https://user-images.githubusercontent.com/58916022/171048630-b23e09e2-20d1-4b28-ba45-daba2e06680f.png)

3-c - Right click on the project at Project Explorer tree (again), then go to 'Properties' -> 'Built' -> 'Variables' then 'Add...' button. Configure as the following configuration, the 'OK' button, tick the box for 'Show system variables' and again press the 'Apply and Close' button.

![image](https://user-images.githubusercontent.com/58916022/171048759-6f903822-0d2b-4165-a1ed-a67f793eb5be.png)

**4 - Adding the FreeRTOS source code to the project**

Right click on the project at Project Explorer tree, then go to 'Import' -> 'Import...'. Select 'File System' inside the 'General' option, and add the following directory: ti\TivaWare_C_Series-2.2.0.295\third_party\FreeRTOS\Source

Config as followed: 

![image](https://user-images.githubusercontent.com/58916022/171045554-caad031b-d869-42cb-b4fe-adc91e89d1e2.png)

**5 - Configuring diretories of GNU compiler**

5-a - Right click on the project at Project Explorer tree, then go to 'Properties' -> 'Build' -> 'GNU Compiler' -> 'Directories'. Then click in the 'Add...' button, then in the 'Workspace...' button, add the current project, then 'OK' and 'OK' again.

![image](https://user-images.githubusercontent.com/58916022/171049456-7869ed9b-678c-4a20-8275-c414ebc8739b.png)

5-b - Click again in the 'Add...' button and this time add the include path, as following:

![image](https://user-images.githubusercontent.com/58916022/171049568-5637d4c0-5bc2-42ac-b471-c3fac83652e8.png)

5-c - Do the same, this time for the path -> 'portable' -> 'GCC' -> 'ARM_CM4F'.

5-d - Now click in the 'Add...' button, this time click in 'Variables' and add the TivaWare variable, then click 'OK' and 'OK' again.

![image](https://user-images.githubusercontent.com/58916022/171050004-d1e35159-0fa5-4838-a9d3-7e535988dcff.png)

5-e - Inside 'Build' -> 'GNU Compiler' go to 'Symbols' then click in the 'Add...' button and generate a symbol with the name 'gcc'.

![image](https://user-images.githubusercontent.com/58916022/171050253-3437d422-17aa-481a-a612-2d9efd1dbc62.png)
