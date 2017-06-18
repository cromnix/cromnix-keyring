# Maintainer: Chris Cromer <chris@cromer.cl>

pkgname=cromnix-keyring
pkgver=20170618
pkgrel=1
pkgdesc='Cromnix PGP keyring'
arch=('any')
url='https://github.com/cromnix/cromnix-keyring/'
license=('GPL')
install="${pkgname}.install"
source=("${pkgname}-${pkgver}::https://github.com/cromnix/cromnix-keyring/archive/${pkgver}.tar.gz")
md5sums=('183822966119dc095bc74c3e4387caf2')
validpgpkeys=('A55C3F1BA61CAA63036D82BAFA91071797BEEEC2') # cromer

package() {
	cd "${srcdir}/${pkgname}-${pkgver}"
	make PREFIX=/usr DESTDIR=${pkgdir} install
}
