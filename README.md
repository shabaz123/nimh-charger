# NiMH Charger

This respository contains a design for a 9V PP3 charger for Nickel Metal Hydride (Ni-MH or NiMH) batteries.

This is unsuitable for any other type of battery. Ony Nickel Metal-Hydride is supported.

The Gerber files zip folder can be uploaded to any PCB manufacturer website to have a printed circuit board (PCB) manufactured.

## Features
* Simple to build, only 'jellybean' components are used
* Uses a 0.1C charging rate
* Rotary control to select the charging current to match the battery capacity (20-30 mA, corresponding to 200 mAH to 300 mAH)
* Built-in over-temperature cut-out
* Automatically stops charging after 19 hours
* Optional microcontroller interface (a microcontroller is not required)

## Operation
This charger uses a low current (0.1 C) charge rate. Insert a PP3 NiMH battery, and the charging light should turn on. Rotate the control knob to select the desired charge current to suit batteries labeled 200 mAH to 300 mAH. After nineteen (19) hours, the 'charge complete' LED should switch on, and the charger will stop charging automatically.
If the battery temperature rises, the charging will pause, and the LED labeled HOT will light up. This light should never light up under normal use, because the charge current is so low.

After the charge time is complete (19 hours), if you wish to charge another battery, insert it, and then power-cycle the charger for the charging to begin again, for another 19 hours.



