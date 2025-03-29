# Old Maintainer: EndeavourOS-Team <info@endeavouros.com>
# Maintainer: Calliope System <calliopesystem@gmail.com>

pkgname=grub-tools
pkgdesc="Fixes, additions and enhancements to grub."
pkgver=1.7.0
pkgrel=1
arch=('any')
license=('GPL')
depends=(grub)

url=https://github.com/CalliopeSystem/$pkgname
_url="https://raw.githubusercontent.com/CalliopeSystem/$pkgname/refs/heads/main"

source=(
  $_url/grub-update-after-kernel.hook    # Automatically updates grub.cfg after a kernel or module is installed/uninstalled.
  $_url/grub-update-after-ucode.hook     # Automatically updates grub.cfg after microcode is installed/uninstalled.
)
sha512sums=('850ddcc495c6593dec17d945d5a4b1333551f6a6fa4062aeb70a77fef50367bcc5527b4fdc7407253d53659e2c274490690f9dcd372fb67a1dccd3279ec7592e'
            '6c9498f39e4aa43b42dc1bfcec856a7d8a22ade2089f7e572ab536b667c77883de71ac9cd95b327a3e157db7ad0fc90cce14561678e6138bbee82e2a6a7040d8'
)

package() {
  cd $srcdir

  install -d $pkgdir/usr/share/libalpm/hooks
  install -Dm644 grub-update-after-kernel.hook   $pkgdir/usr/share/libalpm/hooks/grub-update-after-kernel.hook
  install -Dm644 grub-update-after-ucode.hook   $pkgdir/usr/share/libalpm/hooks/grub-update-after-ucode.hook

  install -d $pkgdir/usr/bin
}
