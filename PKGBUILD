# Maintainer: Pietro Francesco Fontana <pietrofrancesco.fontana@studenti.unimi.it>

_pkgname=cleanupdate
pkgname=cleanupdate-git
pkgver=r62.37a2d12
pkgrel=0
pkgdesc="A simple script to speed up updating and cleaning your system"
arch=('any')
url="https://github.com/cubanpit/$_pkgname"
license=('GPL3')
depends=('ncurses'
		'sudo'
		'bash')
makedepends=('git')
optdepends=('yaourt: update packages from AUR repository (alternative to pacaur)'
		'pacaur: update packages from AUR repository (alternative to yaourt)')
conflicts=()
source=("git://github.com/cubanpit/$_pkgname")
md5sums=('SKIP')

pkgver() {
	printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}
package () {
	cd "$srcdir"
	install -Dm755 "$srcdir/$_pkgname/$_pkgname" "$pkgdir/usr/bin/$_pkgname"
	install -Dm644 "$srcdir/$_pkgname/$_pkgname.desktop" "$pkgdir/usr/share/applications/$_pkgname.desktop"
}
