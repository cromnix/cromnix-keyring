# Maintainer: Chris Cromer <chris@cromer.cl>

pkgname=cromnix-keyring
pkgver=20170619
pkgrel=1
pkgdesc='Cromnix PGP keyring'
arch=('any')
url='https://github.com/cromnix/cromnix-keyring/'
license=('GPL')
install="${pkgname}.install"
source=("${pkgname}-${pkgver}.tar.gz::https://github.com/cromnix/cromnix-keyring/archive/${pkgver}.tar.gz")
md5sums=('10bac2806c58bf90685444421960b683')
validpgpkeys=('A55C3F1BA61CAA63036D82BAFA91071797BEEEC2' # cromer
				'D9B757B7195A485D06A3043932F4AD774C40536B') # artoo

package() {
	cd "${srcdir}/${pkgname}-${pkgver}"
	make PREFIX=/usr DESTDIR=${pkgdir} install
}
