# My Keyboard Setup 

# Hardware

Massdrop fullhand Ergodox 
Cherry MX Clear switches
Blank keycaps

# Firmware

https://github.com/benblazak/ergodox-firmware downloaded via Massdrop ergodox configurator.
Small patch applied to get function keys F13-F24 working.
https://github.com/benblazak/ergodox-firmware/pull/74/files

# Keyboard Layout

http://workmanlayout.org adapted for ergodox.
Defined in: ./keyboard/ergodox/layout/default--layout.h

# Keybindings

Using xbindkeys for Xubuntu OS.
Defined in: xbindkeysrc
Keybindings for volume control and Spotify Previous/Next/PlayPause
Function keys + keybindings used in place of media keys due to spotty support for media keys

# build

## udev rules
sudo cp 49-teensy.rules /etc/udev/rules.d/

## dependencies
sudo apt-get install gcc-avr avr-libc

## build firmware.hex
make

## flash
./teensy &


