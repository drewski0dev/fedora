# What is this?
This is my first time daily driving Linux. This is not necessarily a beginner's guide, but I've compiled some things that I found useful in my experience. You'll find here some basic functionality as well as some of my config files for 'ricing' Linux.\
The device I am using is a ThinkPad X390 running Fedora Linux 40.

![Screenshot_2024-10-07_22-03-33](https://github.com/user-attachments/assets/24adff5e-55b8-4972-bc42-8322743a7021)

# General Functionality
> Some of this may be specific to Fedora's i3 Spin release, and/or X390 components (such as touchpad config files)

## Touchpad Features
Two touchpad features I like to have in my environment are **Natural Scrolling** and **Tap to Click**. These are not enabled by default.\
*To enable these features, adds these lines to your config in `/usr/share/X11/xorg.conf.d/40-libinput.conf` under the InputClass identifer "libinput touchpad catachall"*
```
        Option "NaturalScrolling" "true"
        Option "Tapping" "on"
        Option "TappingButtonMap" "lrm"
```

## Connecting to Wi-Fi in Command Line
Using `nmcli` you can connect to Wi-Fi from the command line\
*First, to list possible connections use `nmcli device wifi'*
> nmcli will put you in Less command mode to navigate this list. If you are unfamiliar with this mode, hit 'q' to exit back to the command line.

*Once you've found the Wi-Fi you would like to connect to, use `nmcli device wifi connect "SSID" password "password"`*

I was running into issues connecting to my school's Wi-Fi. The easy solution I found was using `nm-connection-editor` Create a new connection using the SSID of the school Wi-Fi, and edit the Wi-Fi security settings.
