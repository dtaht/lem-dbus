# Maintainer: Emil Renner Berthing <esmil@mailme.dk>

pkgname=lem-dbus
pkgver=0.1
pkgrel=1
pkgdesc="DBus library for the Lua Event Machine"
arch=('i686' 'x86_64' 'armv5tel' 'armv7l')
url="https://github.com/esmil/lem-dbus"
license=('GPL')
depends=('lem' 'dbus-core')
source=()

build() {
  cd "$startdir"

  make NDEBUG=1
}

package() {
  cd "$startdir"

  make DESTDIR="$pkgdir/" PREFIX='/usr' install
}

# vim:set ts=2 sw=2 et:
