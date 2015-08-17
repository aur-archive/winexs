# Contributor: Jochum Doring <jochum.doring at gmail>
pkgname=winexs
pkgver=2.0
pkgrel=2
pkgdesc="A gui to make Wine easier to use"
arch=("i686" "x86_64")
url="http://tsx.nl/winexs.html"
license=('GPL')
depends=('libxext' 'lib32-gtk' 'lib32-gtk2')
source=("http://tsx.nl/files/$pkgname-$pkgver.tgz" "winexs.sh")
md5sums=('0dcb5d1f853f9b319a7a492c57da77e4'
         'be4b1946be02a887364f8167bef14bfb') 

build() {
  cd $srcdir/$pkgname
install -d $pkgdir/usr/{bin,share/$pkgname}
install winexs winetricks $pkgdir/usr/share/$pkgname/
install -d $pkgdir/usr/{bin,share/$pkgname/winexs\ Libs/}
install winexs\ Libs/libRBAppearancePak.so winexs\ Libs/libRBShell.so $pkgdir/usr/share/$pkgname/winexs\ Libs/
install -m755 $srcdir/winexs.sh $pkgdir/usr/bin/winexs
}

# vim:set ts=2 sw=2 et:
