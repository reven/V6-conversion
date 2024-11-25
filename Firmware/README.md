# Keychron Modified

Modified Keychron firmware for ATMega32U4 powered 108 key V6

Hardware:
  * Keychron V6 hardware with a modified PCB with north facing LEDs.
  * An **insane** matrix (that I don't wish for my enemies) to try and squeeze the I/O of the ATMega32.
  
* Keyboard Maintainer: [reven](https://github.com/reven)
* Hardware Supported: ATMega32U4 and custom PCB
* Hardware Availability: Make your own. See [Hardware](https://github.com/reven/V6-conversion/Hardware)

Make example for this keyboard (after setting up your build environment and copying the 'keychron_mod' folder to your qmk 'keyboards' folder):

    make keychron_mod/v6/ansi:default
    make keychron_mod/v6/ansi:reven
    make keychron_mod/v6/ansi:via

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Notes
My first approach was to go through all the code and change references to STM32. But Keychron use a lot of custom functions, like for example the functions that read the matrix. So I just ended up re-writing the firmware from scratch, from one of the many examples. As such, this firmware **is not** a 1:1 equivalence to the stock V6 firmware.