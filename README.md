## Endeavouros grub theme

### Icons is snatched from

* https://www.gnome-look.org/p/1000140/

### background is courtesy of @northernlass

* https://forum.endeavouros.com/t/endeavour-galleon-wallpaper/2332/8

## Installation

Clone the repo and - as root - copy the files to e.g.

    /boot/grub/themes/endeavouros-nix

Then - as root - edit your grub default **/etc/default/grub** to look like this


    GRUB_THEME="/boot/grub/themes/endeavouros-nix/theme.txt"

Finally rebuild grub

    grub-mkconfig -o /boot/grub/grub.cfg

Reboot


