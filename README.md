# Natural Scrolling
/usr/share/X11/xorg.conf.d/40-libinput.conf
```
Section "InputClass"
        Identifier "libinput touchpad catchall"
        MatchIsTouchpad "on"
        MatchDevicePath "/dev/input/event*"
        Driver "libinput"
        Option "NaturalScrolling" "true"
EndSection
```
# Tap To Click
/usr/share/X11/xorg.conf.d/40-libinput.conf
```
Section "InputClass"
        Identifier "libinput touchpad catchall"
        MatchIsTouchpad "on"
        MatchDevicePath "/dev/input/event*"
        Driver "libinput"
        Option "Tapping" "on"
        Option "TappingButtonMap" "lrm"
EndSection
```
# Feh Wallpaer
feh --bg-scale /path/to/image.file
