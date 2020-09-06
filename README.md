## Endeavouros grub theme

### Icons is snatched from

* https://www.gnome-look.org/p/1000140/

### background is courtesy of @northernlass

* https://forum.endeavouros.com/t/endeavour-galleon-wallpaper/2332/8

## Installation

Clone the repo

    git clone https://github.com/fhdk/endeavouros-grub-theme

Change into the folder

    cd endeavouros-grub-theme

Use `makepkg` to build and install

    makepkg -i

### If you prefer the manual method

Copy the theme to the grub themes folder

    sudo cp -R endeavorous-nix /boot/grub/themes

Then - as root - edit your grub default **/etc/default/grub** to look like this

    GRUB_THEME="/boot/grub/themes/endeavouros-nix/theme.txt"

Finally rebuild grub

    grub-mkconfig -o /boot/grub/grub.cfg

Reboot
