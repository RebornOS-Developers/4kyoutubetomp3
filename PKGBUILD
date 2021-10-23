# Maintainer: Rafael <rafael@rebornos.org>
# v4.3.2.4560

pkgname=4kyoutubetomp3
pkgver=4.3.2
pkgrel=1
pkgdesc="Turn YouTube links into MP3 files in one click."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('5db9de0365f031d7ad9e96297c7a07f2ff9f3084f313aa924aed14f0c72136b8f0cb95efe94dc9dd80ad24aa4e2594f20cc522ad0e85cc5adecf385aad0dc634')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

