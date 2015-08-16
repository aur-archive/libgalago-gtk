# $Id: PKGBUILD 78820 2012-10-25 06:47:28Z foutrelis $
# Maintainer: Sergej Pupykin <pupykin.s+arch@gmail.com>
# Contributor: William Rea <sillywilly@gmail.com>

pkgname=libgalago-gtk
pkgver=0.5.0
pkgrel=4
pkgdesc="GTK+ widgets for the Galago presence framework"
arch=(i686 x86_64)
url="http://www.galago-project.org"
options=('!libtool')
license=('LGPL')
depends=('gtk2' 'libgalago')
source=(http://www.galago-project.org/files/releases/source/libgalago-gtk/libgalago-gtk-$pkgver.tar.gz)
md5sums=('810f7922ac37ca87d61a0fb0cd830b8b')

build() {
  cd $srcdir/$pkgname-$pkgver
  ./configure --prefix=/usr
  make
  make DESTDIR=$pkgdir install
  rm -rf $pkgdir/usr/share/autopackage
}
