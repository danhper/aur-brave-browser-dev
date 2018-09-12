# Maintainer: Daniel Perez <daniel@perez.sh>

pkgname=brave-dev-bin
pkgver=0.50.14
pkgrel=1
pkgdesc='Web browser that blocks ads and trackers by default (dev version, binary release).'
arch=('x86_64')
url='https://www.brave.com'
license=('custom')
depends=('gtk3' 'gconf' 'nss' 'alsa-lib' 'libxss' 'libgnome-keyring' 'ttf-font')
optdepends=('cups: Printer support'
            'pepper-flash: Adobe Flash support')
provides=("${pkgname%-bin}" 'brave-browser-dev')
conflicts=("${pkgname%-bin}")
source=("https://brave-browser-apt-dev.s3.brave.com/pool/main/b/brave-browser-dev/brave-browser-dev_0.50.14_amd64.deb")
options=(!strip)
sha256sums=('319b925220d07cc4810fd9848a1d09a53d0d66e31e3ea0a8f892336fa26ac1c0')

package() {
    tar -xf data.tar.xz -C "${pkgdir}" --no-same-permissions
}
