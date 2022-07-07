# Maintainer: Vivek Pal <vivek@shastraos.co>

pkgname=shastraos-artwork
pkgver=0.1
pkgrel=1
pkgdesc="ShastraOS Logos and Wallpapers"
url="https://github.com/shastra-os/artwork"
arch=('any')
license=('GPL3')
makedepends=()
depends=()
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)

prepare() {
	cp -af ../files/. ${srcdir}
}

package() {
	(find * -type f -exec install -Dm 644 "{}" "$pkgdir/usr/share/shastraos/artwork/{}" \;)
}


