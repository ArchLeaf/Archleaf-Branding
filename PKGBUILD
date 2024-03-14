# Maintainer: Crystal Linux Distribution Team <distribution@lists.getcryst.al>

pkgname=archleaf-branding
_pkgname=Logo
pkgver=v1.0.0
pkgrel=2
pkgdesc='Archleaf branding'
arch=('x86_64')
url="https://gitea.com/Archleaf/${_pkgname}"
license=('GPL-3.0-only')
depends=('lsb-release')
install="${pkgname}.install"
source=("${url}/archive/${pkgver}.tar.gz"
	"os-release_archleaf"
	"issue_archleaf"
	"lsb-release_archleaf")
sha256sums=('e50d71236c7046cbaaa7c350e04f9b3542ffdef91fa3d9cd2bc67110a92a51aa'
            '823540d422787095c2a418730de5928235939c9b514aca5f5ba1de7bd7f06312'
            '44cf3a946e18d57a4428c611df151b50445d680762f31e682c87dece0bf287f8'
            '535666225e9ba5b039d43ac760cbf6b623a58427eacec3bde776df0881497dc6')

package () {
    cd "logo"
    install -Dm 644 Logo/Branding-ArchLeaf.png "${pkgdir}/usr/share/pixmaps/branding-archLeaf.png"
    install -Dm 644 ../os-release_archleaf "${pkgdir}/etc/os-release_archleaf"
    install -Dm 644 ../os-release_archleaf "${pkgdir}/usr/lib/os-release_archleaf"
    install -Dm 644 ../issue_archleaf "${pkgdir}/etc/issue_archleaf"
    install -Dm 644 ../lsb-release_archleaf "${pkgdir}/etc/lsb-release_archleaf"
}
