# Maintainer: Custom Processing Unlimited <cpunltd[at]gmail[dot]com>
# Contributors: Wey (Archlinux forum user)
pkgname=cafepilot-client_beta2
pkgname1=CafePilot_Client
pkgname2=cafepilot-client
pkgver=3.0.0
pkgrel=1
pkgdesc="CafePilot is a cross-platform (Windows and Linux) client/server software suite that makes managing an Internet cafe of any size a breeze. This is the client program."
url="http://www.cafepilot.com"
arch=('any')
license=('GPL')
depends=('java-runtime')
# optdepends=('*')
# makedepends=()
# conflicts=()
# replaces=()
# backup=()
# install='*.install'
source=("http://sourceforge.net/projects/cafepilot/files/CafePilot%203.0.0-beta-2/CafePilot_Client_dist.zip/download"
        "cafepilot-client.sh")
md5sums=('3a2c4a81b3e602c42a169225f090d469'
         'd0ebaad0a19f73ff1ca99a218d79da5d')

package() {
  cd "${srcdir}"
  install -Dm755 $pkgname2.sh $pkgdir/usr/bin/$pkgname2.sh
  install -Dm644 $pkgname1.jar $pkgdir/opt/$pkgname1/$pkgname1.jar
  cp -r "$srcdir"/lib/ "$pkgdir"/opt/$pkgname1/
}

# vim:set ts=2 sw=2 et:
