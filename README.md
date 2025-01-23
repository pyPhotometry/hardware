# pyPhotometry Hardware

This repository contains design files for pyPhometry hardware.  For more information see: https://pyphotometry.readthedocs.io/en/latest/user-guide/hardware/

The repository contains the following devices:

## Acquisition board v1.0

![board_v1.0](acquisition_board_v1.0/photo.jpg)

The original version of the acquisition board as detailed in the [pyPhotometry manuscript](https://www.nature.com/articles/s41598-019-39724-y), featuring:

-  2 analog inputs (0-3.3V) for photoreceiver signals.
- 2 Digital inputs for registering behavioural events or sync pulses.
- 2 LED driver outputs with 0-100mA adjustable current output.

## Acquisition board v2.0

![board_v2.0](acquisition_board_v2.0/photo.png)

An updated version of the acquisition board with the following improvements from version 1.0:

- Increased maximum current of 300mA from the two LED driver outputs.
- 2 additional LED control outputs for triggering external LED drivers that require a voltage control signal (0-3.3V) , allowing the board to be used with optical hardware like the Doric Gen3 minicubes which have integrated LED drivers.  The signals output on the two LED control outputs are the same signals used to control the on-board LED drivers, so it is not possible to independently use the LED control outputs and the LED driver outputs at the same time.
- Reduced artefacts on analog input signals caused by saturation (i.e. voltage exceeding 3.3V) on the other analog input.
- Additional Picoblade connector providing access to 3 pyboard pins including I2C serial communication.  

## Acquisition board case

![board_v2.0](acquisition_board_case/photo.png)

A plastic case compatible both v1.0 and v2.0 acquisition boards.

