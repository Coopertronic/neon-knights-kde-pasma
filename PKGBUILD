# Maintainer: Matthew Phillip Cooper <matthew@coopertronic.co.uk>
pkgname=neon-knights-kde-pasma
_destname1="/usr"
pkgver=1.r15.e9f63bc
pkgrel=1
pkgdesc="This installs the Neon Knights global theme for KDE plasma by ju1464."
arch=('any')
url="https://github.com/Coopertronic/neon-knights-kde-pasma.git"
license=('GPL3')
makedepends=('git')
depends=('plasma-desktop')
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=("git+$url")
sha256sums=('SKIP')

pkgver() {
    printf "1.r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
}
