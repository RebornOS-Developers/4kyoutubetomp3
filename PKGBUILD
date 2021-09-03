# Maintainer: Rafael <rafael@rebornos.org>
# v4.2.2.4500

pkgname=4kyoutubetomp3
pkgver=4.2.2
pkgrel=1
pkgdesc="Turn YouTube links into MP3 files in one click."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('43d2e02fa1c24d3d7530b375efea16bd27d27de70b59d0ec0efd6c282b53befd0a10b58bb5699395058f1fc6d7aed43b60c1d4ddd2a9673ae541fc97057fd89b')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

