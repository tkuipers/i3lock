## Forked fork

This fork of i3lock is based off of another fork by [Lixxia](https://github.com/Lixxia). This forks adds a
feature that changes the color of the wheel to an inverse of the average color
of the background picture being used. It can only be used if you specify a
background image.

The feature can be used with the --inverse-wheel flag.
  
## Ubuntu Dependencies

Here is a list of the dependencies specifically for Ubuntu (tested on Ubuntu 14.04).
See also: the 'Requirements' list below.

- libxcb-dpms0-dev

- libxcb-xkb-dev

- libev-dev

- libxkbcommon-x11-dev

- libxcb-image0-dev

- libxkbcommon-dev

- libxkbcommon0

### Original fork

This is my own copy of i3lock, consisting of the following tweaks: 
- Changed the display on key-strokes and escape/backspace.
- Added 12-hour clock to the unlock indicator and periodic updater so time stays relevant. 
- Changed border, text, and background colors.
- Changed it so that the unlock indicator will always be displayed, regardless of state. (Originally it was only shown after initial keypress).

## Screenshots
#### Default
![Default state](/screenshots/lockscreen.png?raw=true "")
### Key Press
![On key press](/screenshots/lockscreenkeypress.png?raw=true "")
### Escape/Backspace
![On escape or backspace](/screenshots/lockscreenesc.png?raw=true "")

<p>
---
### Original README

i3lock - improved screen locker
===============================
i3lock is a simple screen locker like slock. After starting it, you will
see a white screen (you can configure the color/an image). You can return
to your screen by entering your password.

Many little improvements have been made to i3lock over time:

- i3lock forks, so you can combine it with an alias to suspend to RAM
  (run "i3lock && echo mem > /sys/power/state" to get a locked screen
   after waking up your computer from suspend to RAM)

- You can specify either a background color or a PNG image which will be
  displayed while your screen is locked.

- You can specify whether i3lock should bell upon a wrong password.

- i3lock uses PAM and therefore is compatible with LDAP etc.

Requirements
------------
- pkg-config
- libxcb
- libxcb-util
- libpam-dev
- libcairo-dev
- libxcb-xinerama
- libev
- libx11-dev
- libx11-xcb-dev
- libxkbfile-dev
- libxkbcommon >= 0.4.0
- libxkbcommon-x11 >= 0.4.0

Running i3lock
-------------
Simply invoke the 'i3lock' command. To get out of it, enter your password and
press enter.

Upstream
--------
Please submit patches to http://cr.i3wm.org/
