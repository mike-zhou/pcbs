9200-45-1st-board.zip is the basic of the first PCB board.

9200-53-no-cpld.zip includes many improvments, such as the direction of the serial port,
adjustion of the BMS, connection of the BFOE to the dm9161, removal of the 74lv245 chips,
adjustion of the USB layout, adjustion of the flash, pulling up the data bus, adjustion
 of hole's inner diameter, adjustion of FIQ and IRQ0, addion of the outer power supply of the oscillistor,
adjustion of the fixing hole.

The anchor points are not connected GND directly.

The RS232 in the previous version is wrong, it is updated to male.

A CPLD is added in this version, but it is not routed.

PA5,PA6 should be used to control USBD, other than PA3 and PA4, so as to make SPI available.
Modified.

Remove the audion of USBD.

Changed the resister relevant to the LED.

EPM240 has been added in the board.

Removed the diode connect to the USBD.

2008.1.4
Adjust the distance between two pads of 1206 to 3mm.
Adjust the width of the pads of 2220 to 3mm.
Adjust the pad size of 0603 to 1mm*1mm, the distance between two pad to 1.6mm.

2008.1.5
In the SCH about the ethernet, only the SCH in main.sch is correct. VCCA is connected to L7, L7 is connected to AGND directly in other SCH, this is a serious problem.
Relocate the component about the ethernet. 
BasicComponents.pcb is created.
Adjust the position of the components in BasicComponents.pcb, delete the L that connecting the AGND and GND, delete a power supply of ethernet, then save the result as BasicComponents-1.pcb

2008.1.6
Adjust the serial port connection in PCB4_total.pcb

2008.1.9
Data I/O pins of the flash have been adjusted.

2008.1.10
Change BFOE from PC4 to PA17.
JTAG is adjusted to 20 pins.
The outline of the USB-device is adjusted.
The hole size of USB-device and usb-host is adjusted.

2008.1.12
Adjust the JTAG according to the pinouts in the ARM ICE documents.
Disconnect the PIOB from EPM240.

2008.1.21
Finished the PCB of board.
Connected the EARTH and GND.

2008.1.29
Re-design the GND connected to the eth0, increase the distance between the GND and EARTH.

2008.2.28
Add a resistor which is parelel the LED of DTX.

2008.8.6
Finished the voltage meter.
Adjusted the ECD_920, the hole size for PIO and EMI are expanded, and earth plane near the USB host and device port are adjusted. 
The capactor near the PIO_A are placed to the bottom plane. The width of 1206 are increased.

2008.8.12
Updated the SCH of ECD_920.

2008.8.14
Adjusted the position of text 'pioa', 'piob' and 'pioc'.
Redesigned feed-back and current sample resister in the VS212A.

2008.8.17
Adjusted the pad with of the footprint of transistor.

2008.8.31
Adjusted the diode to protect TIP122 and TIP127, connected one pad of the diode to the emmiter of the TIP122 and TIP127.

2008.9.1
Move the CS of VS212A left.

2008.9.3
Rename VS212A to VP212A.
Adjust the filteres for V+ and V- of VP212A.
Adjust the ground for ADC.

2008.9.10
Add a thermal dispatcher to V14 of VM810A.

2008.9.21
Add thermal dispatcher to TIP122 and TIP 127.

2009.2.8
Add feedback selection Rs to the VS212A.
Voltage reference 2.5V can be configured in three ways. If a LM385 is used, reference +2.5V can be created by connecting R31 with 1K, R30 and R32 with 0; -2.5V can be created by conecting R34 and R35 with 0, R33 with 1K. If ADR421 is used, reference +2.5V can be created at pin 6.

2009.2.21
Add a larger capacity to the VREF of VS212A. Adjust the position of the fixing pads of VM810A to make them same as those in VS212A.

2009.4.29
7c68013 is finished.

2009.5.4
upate the layout of the usb tracks.