# CHIP-8-Emulator
A CHIP-8 emulator in C++

![Space Invaders](screenshots/invaders.png "Space Invaders")
*Space Invaders*

![Pong](screenshots/pong.png "Pong")
*Pong*

CHIP-8 is an interpretted programming language developed by Joseph Weisbecker in the mid 70s and was initally used on the COSMAC VIP and Telmac 1800 8-bit microcomputers to make game programming easier. CHIP-8 programs are run using a CHIP-8 virtual machine.

This is a fairly complete implementation of a CHIP-8 virtual machine however there is currently no sound.

## Compiling and Running

Requires SDL2.dll:

[Official Link](https://github.com/libsdl-org/SDL/releases/tag/release-2.30.6)


To run, use three command-line arguments:

Scale: The CHIP-8 video buffer is only 64x32, so we’ll need an integer scale factor to be able to play on our big modern monitors.

Delay: The CHIP-8 had no specified clock speed, so we’ll use a delay to determine the time in milliseconds between cycles. Different games run best at different speeds, so we can control it here.

ROM: The ROM file to load.

example:
Run:
```
./chip8 10 1 <ROM file>
```