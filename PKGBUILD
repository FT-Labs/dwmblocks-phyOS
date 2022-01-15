# Maintainer: Arda Atci<phystecharda@gmail.com>
pkgname=dwmblocks-phyOS
pkgver=1
pkgrel=1
pkgdesc="dwmblocks build for phyOS"
arch=(x86_64)
url="git://github.com/PhyTech-R0/dwmblocks-phyOS"
license=('MIT')
makedepends=('git' 'make')
optdepends=('dwm')
provides=("dwmblocks")
conflicts=("dwmblocks")
options=('zipman')
source=('git://github.com/PhyTech-R0/dwmblocks-phyOS')
md5sums=('SKIP')

build() {
	cd "$pkgname"
	make
}

package() {
	cd "$pkgname"
	make PREFIX=/usr/local DESTDIR="$pkgdir/" install
}
