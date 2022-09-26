# One 3 Mini (DKON2161ST)

![one3mini](https://www.duckychannel.com.tw/upload/2022_04_272/202204271632021pemzkLez2.png)

A 60% keyboard by Ducky.

This firmware was tested on the Ducky One 3 Mini 2161ST version.


* Keyboard Maintainer: [FlamingCupcake](https://github.com/FlamingCupcake)
* Hardware Supported: Ducky One 3 Mini (DKON2161ST), NUC126SG4AE + MBI5042GP
* Hardware Availability: [Ducky Channel](https://www.duckychannel.com.tw/en/One3-Mini)

## Compiling the Firmware:

Make example for this keyboard (after setting up your build environment):

    make ducky/one3mini/2161st:default

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Accessing Bootloader Mode

To enter the 2161ST bootloader to flash, boot the keyboard while holding D+L.

## Flashing the Firmware:

There are then two ways to flash the keyboard:

    pip install --user nuvoton-isp
    nuvoisp -f ducky_one3mini_ansi.bin

Alternatively you can use elfmimi's [nu-isp-cli](https://lib.rs/crates/nu-isp-cli) which is more complete than nuvoisp and allows flashing .hex files as well.

    cargo install nu-isp-cli
    nu-isp-cli flash ducky_one3mini_ansi.bin

