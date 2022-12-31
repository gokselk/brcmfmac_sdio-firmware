# Maintainer: Goksel Kabadayi <goksel@goksel.xyz>
pkgname=brcmfmac_sdio-firmware
pkgver=r82.528134d
pkgrel=1
pkgdesc="Firmware for the Broadcom SDIO 802.11a/b/g/n/ac wireless chips"
url="https://github.com/LibreELEC/brcmfmac_sdio-firmware"
license=('custom')
arch=('any')
depends=()
source=("${url}/archive/528134d76f87bdd39d6f1ab27d20f28f1759434e.tar.gz")
sha256sums=('711097858a8d86912a9746d2095eb7db3b3c743bf918cf8e9957fcdad402be1a')

package() {
    cd "${srcdir}/${pkgname}-528134d76f87bdd39d6f1ab27d20f28f1759434e"
    rm -rf .[!.]* *.md
    install -d "${pkgdir}/usr/lib/firmware/brcm"
    cp -r * "${pkgdir}/usr/lib/firmware/brcm"
}
