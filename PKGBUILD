# Maintainer: Rasmus Steinke <rasi at xssn dot at>
# Contributor: Christian Rebischke

pkgname=mppc-git
pkgver=46.b0f491d
pkgrel=1
pkgdesc="a mpc clone written in python"
arch=('any')
url='https://github.com/carnager/mppc'
license=('GPL')
depends=('python-mpd2')
makedepends=('git')
source=('git+http://git.53280.de/mppc')

pkgver() {
	cd mppc
	printf "%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {

  install -D -m755 "${srcdir}/mppc/mppc" \
    "${pkgdir}/usr/bin/mppc"

}

md5sums=('SKIP')
