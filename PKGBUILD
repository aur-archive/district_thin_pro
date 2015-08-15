# Maintainer: James Morris - jwm-art-net - james@jwm-art.net
pkgname=district_thin_pro
pkgver=20150506
pkgrel=1
#depends=('fontconfig' 'xorg-font-utils')
pkgdesc="The thinnest weight from GarageFonts' District family, by Kienan and Dylan Smith."
arch=('any')
url="http://www.philsfonts.com/index.php/free_fonts"
license=('custom:Phil'\''s Fonts/GarageFonts End User License Agreement')
source=(district_thin_pro-${pkgver}.zip::https://philsfonts.com/dl/district_thin_pro.zip)
install=$pkgname.install
md5sums=('3f562ca6770e295579969b1da881e867')

package() {
  cd "${srcdir}/district_thin_pro" || return 1
  install -dm755 "${pkgdir}/usr/share/fonts/OTF" || return 1
  install -m644 *.otf "${pkgdir}/usr/share/fonts/OTF" || return 1
  install -dm755 "${pkgdir}/usr/share/licenses/${pkgname}" || return 1
  install -m644 'GF EULA.pdf' "${pkgdir}/usr/share/licenses/${pkgname}/eula.pdf" || return 1
}

# vim:set ts=2 sw=2 et:
