# Maintainer: Rafael <rafael@rebornos.org>
# v4.3.1.4540

pkgname=4kyoutubetomp3
pkgver=4.3.1
pkgrel=1
pkgdesc="Turn YouTube links into MP3 files in one click."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('7706ab1408a70723a9448b99be71fcc1cdf7d10d1b8e92cf83ba9d8af20238ba024296ddbcdcddd58565fc563e7ac1d55e309305065031842691863f53944b8c')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

