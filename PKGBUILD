# Maintainer: [Your Name] <your.email@example.com>
pkgname=nix-openrc
pkgver=1.0
pkgrel=1
pkgdesc="OpenRC support for Nix package manager"
arch=('any')
url="https://nixos.org/nix"
license=('GPL')
depends=('nix' 'openrc')
install="$pkgname.install"
source=("nix-daemon.initd" "nix-remote.sh")
sha256sums=('47b6a239785df7a4392d29def666bac5d9bc15b5d1ebab404968c32a18fc1756'
            '0159a5574bb63a846bc36fa6c5a15a353146620fdec42115b3a0840515a35baa')

package() {
  install -Dm755 "$srcdir/nix-daemon.initd" "$pkgdir/etc/init.d/nix-daemon"
  install -Dm755 "$srcdir/nix-remote.sh" "$pkgdir/etc/profile.d/nix-remote.sh"
}
