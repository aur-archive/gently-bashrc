# Maintainer: Gently <toddrpartridge@gmail.com>

pkgname=gently-bashrc
_pkgname=${pkgname/-/.}
pkgver=0.87
pkgrel=1
pkgdesc="A thorough bash configuration file meant to replace the local ~/.bashrc."
arch=("any")
url="https://github.com/Gen2ly/gently-bashrc"
license=("GPL2")
depends=("")
makedepends=("git")
install=${pkgname}.install
changelog=
source=("git://github.com/Gen2ly/gently-bashrc")
md5sums=('SKIP')

pkgver() {
  cd "$srcdir"/$pkgname
  git describe | sed 's/^v//;s/-.*//'
}

package() {
  cd "$srcdir/$pkgname"
  install -Dm644 $_pkgname   "$pkgdir"/usr/share/doc/$pkgname/$_pkgname
  install -Dm644 license.txt "$pkgdir"/usr/share/licenses/$pkgname/license.txt
}

# vim:set ts=2 sw=2 et:
