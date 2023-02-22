# Contributor: ivanp7
# Maintainer: ivanp7

_pkgname=slock
pkgname=$_pkgname-ivanp7
pkgver=1.5
pkgrel=1
pkgdesc="Simple X display locker"
url='http://tools.suckless.org/slock'
arch=('i686' 'x86_64' 'armv7h')
license=('custom:MIT/X')
depends=('libxrandr')
makedepends=('git')
provides=("$_pkgname")
conflicts=("$_pkgname")
source=('arg.h' 'config.h' 'config.mk' 'LICENSE' 'Makefile' 'slock.1' 'slock.c' 'util.h')
sha256sums=('5f4ecca1bb057a6d6301aff8f2b403e723af5dc86a5e00e8c7e5c2f56cdb9c79'
            'e4c8e470dcd320c2f4c90bb47b136e06193b8edf6ffc0060b7a91144c7c90349'
            '8eb620af5293d8ff6853d263978e2ba3712ba4e64faa3ee276b52be43351c4ea'
            'a03eada2c7b597102845c091869529ed9a4493e1f149756459422f6082fbef0d'
            'e047fb2961ae2ba92af57955257395f2aa3b36e0c1e749fd4b1353d9a3e7b70d'
            '1254329f174ce9c7884275e6e9bb1ecb3383131b05e5c96906512aeb6e423f4d'
            '5ba4f950c4a3eafb7f4325a6ef5858789fce4381ade045c58a0be3a3197587b4'
            'd1a94d121774e91849b372458eec284f65104f01dec71f01390f397fa98c4e47')

build() {
  make PREFIX=/usr DESTDIR="$pkgdir"
}

package() {
  make PREFIX=/usr DESTDIR="$pkgdir" install
  install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

