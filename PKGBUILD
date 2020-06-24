# Maintainer: Paul Gessinger < paul.gessinger@cern.ch >
pkgname='HepPDT'
pkgver=2.06.01
pkgrel=1
pkgdesc=""
depends=()
url=""
arch=('x86_64')
license=('')
source=(
  "http://lcgapp.cern.ch/project/simu/${pkgname}/download/${pkgname}-${pkgver}.tar.gz"
)

sha256sums=(
  '12a1b6ffdd626603fa3b4d70f44f6e95a36f8f3b6d4fd614bac14880467a2c2e'
)
 


build() {

  cd "$pkgname-$pkgver"

  pwd
  ls
  ./configure --prefix=/usr
  make



}

package() {

  cd "$pkgname-$pkgver"

  make DESTDIR="${pkgdir}" install
}

