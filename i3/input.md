# Input

- Mouse
- Touchpad
- Keyboard

## Changes

### Mouse and Touchpad

1. Edit the file `sudo vim /usr/share/X11/xorg.conf.d/40-libinput.conf`
2. Add `Option "NaturalScrolling" "True"` to pointer and touchpad identifiers
3. Add `Option "Tapping" "on"` to touchpad identifier

### Keyboard

1. Download i3-keyboard-layout `wget https://raw.githubusercontent.com/porras/i3-keyboard-layout/master/i3-keyboard-layout ~/.config/i3`
2. Run `chmod +x ~/.config/i3/i3-keyboard-layout`
