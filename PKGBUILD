# Maintainer: Dirk Traenapp <dirk.traenapp@nwowhv.de>
pkgname=synology-chat
pkgver=1.1.1
pkgrel=57
pkgdesc="Chat Client for Synology Chat"
arch=('i686' 'x86_64')
url="https://www.synology.com/support/download/"
license=('(C) Synology: Proprietary')
#depends=('')
makedepends=('rpmextract')
options=('emptydirs')

# https://www.synology.com/en-us/support/download/DS216
if [[ ${CARCH} == "i686" ]]; then
    source=("https://global.download.synology.com/download/Tools/ChatClient/${pkgver}-${pkgrel}/Fedora/i686/Chat-${pkgver}-${pkgrel}.i686.rpm")
    md5sums=('4356702559e164c80d5ba10fbe4dc81d')
elif [[ ${CARCH} == "x86_64" ]]; then
    source=("https://global.download.synology.com/download/Tools/ChatClient/${pkgver}-${pkgrel}/Fedora/x86_64/Chat-${pkgver}-${pkgrel}.x86_64.rpm")
    md5sums=('61b06e2696e39378075ebbea18812086')
fi

package() {
    cp -rf $srcdir/opt $pkgdir/
    cp -rf $srcdir/usr $pkgdir/
}
