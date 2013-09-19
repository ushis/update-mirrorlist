# Maintainer: ushi <martin.kalcher@gmail.com>
pkgname=update-mirrorlist
pkgver=1.0.10
pkgrel=1
pkgdesc="Update tool for pacmans mirrorlist"
arch=(any)
url="https://github.com/ushis/update-mirrorlist"
license=('GPL')
depends=('coreutils' 'curl' 'pacman' 'iputils' 'grep')
backup=('etc/pacman.d/update-mirrorlist.conf')
install=update-mirrorlist.install

source=(
  'update-mirrorlist'
  'update-mirrorlist.conf'
)

sha256sums=(
  'af1ec558e833d2fe37e59235fc2c8210d925caa080be74c889c6506f0e2c1dba'
  '70f63174373cb6bdecb1e6b9537dc5bbb85483d69ae290a01b1d88370d446c95'
)

package() {
  cd "$srcdir"
  install -D -m755 'update-mirrorlist'      "${pkgdir}/usr/bin/update-mirrorlist"
  install -D -m644 'update-mirrorlist.conf' "${pkgdir}/etc/pacman.d/update-mirrorlist.conf"
}

# vim:set ts=2 sw=2 et:
