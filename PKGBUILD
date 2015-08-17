# $Id: PKGBUILD 98749 2013-10-17 14:17:53Z mtorromeo $
# Maintainer: Massimiliano Torromeo <massimiliano.torromeo@gmail.com>

pkgname=python-augeas
pkgver=0.5.0
pkgrel=1
pkgdesc="Pure python bindings for augeas"
arch=('any')
license=('LGPL')
url="http://augeas.net"
depends=(augeas python)
makedepends=('python-setuptools')
source=(https://fedorahosted.org/released/python-augeas/python-augeas-$pkgver.tar.gz)

build() {
    cd "$srcdir/python-augeas-$pkgver"
    python setup.py build
}

package() {
    cd "$srcdir/python-augeas-$pkgver"
    python setup.py install --skip-build -O1 --root="$pkgdir"
}

sha512sums=('d93d9e21c720084ee3c1841a2172dd1a4cfb41e668de0f557bd214efd65e685a1e5fc713a7d34e0fed727fe908bb1e8a09a1c10587bc27f3708cbcdee575cc51')
