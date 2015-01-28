# CANtact Firmware

This repository contains sources for CANtact firmware.

## Building

Firmware builds with GCC. Specifically, you will need gcc-arm-none-eabi, which 
is packaged for Windows, OS X, and Linux on 
[Launchpad](https://launchpad.net/gcc-arm-embedded/+download). Download for your 
system and add the `bin` folder to your PATH.

With that done, you should be able to compile using `make`.

## Flashing & Debugging

Debugging and flashing can be done with any STM32 Discovery board as a 
programmer. You can also use other tools that support SWD.

To use an STM32 Discovery, run [OpenOCD](http://openocd.sourceforge.net/) using
the stm32f0x.cfg file: `openocd -f fw/stm32f0x.cfg`.

With OpenOCD running, arm-none-eabi-gdb can be used to load code and debug.

## License

See LICENSE.md