# Maintainer: Andrii Burkivskyi <buryk212@gmail.com>
pkgname=vidoas
pkgver=1.0
pkgrel=1
pkgdesc="Edits a doas.conf file and autochecks it for errors before saving."
arch=('x86_64' 'i686')
url="https://github.com/le0me55i/vidoas"
license=('BSD')
depends=('opendoas' 'pam')
optdepends=('opendoas-sudo')
makedepends=('git')
provides=('vidoas')
conflicts=('vidoas')
backup=(etc/doas.conf)
source=('vidoas::git+https://github.com/le0me55i/vidoas.git')
md5sums=('SKIP')

package() {
	cd "$pkgname"
	install -Dm644 "$pkgname" "$pkgdir"/usr/local/bin/"$pkgname"
	install -Dm644 LICENSE "$pkgdir"/usr/share/licenses/vidoas/LICENSE
}
