# Maintainer: Ben Ruijl <benruyl@gmail.com>

pkgname=python2-sabyenc
pkgver=3.3.3
pkgrel=1
pkgdesc="Python2 yEnc package optimized for use within SABnzbd"
url="https://github.com/sabnzbd/sabyenc"
arch=('x86_64')
license=("GPL")
depends=("python2")
makedepends=("python2-setuptools")

source=("https://github.com/sabnzbd/sabyenc/archive/v${pkgver}.tar.gz")
md5sums=('c2ed3984ae401507688c96beb7fa604a')

build() {
  cd "${srcdir}/sabyenc-${pkgver}"
  python2 setup.py build
}

package() {
  cd "${srcdir}/sabyenc-${pkgver}"
  python2 setup.py install --root="${pkgdir}" --optimize=1
}
