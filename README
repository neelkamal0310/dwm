# dwm - dynamic window manager
dwm is an extremely fast, small, and dynamic window manager for X.


### Requirements
In order to build dwm you need the Xlib header files.


### Installation
Edit config.mk to match your local setup (dwm is installed into
the `/usr/local` namespace by default).

Afterwards enter the following command to build and install dwm (if
necessary as root):
```
make clean install
```

### Running dwm
Add the following line to your .xinitrc to start dwm using startx:
```
exec dwm
```

Or to restart dwm without killing X (Mod+Shift+r in this build), put the following snippet
in `~/bin/startdwm` and start `startdwm` using startx:
```
while true; do
    # Log stderror to a file
    dwm 2> /tmp/.dwm.log
    # No eror logging
    #dwm > /dev/null 2>&1
done
```

### Configuration
The configuration of dwm is done by creating a custom `config.h`
and (re)compiling the source code.

### Applied Patches

* [fullgaps](https://dwm.suckless.org/patches/fullgaps/) - gaps between windows
* [systray](https://dwm.suckless.org/patches/systray/) - system tray support
* [alpha](https://dwm.suckless.org/patches/alpha/) - transparency support in status bar (not system tray) and opaque borders
* [pertag](https://dwm.suckless.org/patches/pertag/) - preserve layout across tags

### Notes
* `dmenu` called by this build requires patches border, center and grid. Change it in `config.h`
