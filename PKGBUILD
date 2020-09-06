# Maintainer: root.nix.dk

pkgname=endeavouros-nix
pkgver=0.1
pkgrel=1
arch=('any')
license=('MIT')
install=theme.install


package() {
    install -d -m755 $pkgdir/boot/grub/themes/$pkgname
    cp -R $startdir/$pkgname $pkgdir/boot/grub/themes/
}

