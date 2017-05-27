# WacomTouchToggle

Easily turn on and off touchpad capabilities for Wacom tablets (such as the Wacom Bamboo).

## Authors

- Jason C. McDonald (CodeMouse92)

## History

Wacom tablets are essential parts of any modern graphic designer's toolkit. Luckily for us
Linux users, they work with Ubuntu very well out of the box! However, some tablets
(such as the Wacom Bamboo) have touchpad capabilities, which can be a massive inconvenience
if you tend to rest your hand on the pad while drawing. Shutting this capability off is less than
trivial, so I wrote this script to automate the process.

I've been using this script for three years - it's the first thing I run when I plug in
my Wacom Bamboo!

## Prerequisites

You must have the packages `pcregrep` and `xsetwacom` installed on your system. Both should
be available from your system's default package repository.

## Installation

Simply place the `wacomtouch` file in a convenient place for scripts (such as `/usr/local/bin`), and
be sure to add that directory to your system path. Mark the script as executable via `chmod +x wacomtouch`.

## Usage

To turn on and off your tablet's touchpad capability, run `wacomtouch off` or `wacomtouch on`.
