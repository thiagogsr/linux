# Linux

## Requirements

```
sudo apt install playerctl xclip maim
```

## Input

### Mouse and Touchpad

1. Edit the file

```
sudo vim /usr/share/X11/xorg.conf.d/40-libinput.conf
```

2. Add `Option "NaturalScrolling" "True"` to pointer and touchpad identifiers
3. Add `Option "Tapping" "on"` to touchpad identifier

### Keyboard

1. Download i3-keyboard-layout

```
wget https://raw.githubusercontent.com/porras/i3-keyboard-layout/master/i3-keyboard-layout ~/.config/i3
```

2. Then

```
chmod +x ~/.config/i3/i3-keyboard-layout
```

## i3

1. Create symbolic links for config files

1.1 i3

```
ln -s /home/thiago/projects/linux/i3/config /home/thiago/.config/i3/config
```

1.2 i3status

```
ln -s /home/thiago/projects/linux/i3status/config /home/thiago/.config/i3status/config
```

## Dracula

### Ulauncher

```
git clone https://github.com/dracula/ulauncher.git ~/.config/ulauncher/user-themes/dracula-ulauncher
```
