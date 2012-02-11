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
source=('update-mirrorlist' 'update-mirrorlist.conf')
md5sums=('a6aa441dbf4d7c6af3b91f7361eac887'
         'b13a7e783d0a84ea75704b6f4f8ce57c')

package() {
  cd "$srcdir"
  make DESTDIR="$pkgdir" install
}

# vim:set ts=2 sw=2 et:
