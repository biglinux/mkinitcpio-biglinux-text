# Maintainer: Bruno Goncalves <biglinux.com.br>

pkgname=mkinitcpio-biglinux-text
pkgver=1
pkgrel=1
arch=('any')
license=('')
url="https://github.com/biglinux/mkinitcpio-biglinux-text"
pkgdesc="Add text in boot saying BIGLINUX and hardware informations"

source=('git+https://github.com/biglinux/mkinitcpio-biglinux-text.git')
sha256sums=('SKIP')
makedepends=('git')
install=${pkgname}.install

pkgver() {
    cd ${pkgname}
    printf "1_r$(git rev-list --count HEAD)_$(date "+%Y_%m_%d")"
}


package() {
    cp -r "${srcdir}/${pkgname}/usr" "${pkgdir}/usr"
}

