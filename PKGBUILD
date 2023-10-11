# Contributor: noonov <noonov@gmail.com>

pkgname=ttf-monapo
pkgver=20170722
pkgrel=2
pkgdesc="A Japanese font for viewing Japanese ascii arts properly"
arch=('any')
url="https://github.com/utuhiro78/modified-fonts"
license=('custom')
depends=('fontconfig' 'xorg-mkfontscale')
source=(https://raw.githubusercontent.com/utuhiro78/modified-fonts/main/monapo-20170722.tar.xz)
sha256sums=('f1cf49006f9ef3079e95b2808c8727727aa664006502c9b52fa268bbe901d3cd')

package() {
	cd ${srcdir}/monapo-${pkgver}

	install -D -m644 monapo.ttf ${pkgdir}/usr/share/fonts/TTF/monapo.ttf

	install -D -m644 ipagp00303/IPA_Font_License_Agreement_v1.0.txt \
		${pkgdir}/usr/share/licenses/${pkgname}/COPYING_IPA.txt
}
