# Linux

## Requirements

```
sudo apt install playerctl xclip maim lxappearance
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

i3

```
ln -s /home/thiago/projects/linux/i3/config /home/thiago/.config/i3/config
ln -s /home/thiago/projects/linux/i3/workspace-1.json /home/thiago/.config/i3/workspace-1.json
ln -s /home/thiago/projects/linux/i3/workspace-2.json /home/thiago/.config/i3/workspace-2.json
ln -s /home/thiago/projects/linux/i3/workspace-3.json /home/thiago/.config/i3/workspace-3.json
ln -s /home/thiago/projects/linux/i3/workspace-4.json /home/thiago/.config/i3/workspace-4.json
```

i3status

```
ln -s /home/thiago/projects/linux/i3status/config /home/thiago/.config/i3status/config
```

## Terminator

1. Create symbolic link for config file

```
ln -s /home/thiago/projects/linux/terminator/config /home/thiago/.config/terminator/config
```

## Dracula

### Ulauncher

```
git clone https://github.com/dracula/ulauncher.git ~/.config/ulauncher/user-themes/dracula-ulauncher
```

### GTK

1. Download and unzip the theme

```
mkdir ~/.themes
wget https://github.com/dracula/gtk/archive/master.zip -O ~/.themes/dracula-gtk.zip
unzip ~/.themes/dracula-gtk.zip -d ~/.themes && mv ~/.themes/gtk-master ~/.themes/dracula
rm ~/.themes/dracula-gtk.zip
```

2. Run `lxappearance` and change theme to `dracula`
