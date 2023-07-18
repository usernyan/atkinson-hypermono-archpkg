# Maintainer: User Nyan <74884883+usernyan@users.noreply.github.com>
pkgname='atkinson-hypermono-git'
pkgver=1
pkgrel=1
pkgdesc="Monospaced version of Atkinson Hyperlegible"
arch=('x86_64')
license=('unknown')
makedepends=('git')
source=("$pkgname::git+https://github.com/nino/Atkinson-Hypermono")
md5sums=("SKIP")

pkgver() {
	cd "$pkgname"
	printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
	install -Dm644 -t "$pkgdir/usr/share/fonts/OTF/" $pkgname/*.otf
}
