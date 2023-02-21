## Adafruit Floppy FeatherWing with 34-Pin IDC Connector PCB

<a href="http://www.adafruit.com/products/5679"><img src="assets/5679-01.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit Floppy FeatherWing with 34-Pin IDC Connector. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/5679

### Description

Relive the days when storage was counted out in kilo-bytes not giga-bytes, using the Adafruit Floppy FeatherWing on a Feather board - perfect for interfacing with 34-Pin IDC Connector floppy drives that were ubiquitous on PC's. This 'Wing has level shifting and a ready-to-plug connector that works with 3.5" or 5.25" floppy disks for reading or writing!

Floppy disks have an interesting data transfer method where raw bit transitions are measured and converted to data. This data streams pretty fast from the disk drive so you'll want to use a fast microcontroller that has large SRAM storage and ideally, a peripheral to DMA the data signal. For that reason we only have this FeatherWing working with the Feather M4 or Feather RP2040. ESP32, ATmega, nRF52, etc have not been ported to our support library!

Floppy disk drives require 5V power and logic. For the logic level shifting, we have a small boost converter on the 'Wing that will give 5V logic levels out the 34-pin connector. It will also shift the incoming signals down to a Feather-safe 3.3V.

For floppy driver powering you will likely need a separate external 5V power supply that can provide 5V at 2 A. You can't power most drives off of USB power, they have big motors that require more current than USB can provide!

We've got code and examples for three use cases:

Reading floppy disks and storing the raw bit patterns and/or converted data format for data archiving. For this use case we recommend using the 'Wing with a Feather programmed to act as a greaseweazle or fluxengine client device. Then run those command line programs on your computer to have the Feather send the raw track data to the computer for analysis, bit-repair and format interpretation. You can also write some formats via those two programs, for use with older computers. We also have a 'Write Disable' switch on board specifically for this use case so that it is not possible for the write-enable pin to accidentally be activated.
Reading/Writing FAT formatted floppy disks from Arduino, CircuitPython or a computer that is connected via USB. Floppy disks can still be used to save, read data from! This is great for retro-themed projects or if you want to write data to floppy disks for them to be used by IBM-PC compatibles or other devices that are expecting FAT-formatted floppy disks
Cool floppy music sequencing!
Each order comes with one FeatherWing with the 2x17 header attached and level shifting circuitry built in. Before it can be used to read/write floppies, you will need to:

Solder pin headers on to attach to a Feather board. 
Attach an M4 or RP2040 Feather as the driver/brains.
Find a 34-pin IDC Floppy Drive that works
Connect a 34-pin DC cable between the 'Wing and the Floppy drive.
Provide 5V power to the floppy drive, as much as 2 Amps. 5.25" disk drives will also need a 12V power supply!
Find some floppy disks to read/write
Many of these items are no longer sold, and will require some sleuthing to locate!

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
