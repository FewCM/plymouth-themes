# Maintainer: Aditya Shakya <adi1090x@gmail.com>

pkgname=plymouth-themes
pkgver=1.0
pkgrel=1
pkgdesc="plymouth themes"
arch=('any')
license=('GPL3')
makedepends=()
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)

prepare() {
	cp -af ../files/. ${srcdir}
}

package() {
	(find archcraft -type f -exec install -Dm 644 "{}" "$pkgdir/usr/share/plymouth/themes/{}" \;
	 find spin -type f -exec install -Dm 644 "{}" "$pkgdir/usr/share/plymouth/themes/{}" \;
	 find circle -type f -exec install -Dm 644 "{}" "$pkgdir/usr/share/plymouth/themes/{}" \;
	)
	
}
