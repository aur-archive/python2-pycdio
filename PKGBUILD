# Maintainer: Alessandro Pezzoni <donbex at nerdshack dot com>
pkgname=python2-pycdio
pkgver=0.19
pkgrel=1
pkgdesc="Python OO interface to libcdio (CD Input and Control library)"
arch=("i686" "x86_64")
url="http://pypi.python.org/pypi/pycdio/"
license=('GPL')
depends=('python2' 'libcdio')
makedepends=('python2-distribute' 'pkg-config' 'swig')
options=(!emptydirs)
source=("http://pypi.python.org/packages/source/p/${pkgname#python2-}/${pkgname#python2-}-${pkgver}.tar.gz")
md5sums=('a6b00666ce8d77ab80a4084a8ff1136b')

package() {
  cd "$srcdir/${pkgname#python2-}-$pkgver"
  python2 setup.py install --root=$pkgdir/ --optimize=1
}

# vim:set ts=2 sw=2 et:
