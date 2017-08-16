pkgname=cryptsetup-helper-mfserver
pkgver=1.1
pkgrel=1
depends=('cryptsetup')
pkgdesc="cryptsetup wrapper to simplify mounting and unmounting of volumes the Arch way"
arch=('any')
url="mfserver.net"
source=("cryptmount" "cryptumount")
md5sums=('a697d70c38736a6f48dcf55562e69438' '80c6fce493aae0232b852eeb13166138')

package() {
  cd ${srcdir}
  install -D -m755 -T cryptmount ${pkgdir}/usr/bin/cryptmount || return 1
  install -D -m755 -T cryptumount ${pkgdir}/usr/bin/cryptumount || return 1
}