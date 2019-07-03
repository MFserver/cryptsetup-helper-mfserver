pkgname=cryptsetup-helper-mfserver
pkgver=1.2
pkgrel=1
depends=('cryptsetup')
pkgdesc="cryptsetup wrapper to simplify mounting and unmounting of volumes the Arch way"
arch=('any')
url="mfserver.net"
source=("cryptmount" "cryptumount")
md5sums=('0e2d9a9b2d53a9de7abc87f9f9e4b224' '5d9032d0bdfe810f2a3281ef1c9440d6')

package() {
  cd ${srcdir}
  install -D -m755 -T cryptmount ${pkgdir}/usr/bin/cryptmount || return 1
  install -D -m755 -T cryptumount ${pkgdir}/usr/bin/cryptumount || return 1
}
