# WacomTouchToggle

Easily turn on and off touchpad capabilities for Wacom graphics tablets (such as
the Wacom Bamboo).

## Authors

- Jason C. McDonald (CodeMouse92)
- Inspired by [this answer][1] from Maxweel on AskUbuntu.

## Compatibility

This should work on any Debian-based system, and may also work on other Linux
systems. It is designed to work automatically with any graphics tablet that can
be controlled by `xsetwacom`.

**If you encounter any problems with any Linux system or Wacom tablet, please
report in Issues!**

## History

Wacom graphics tablets are essential parts of any modern graphic designer's
toolkit. Luckily for us Linux users, they work with Ubuntu very well out of the
box! However, some tablets (such as the Wacom Bamboo) have touchpad
capabilities, which can be a massive inconvenience if you tend to rest your hand
on the pad while drawing. Shutting this capability off is less than trivial, so
I wrote this script to automate the process.

I've been using this script for three years - it's the first thing I run when I
plug in my Wacom Bamboo!

## Prerequisites

You must have the package `pcregrep` installed on your system, which should be
available from your system's default package repository. You should also have
`xsetwacom` on your system, which is usually pre-installed on Ubuntu by default.

## Installation

Simply place the `wacomtouch` file in a convenient place for scripts, and be
sure the location is included in your environment path. Mark the script as
executable via `chmod +x wacomtouch`.

Here's an example install, placing the script in your `/usr/local/bin`
directory. Note that we only need the `sudo` because we're working in a system
directory.

```bash
# Move to the location where the script will live.
$ cd /usr/local/bin
# Download the script file from GitHub directly.
$ sudo wget https://github.com/CodeMouse92/WacomTouchToggle/raw/master/wacomtouch
# Make the script executable. (You are encouraged to read the file BEFORE doing this, so you know what it does.
$ sudo chmod +x wacomtouch
# Run the script, turning off your tablet's touch functionality.
$ wacomtouch off
```

## Usage

To turn on and off your tablet's touchpad capability, run `wacomtouch off` or `wacomtouch on`.

If you receive the message...

> No Wacom touch device detected.

...that means the tablet is either not plugged in, or has no touch capability to
toggle.

[1]: https://askubuntu.com/a/118466/23786
