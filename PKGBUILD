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
sha256sums=('1d50f7c8607625de2fd78b3002564bea356ca0599b42c54a3cd4aceaa0f553df'
            '0159a5574bb63a846bc36fa6c5a15a353146620fdec42115b3a0840515a35baa')

package() {
  install -Dm755 "$srcdir/nix-daemon.initd" "$pkgdir/etc/init.d/nix-daemon"
  install -Dm755 "$srcdir/nix-remote.sh" "$pkgdir/etc/profile.d/nix-remote.sh"
}
