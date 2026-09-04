# Automatic Padlock Opener

This repository preserves the controller program for a 2014 UC Davis EME 154 mechatronics project built by Brian Mar and Max Toback.

The system used a motor, encoder, solenoid, keypad, and the UC Davis MORPH controller platform to operate a three-number combination padlock.

## Controller behavior

The source includes:

- Manual clockwise and counterclockwise movement.
- A semi-automatic operating mode.
- Automatic combination entry and dial sequencing.
- Configurable encoder resolution, motor speed, and dial positions.
- Position feedback through the controller's motion registers.
- Solenoid activation after the final dial movement.
- Console menus, setup state, and basic input checks.

The implementation is in [`APOC_before_Tues.C`](APOC_before_Tues.C).

## Hardware and toolchain

The program targets an 8052-compatible microcontroller and depends on the course-specific `MORPH.h` interface, memory-mapped controller registers, and assembly entry points supplied by the MORPH environment.

It is not a portable desktop C++ application and cannot be built with a standard compiler without the original controller headers and runtime.

## Project status

This is an archived classroom artifact. The source is kept close to its original 2014 state, including work-in-progress comments and hardware-specific assumptions. It has not been verified on a modern MORPH toolchain.
