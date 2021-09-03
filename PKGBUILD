# Maintainer: Rafael <rafael@rebornos.org>
# v3.4.3.3630

pkgname=4kstogram
pkgver=3.4.3
pkgrel=1
pkgdesc="Download Instagram photos, accounts, hashtags and locations."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('49f66db3e53a93532e054c78d49e384106ed67b3164776c23cc8cfbc4f3f0da796f1751245a82dbd1c65128f4f210dcb7627e8a6c5f513f44958a4ff87069623')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

