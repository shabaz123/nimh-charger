# NiMH Charger

This respository contains a design for a 9V PP3 charger for Nickel Metal Hydride (Ni-MH or NiMH) batteries.

This is unsuitable for any other type of battery. Ony Nickel Metal-Hydride is supported.

The Gerber files zip folder can be uploaded to any PCB manufacturer website to have a printed circuit board (PCB) manufacturered.

## Operation
This charger uses a low current (0.1 C) charge rate. Insert a PP3 NiMH battery, and the charging light should turn on. Rotate the control knob to select the desired charge current to suit batteries labeled 200 mAH to 300 mAH. After nineteen (19) hours, the 'charge complete' LED should switch on, and the charger will stop charging automatically.
If the battery temperature rises, the charging will pause, and the LED labeled HOT will light up. This light should never light up under normal use, because the charge current is so low.

After the charge time is complete (19 hours), if you wish to charge another battery, insert it, and then power-cycle the charger for the charging to begin again, for another 19 hours.



