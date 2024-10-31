# Royal Kludge R75 QMK Firmware

This is a port of [iamdanielv's customization](https://github.com/iamdanielv/kb_rk_r65) of [irfanjmdn's QMK R65 firmware](https://github.com/irfanjmdn/r65) to the R75

This also fixes a bug in [sdk66's R75 firmware](https://github.com/hangshengkeji/qmk_firmware/tree/master/keyboards/rk/R75/ansi) where the wiring and RGB matrix were incorrectly configured, causing RGB effects to be offset and several issues in VIAL.

## VIA

To use, follow [this guide from irfanjmdn's repo](https://github.com/irfanjmdn/r65/?tab=readme-ov-file#guide) and replace all occurrences of r65 with r75.

The build and flash commands for VIA can be found [here](https://github.com/mossbed/r75/blob/master/keyboards/r75/via/readme.md).

The VIA JSON can be found in the [extras folder](https://github.com/mossbed/r75/blob/master/extras).

## VIAL

There is a version of this firmware for VIAL in the [vialrgb branch](https://github.com/mossbed/r75/tree/vialrgb), follow the instructions in [irfanjmdn's vialrgb branch](https://github.com/irfanjmdn/r65/tree/vialrgb?tab=readme-ov-file#guide) and replace all occurrences of r65 with r75.

> [!WARNING]  
> Due to VIAL not allowing hard-coded tap dance functions, there is no way to go into the bootloader or to clear EEPROM by pressing key combos, like there is in the VIA version.
>
> To enter the bootloader, unplug your keyboard, hold escape, and then plug it back in again (this will erase your EEPROM as well). You can also enter the bootloader from within VIAL by going to Security > Enter bootloader.
> 
> FN+Shift+Q is already set to TD(0), however, this tap dance key does nothing as stated above. This means that all you need to do to restore the bootloader key is assign the Tap Dance 0 key to Reset from within VIAL. Do note that this will be cleared every time the keyboard is flashed with new firmware.

The build and flash commands for VIAL can be found [here](https://github.com/mossbed/r75/tree/vialrgb/keyboards/rk/r75/readme.md).
