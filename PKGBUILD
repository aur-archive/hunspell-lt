# Maintainer: Algimantas Margevičius <algimantas@margevicius.lt>
pkgname=hunspell-lt
pkgver=1.1
pkgrel=2
pkgdesc="Lithuanian language for hunspell"
arch=('any')
url="http://margevicius.lt/myspell-lt-1.3.zip"
license=('GPL')
groups=()
depends=('hunspell'
		     'hyphen')
source=("http://margevicius.lt/myspell-lt-1.3.zip")
md5sums=("11320c87b4fd39726053fe7f6647a62c") 

package() {
	cd "${srcdir}/myspell-lt-1.3"
	install -dm755 "${pkgdir}/usr/share/hunspell"
	install -dm755 "${pkgdir}/usr/share/myspell"
	install -D -m644 "lt_LT.aff"	"${pkgdir}/usr/share/myspell/lt_LT.aff"  
	install -D -m644 "lt_LT.dic"	"${pkgdir}/usr/share/myspell/lt_LT.dic" 
	install -D -m644 "lt_LT.aff"	"${pkgdir}/usr/share/hunspell/lt_LT.aff"  
	install -D -m644 "lt_LT.dic"	"${pkgdir}/usr/share/hunspell/lt_LT.dic" 
	install -D -m644 "README" "${pkgdir}/usr/share/docs/hunspell-lt/README"
}
