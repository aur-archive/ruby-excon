# Contributor: Emiliano Vavassori <syntaxerrormmm(at)gmail.com>
# Maintainer: nbryskin
pkgname=ruby-excon
_gemname=excon
pkgver=0.45.3
pkgrel=1
pkgdesc="speed, persistence, http(s)"
arch=('any')
url="https://github.com/geemus/excon"
license=('MIT')
depends=('ruby')
makedepends=('rubygems')
source=(http://rubygems.org/downloads/${_gemname}-${pkgver}.gem)
noextract=(${_gemname}-${pkgver}.gem)
md5sums=('eb53e3adefb409c278a3b38b2b5c6d62')

package() {
  cd "${srcdir}"
  local _gemdir="$(ruby -e'puts Gem.default_dir')"

  gem install --ignore-dependencies --no-user-install -i "${pkgdir}${_gemdir}" "${_gemname}-${pkgver}.gem"
}
