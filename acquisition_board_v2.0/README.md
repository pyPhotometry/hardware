# Acquisition board v2.0

![photo](photo.png)

An updated version of the acquisition board with the following improvements from version 1.0:

- Increased maximum current of 300mA from the two LED driver outputs.
- 2 additional LED control outputs for triggering external LED drivers that require a voltage control signal (0-3.3V) , allowing the board to be used with optical hardware like the Doric Gen3 minicubes which have integrated LED drivers.  The signals output on the two LED control outputs are the same signals used to control the on-board LED drivers, so it is not possible to independently use the LED control outputs and the LED driver outputs at the same time.
- Reduced artefacts on analog input signals caused by saturation (i.e. voltage exceeding 3.3V) on the other analog input.
- Additional Picoblade connector providing access to 3 pyboard pins including I2C serial communication. 
