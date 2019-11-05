# Maintainer: YuutaW <i@yuuta.moe>
# Thanks: https://aur.archlinux.org/cgit/aur.git/tree/PKGBUILD?h=systemd-boot-pacman-hook
pkgname=x-touch-touchpad
pkgver=1
pkgrel=1
pkgdesc="Enable TouchPad touch-as-click for Xorg"
arch=("any")
url="https://github.com/Trumeet/X-Touch-Touchpad"
license=('GPL')
depends=("xorg-server")
source=(20-touchpad.conf)
md5sums=('9044be56ab91ae1c550ba68f12a6a4fe')

package() {
    install -m755 -d "${pkgdir}/etc/X11/xorg.conf.d"
    install -m644 "${srcdir}/20-touchpad.conf" "${pkgdir}/etc/X11/xorg.conf.d/20-touchpad.conf"
}
