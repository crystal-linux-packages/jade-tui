# Maintainer: echo -n 'bWF0dEBnZXRjcnlzdC5hbA==' | base64 --decode
# Contributor: echo -n 'cmNhbmRhdUBnZXRjcnlzdC5hbA==' | base64 -d

pkgname=jade-tui
pkgver=1.0.0
pkgrel=2
pkgdesc="Tui frontend for the jade installer"
license=('GPL3')
arch=('any')
url="https://github.com/crystal-linux/${pkgname}"
depends=('jade' 'gum' 'openssl')
source=("${pkgname}-${pkgver}::${url}/archive/v${pkgver}.tar.gz")
sha256sums=('faf95c456e5d10c92372ccc007cbb25f4f65b43d7016e99388cffdc8d9abf982')

package() {
    cd "${srcdir}/${pkgname}-${pkgver}"
    install -Dm 755 "${pkgname}" "${pkgdir}/usr/bin/${pkgname}"
    install -Dm 644 locales "${pkgdir}/usr/share/${pkgname}/locales"
}
