# my_i3wm
my_i3wm configuration


refer to:
https://kifarunix.com/install-and-setup-i3-windows-manager-on-ubuntu-20-04/


* extra setting for touchpad in i3wm
https://cravencode.com/post/essentials/enable-tap-to-click-in-i3wm/
/etc/X11/xorg.conf.d/90-touchpad.conf


Section "InputClass"
        Identifier "touchpad"
        MatchIsTouchpad "on"
        Driver "libinput"
        Option "Tapping" "on"
        Option "TappingButtonMap" "lrm"
        Option "TappingButtonMap" "lmr"
        Option "NaturalScrolling" "on"
        Option "ScrollMethod" "twofinger"
        Option "AccelSpeed" "0.1"
EndSection
testing the set parameter by refer to https://askubuntu.com/questions/948373/change-cursor-speed-in-libinput


* touch screen auto rotation
  refer to this repos: https://gist.github.com/mortie/e725d37a71779b18e8eaaf4f8a02bf5b#file-auto-screen-rotate-sh
