# Fedora I3 Spin | Thinkpad X390
This repo is all about practice for me. First time using Github, as well as daily driving Linux. I decided to go with Fedora for it's rolling releases. My other option was Arch, but decided not to just so I could get comfortable with Linux. I am running this all on a Thinkpad X390.

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
