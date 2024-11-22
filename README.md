# NiMH Charger

This respository contains a design for a battery charger for Nickel Metal Hydride (Ni-MH or NiMH) batteries.

This is unsuitable for any other type of battery chemistry. Ony Nickel Metal-Hydride is supported.

I have only tested this with 9V PP3 Ni-MH batteries, but it should work with other Ni-MH batteries too (you may need to change resistor values if you need to charge at a different current; consult your battery datasheet).

The Gerber files zip folder can be uploaded to any PCB manufacturer website to have a printed circuit board (PCB) manufactured.

## Features
* Simple to build, only 'jellybean' components are used
* Uses a 0.1C charging rate
* Rotary control to select the charging current to match the battery capacity (20-30 mA, corresponding to 200 mAH to 300 mAH)
* Built-in over-temperature charge pause, until the temperature decreases again
* Automatically stops charging after 19 hours
* Optional microcontroller interface (a microcontroller is not required)

## Operation
This charger uses a low current (0.1 C) charge rate (see Technical Note below). Insert the NiMH battery, and the charging light should turn on. Rotate the control knob to select the desired charge current to suit batteries labeled 200 mAH to 300 mAH. After nineteen (19) hours, the 'charge complete' LED should switch on, and the charger will stop charging automatically.
If the battery temperature rises, the charging will pause, and the LED labeled HOT will light up. This light should never light up under normal use, because the charge current is so low.

After the charge time is complete (19 hours), if you wish to charge another battery, insert it, and then power-cycle the charger for the charging to begin again, for another 19 hours.

## Technical Note
Consult the battery manufacturer datasheet or white paper to confirm that the charging method is suitable. This project relies on the following note within a GP Technical Paper:

>Apart from fast charging, GP NiMH batteries can also be charged at a lower current rate of 0.1C. As this charging method is less severe, charge termination at 160% nominal capacity input is recommended (to help avoid extended overcharging of the battery). Also, in some applications where overcharging is necessary, GP NiMH batteries can endure 0.1C continuous charging for about one year.

## Files
There are two different PCBs, Type 1 and Type 2.

Type 1 contains a PP3 battery holder. See the file [nimh-charger-gerbers-rev1-1.zip](nimh-charger-gerbers-rev1-1.zip) for the Gerber files for Type 1. The schematic is in [nimh-pp3-charger-schematic-rev1.pdf](nimh-pp3-charger-schematic-rev1.pdf)

Type 2 omits the battery holder, so that a NiMH battery can be attached using a cable with any desired connector. The components are uprated, to support charging for higher capacity batteries compared to PP3. The Gerber files are in [export-nimh-charger-gerbers-rev1-1.zip](export-nimh-charger-gerbers-rev1-1.zip) and the schematic is in [nimh-charger-rev1-1-schematic.pdf](nimh-charger-rev1-1-schematic.pdf)


