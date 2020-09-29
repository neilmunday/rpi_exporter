pkgname=('rpi_exporter')
pkgver=1
pkgrel=1
pkgdesc='Raspberry Pi metrics exporter for Prometheus'
arch=('any')
license=('GPL')
depends=('python')
source=('rpi_exporter' 'rpi_exporter.service')
md5sums=('7f692df29069d91f9c172884f913ebf6' '4f782b90fe617d310a6141f141a52c99')

package() {
  install -d "$pkgdir"/usr/lib/systemd/system
  install -d "$pkgdir"/usr/bin
  install -m 644 "$srcdir"/rpi_exporter.service "$pkgdir"/usr/lib/systemd/system/
  install -m 755 "$srcdir"/rpi_exporter "$pkgdir"/usr/bin/
}
