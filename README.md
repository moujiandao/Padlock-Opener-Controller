# Automatic Padlock Opener

Final project for **EME 154: Mechatronics** at UC Davis.

This project controls an electromechanical system that automatically operates a three-number combination padlock. The embedded C++ program coordinates the motor, encoder, user interface, and solenoid used to dial and release the lock.

## Features

- Manual, semi-automatic, and automatic operating modes
- Encoder-based dial positioning
- Clockwise and counterclockwise motor control
- Configurable motor speed and encoder resolution
- Input validation and system diagnostics
- Solenoid actuation to release the lock

## How It Works

In automatic mode, the user enters a three-number combination. The controller calculates the required dial movement, executes the correct clockwise and counterclockwise sequence, and activates the solenoid after reaching the final number.

## Technical Details

- Embedded C++
- 8052-compatible microcontroller
- Motor and encoder feedback
- 40-position combination dial
- UC Davis MORPH mechatronics platform

## Source

The controller implementation is in [`APOC_before_Tues.C`](./APOC_before_Tues.C).

## Authors

Brian Mar and Max Toback
