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
    install -Dm0644 "$pkgdir/opt/brave.com/brave-dev/product_logo_16.png" "$pkgdir/usr/share/icons/hicolor/16x16/apps/brave-browser-dev.png"
    install -Dm0644 "$pkgdir/opt/brave.com/brave-dev/product_logo_22.png" "$pkgdir/usr/share/icons/hicolor/22x22/apps/brave-browser-dev.png"
    install -Dm0644 "$pkgdir/opt/brave.com/brave-dev/product_logo_24.png" "$pkgdir/usr/share/icons/hicolor/24x24/apps/brave-browser-dev.png"
    install -Dm0644 "$pkgdir/opt/brave.com/brave-dev/product_logo_32.png" "$pkgdir/usr/share/icons/hicolor/32x32/apps/brave-browser-dev.png"
    install -Dm0644 "$pkgdir/opt/brave.com/brave-dev/product_logo_48.png" "$pkgdir/usr/share/icons/hicolor/48x48/apps/brave-browser-dev.png"
    install -Dm0644 "$pkgdir/opt/brave.com/brave-dev/product_logo_64.png" "$pkgdir/usr/share/icons/hicolor/64x64/apps/brave-browser-dev.png"
    install -Dm0644 "$pkgdir/opt/brave.com/brave-dev/product_logo_128.png" "$pkgdir/usr/share/icons/hicolor/128x128/apps/brave-browser-dev.png"
    install -Dm0644 "$pkgdir/opt/brave.com/brave-dev/product_logo_256.png" "$pkgdir/usr/share/icons/hicolor/256x256/apps/brave-browser-dev.png"

}
