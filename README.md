## Endeavouros grub theme

![][1]

![][2]

### Icons is snatched from

* https://www.gnome-look.org/p/1000140/

### background is courtesy of @northernlass

* https://forum.endeavouros.com/t/endeavour-galleon-wallpaper/2332/8

## Installation

Clone the repo

```bash
$ git clone https://github.com/fhdk/endeavouros-grub-theme
```

Change into the folder

```bash
$ cd endeavouros-grub-theme
```

Use `makepkg` to build and install

```bash
$ makepkg -i
```

### If you prefer the manual method

Copy the theme to the grub themes folder

```bash
sudo cp -R endeavorous-nix /boot/grub/themes
```

Then - as root - edit your grub default **/etc/default/grub** to look like this

```txt
GRUB_THEME="/boot/grub/themes/endeavouros-nix/theme.txt"
```

Finally rebuild grub

```bash
$ sudo grub-mkconfig -o /boot/grub/grub.cfg
```

Reboot

## Change format

The theme uses 16:9 format. If you prefer 4:3 modify the **theme.txt** file in the theme folder to use either 4:3 format

```
# 16:9 splash
desktop-image: "splash_169.png"
# 4:3 splash
#desktop-image: "splash_43.png"
```

[1]: endeavouros-nix-grub.png
[2]: endeavouros-nix-boot.png