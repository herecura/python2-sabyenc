# Maintainer: Ben Ruijl <benruyl@gmail.com>

pkgname=python2-sabyenc
pkgver=3.3.4
pkgrel=1
pkgdesc="Python2 yEnc package optimized for use within SABnzbd"
url="https://github.com/sabnzbd/sabyenc"
arch=('x86_64')
license=("GPL")
depends=("python2")
makedepends=("python2-setuptools")

source=("https://github.com/sabnzbd/sabyenc/archive/v${pkgver}.tar.gz")
md5sums=('1088c7d830dbc37b6685990d7fe1f130')

build() {
  cd "${srcdir}/sabyenc-${pkgver}"
  python2 setup.py build
}

package() {
  cd "${srcdir}/sabyenc-${pkgver}"
  python2 setup.py install --root="${pkgdir}" --optimize=1
}
