# Maintainer: Ben Ruijl <benruyl@gmail.com>

pkgname=python2-sabyenc
pkgver=3.3.0
pkgrel=1
pkgdesc="Python2 yEnc package optimized for use within SABnzbd"
url="https://github.com/sabnzbd/sabyenc"
arch=('i686' 'x86_64')
license=("GPL")
depends=("python2")
makedepends=("python2-setuptools")

source=("https://github.com/sabnzbd/sabyenc/archive/v${pkgver}.tar.gz")
md5sums=('67b6f73c1ea11c70b85a7d914d8e18f1')

build() {
  cd "${srcdir}/sabyenc-${pkgver}"
  python2 setup.py build
}

package() {
  cd "${srcdir}/sabyenc-${pkgver}"
  python2 setup.py install --root="${pkgdir}" --optimize=1
}
