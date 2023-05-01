# Maintainer: Name <E-mail>
# Contributor: William Ghazarian <lvswgh@proton.me>

pkgname="marvin-cli"
pkgver=0.5.1
pkgrel=1
pkgdesc="A command-line tool for interfacing with the Amazing Marvin desktop app and public API."
arch=("x86_64")
url="https://github.com/amazingmarvin/marvin-cli"
license=("custom:Commercial")
depends=('deno')
source=($pkgname-$pkgver::https://github.com/amazingmarvin/marvin-cli/releases/download/v$pkgver/marvin-cli-linux
        LICENSE-$pkgname-$pkgver.txt::https://raw.githubusercontent.com/amazingmarvin/marvin-cli/v0.5.1/LICENSE.txt)
sha256sums=('6274057c8b0711a82c7ec1c065bc94111ef9bd8a93d3174d30f877f5b639c250'
            '81ee649b70c04f896c5628d66a4ee772915075ad7755f2ed6f86e15773a4f10d')

package() {
  install -Dm755 "$pkgname-$pkgver" "$pkgdir/usr/bin/marvin"
  install -Dm755 LICENSE-$pkgname-$pkgver.txt "$pkgdir/usr/share/licenses/$pkgname/LICENSE.txt"
}
