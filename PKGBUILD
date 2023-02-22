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

build() {
  make PREFIX=/usr DESTDIR="$pkgdir"
}

package() {
  make PREFIX=/usr DESTDIR="$pkgdir" install
  install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

sha256sums=('5f4ecca1bb057a6d6301aff8f2b403e723af5dc86a5e00e8c7e5c2f56cdb9c79'
            '837269668b209d204b29b49753b4465e4f6ed55004f8358e74162409c15ae03e'
            '438a17027c5f48d6e88a1ebc690dcc55f40e40dfa8ccdeee9694f92075b3eee9'
            'a03eada2c7b597102845c091869529ed9a4493e1f149756459422f6082fbef0d'
            'e047fb2961ae2ba92af57955257395f2aa3b36e0c1e749fd4b1353d9a3e7b70d'
            '1254329f174ce9c7884275e6e9bb1ecb3383131b05e5c96906512aeb6e423f4d'
            '60cb7a372cbb3403105c0230a39b3794aa080885afb184e551776c77ecde5a1e'
            'd1a94d121774e91849b372458eec284f65104f01dec71f01390f397fa98c4e47')
sha256sums=('5f4ecca1bb057a6d6301aff8f2b403e723af5dc86a5e00e8c7e5c2f56cdb9c79'
            '837269668b209d204b29b49753b4465e4f6ed55004f8358e74162409c15ae03e'
            '6b5a81c7a633d00e8a1658922d90213309f2ceb5c3dd321a13994d8e48a9ea04'
            'a03eada2c7b597102845c091869529ed9a4493e1f149756459422f6082fbef0d'
            'e047fb2961ae2ba92af57955257395f2aa3b36e0c1e749fd4b1353d9a3e7b70d'
            '1254329f174ce9c7884275e6e9bb1ecb3383131b05e5c96906512aeb6e423f4d'
            '60cb7a372cbb3403105c0230a39b3794aa080885afb184e551776c77ecde5a1e'
            'd1a94d121774e91849b372458eec284f65104f01dec71f01390f397fa98c4e47')
