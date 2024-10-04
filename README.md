# What is this?
This repo is all about practice for me; first time using Github, as well as daily driving Linux. I decided to go with Fedora (i3 Spin) for the rolling releases. The other option was Arch, but I passed just so I could get a little more comfortable with Linux. Doing this on my secondary laptop (ThinkPad X390), but will probably be my main for the rest of the year at least.

![Screenshot_2024-10-03_22-49-00](https://github.com/user-attachments/assets/f906486a-b2ac-4926-bed0-d7726a25a395)

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
