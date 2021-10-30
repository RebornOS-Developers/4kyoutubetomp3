# Maintainer: Rafael <rafael@rebornos.org>
# v4.3.3.4570

pkgname=4kyoutubetomp3
pkgver=4.3.3
pkgrel=1
pkgdesc="Turn YouTube links into MP3 files in one click."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('c8b4f3b690b9a073f9d0e138de9165a59b4e7b9d1bc33f2873f8a4ab591d96d7c29fe01836b11c501ec957a0ea36d875e5e3baaabebe584fe52cf4a521666220')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

