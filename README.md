## Endeavouros grub theme

![][1]

![][2]

### Icons is snatched from

* https://www.gnome-look.org/p/1000140/

### background is courtesy of @northernlass

* https://forum.endeavouros.com/t/endeavour-galleon-wallpaper/2332/8

## Installation

### Using `yay`

```bash
$ yay -S endeavouros-galleon-grub
```

### Using `git` and  `makepkg`

```bash
$ git clone https://github.com/fhdk/endeavouros-galleon
```

Change into the folder

```bash
$ cd endeavouros-galleon
```

Use `makepkg` to build and install

```bash
$ makepkg -i
```

### Manual

Copy the theme to the grub themes folder

```bash
sudo cp -R endeavorous-galleon /usr/share/grub/themes
```

Then - as root - edit your grub default **/etc/default/grub** to look like this

```txt
GRUB_THEME="/usr/share/grub/themes/endeavouros-galleon/theme.txt"
```

Finally rebuild grub

```bash
$ sudo grub-mkconfig -o /boot/grub/grub.cfg
```

Reboot

## Change format

The theme uses 16:9 format. If you prefer 4:3 modify the **theme.txt** file in the theme folder to use either format

```txt
# 16:9 splash
desktop-image: "splash_169.png"
# 4:3 splash
#desktop-image: "splash_43.png"
```

To play with EndeavourOS logo colors - comment/uncomment the relevant lines in the theme

```txt
#title-color: "#FF7F7F"       # background sail: #FF7F7F
#title-color: "#7F7FFF"       # foreground sail: #7F7FFF
#title-color: "#7F3FBF"       # sail overlap:    #7F3FBF
```

```txt
#item_color = "#FF7F7F"       # background sail: #FF7F7F
#item_color = "#7F7FFF"       # foreground sail: #7F7FFF
#item_color = "#7F3FBF"       # sail overlap:    #7F3FBF
```

```txt
#selected_item_color = "#FF7F7F"       # background sail: #FF7F7F
#selected_item_color = "#7F7FFF"       # foreground sail: #7F7FFF
#selected_item_color = "#7F3FBF"       # sail overlap:    #7F3FBF
```





[1]: endeavouros-galleon-grub.png	"EndeavourOS Galleon Grub"
[2]: endeavouros-galleon-boot.png	"EndeavourOS Galleon Boot"
