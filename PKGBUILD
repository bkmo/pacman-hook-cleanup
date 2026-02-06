# bkmo original

pkgname=pacman-hook-cleanup
pkgver=1.2
pkgrel=1
pkgdesc="Post transaction cleanup of caches"
arch=('any')
url="https://github.com/bkmo/pacman-hook-cleanup"
license=('GPL3')
depends=('pacman' 'pacman-contrib' 'kompare')
makedepends=('git')
provides=('pacman-hook-cleanup')
source=($url/archive/refs/tags/$pkgver.tar.gz)
md5sums=('SKIP')

package() {
 cd $pkgname-$pkgver
 install -Dm755 cleaning-automation -t "$pkgdir/usr/share/libalpm/scripts/"
 install -Dm644 zz-clean_package_cache.hook -t "$pkgdir/usr/share/libalpm/hooks/"
}
