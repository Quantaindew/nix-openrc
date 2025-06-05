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
sha256sums=('SKIP' 'SKIP')

package() {
  install -Dm755 "$srcdir/nix-daemon.initd" "$pkgdir/etc/init.d/nix-daemon"
  install -Dm755 "$srcdir/nix-remote.sh" "$pkgdir/etc/profile.d/nix-remote.sh"
}
