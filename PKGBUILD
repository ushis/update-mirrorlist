# Maintainer: ushi <martin.kalcher@gmail.com>
pkgname=update-mirrorlist
pkgver=1.0
pkgrel=1
pkgdesc="Update tool for pacmans mirrorlist"
arch=(any)
url="https://github.com/ushis/update-mirrorlist"
license=('GPL')
depends=('coreutils' 'wget' 'pacman' 'iputils' 'grep')
backup=('etc/pacman.d/update-mirrolist.conf')
install=update-mirrorlist.install
source=()
md5sums=()

package() {
  cd "$srcdir"
  make DESTDIR="$pkgdir" install
}

# vim:set ts=2 sw=2 et:
