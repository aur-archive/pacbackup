# Maintainer: Adrien Bak <adrien.bak+aur@gmail.com>
pkgname=pacbackup
pkgver=1.0.3
pkgrel=1.0
pkgdesc="Backs up the list of all explicitly installed packaged and provides restoration script"
arch=('any')
url="http://www.abak.io/pacbackup"
license=('BSD')
groups=()
depends=('python>=3.4' 'git>=2.1.0' 'pyalpm>=0.6.2' 'python-pygit2>=0.21')
makedepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=(!emptydirs)
install=
source=("https://github.com/abak/pacbackup/releases/download/1.0.3/pacbackup-1.0.3.tar.gz")
md5sums=('c4ff097fca6d3f0e1135d839a04e5877')

package() {
  cd "$srcdir/$pkgname-$pkgver"
  python3 setup.py install --root="$pkgdir/" --optimize=1

  install -D -m644 LICENSE.md "${pkgdir}/usr/share/licenses/$_pkgname"

}

