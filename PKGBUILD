# Maintainer: ushi <martin.kalcher@gmail.com>
pkgname=update-mirrorlist
pkgver=1.0.8
pkgrel=1
pkgdesc="Update tool for pacmans mirrorlist"
arch=(any)
url="https://github.com/ushis/update-mirrorlist"
license=('GPL')
depends=('coreutils' 'curl' 'pacman' 'iputils' 'grep')
backup=('etc/pacman.d/update-mirrorlist.conf')
install=update-mirrorlist.install
source=('update-mirrorlist'
        'update-mirrorlist.conf'
        'makefile')
md5sums=('3759c398bdb2bade77af3ac070346dd6'
         '1484f46932e249ecb8c2716956ebbc7b'
         '090a56e65fafddff46ea5a60a40d84f7')
package() {
  cd "$srcdir"
  make DESTDIR="$pkgdir" install
}

# vim:set ts=2 sw=2 et:
