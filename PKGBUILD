# Maintainer: codydg <codydgraham@gmail.com>
pkgname=installable-package
pkgver=0.1
pkgrel=1
pkgdesc="Test making a package for Arch Linux"
arch=('any')
url="https://github.com/codydg/InstallableProject"
license=('APACHE')
provides=('installable-package')
conflicts=('installable-package')
source=("$pkgname-$pkgver::git+https://github.com/codydg/InstallableProject.git")
md5sums=('SKIP')

build() {
    cd "$pkgname-$pkgver"
    make
}

package() {
    cd "$pkgname-$pkgver"
    make DESTDIR="$pkgdir/" install
}
