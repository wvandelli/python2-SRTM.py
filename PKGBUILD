# Maintainer: Wainer Vandelli <wainer dot vandelli at gmail dot com>
_name=SRTM.py
pkgname=python2-${_name}
pkgver=0.3.2
pkgrel=1
pkgdesc="Python parser for the Shuttle Radar Topography Mission elevation data"
arch=(any)
url="https://github.com/tkrajina/srtm.py"
license=('Apache')
depends=('python2' 'python2-gpxpy')
makedepends=('python2-setuptools')
provides=()
conflicts=()
replaces=()
backup=()
options=(!emptydirs)
install=
source=(https://files.pythonhosted.org/packages/source/${_name::1}/${_name}/${_name}-${pkgver}.tar.gz)
sha256sums=('08ae42de3e2b76517a476038dfa4078eaff9bf47ed7406d59b630d0af96c842c')

package() {
   cd "${srcdir}/${_name}-${pkgver}"
   python2 setup.py install --root="${pkgdir}" --optimize=1 || exit 1
}
