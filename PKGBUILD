# Maintainer: root.nix.dk

pkgname='endeavouros-galleon'
pgkdesc='EndeavourOS Galleon GRUB Theme'
pkgver=0.2
pkgrel=1
arch=('any')
license=('MIT')
install=theme.install
provides=('galleon-grub-theme')
replaces=('endeavouros-nix')


package() {
    install -d -m755 $pkgdir/boot/grub/themes/$pkgname
    cp -R $startdir/$pkgname $pkgdir/boot/grub/themes/
}

