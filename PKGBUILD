# Maintainer: Rafael <rafael@rebornos.org>
# v4.3.0.4520

pkgname=4kyoutubetomp3
pkgver=4.3.0
pkgrel=1
pkgdesc="Turn YouTube links into MP3 files in one click."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('1391e20173bf833330edaa7eedcd1e7d81cdbfc6edc37b0607939f17c8b89cada3cc7ea5a17d73a94a9c3c026a2e20e63aee9eb03c172d8067d78af9907a1dad')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

