# Maintainer: Pietro Francesco Fontana <pietrofrancesco.fontana@studenti.unimi.it>

_pkgname=cleanupdate
pkgname=cleanupdate-git
pkgver=0.2
pkgrel=2
pkgdesc="A simple script to speed up updating and cleaning your system"
arch=('any')
url="https://github.com/cubanpit/$_pkgname"
license=('GPL3')
depends=('ncurses')
makedepends=('git')
optdepends=('yaourt: update packages from AUR repository (alternative to pacaur)'
		'pacaur: update packages from AUR repository (alternative to yaourt)')
conflicts=()
source=("git://github.com/cubanpit/$_pkgname")
md5sums=('SKIP')

package () {
	cd "$srcdir"
		install -Dm755 "$srcdir/$_pkgname/$_pkgname" "$pkgdir/usr/bin/$_pkgname"
}
