pkgname=ttf-babelstone-phagspa
pkgver=2.00
pkgrel=1
pkgdesc="Phags-pa fonts with OpenType features that allow complex joining and shaping behaviour."
arch=('any')
url="http://www.babelstone.co.uk/Fonts/Phags-pa.html"
license=('custom:OFL')
depends=('fontconfig' 'xorg-font-utils')
source=('http://www.babelstone.co.uk/Fonts/BabelStonePhagspaBook_v2.ttf'
        'http://www.babelstone.co.uk/Fonts/BabelStonePhagspaTibetanA_v2.ttf'
        'http://www.babelstone.co.uk/Fonts/BabelStonePhagspaTibetanB_v2.ttf'
        'http://www.babelstone.co.uk/Fonts/BabelStonePhagspaSeal_v1.ttf'
        'http://www.babelstone.co.uk/Fonts/BabelStoneOFL.txt')
sha256sums=('bcb283be644f31301bfe0e2a17d339d43058daedd253dcb6138036310024a0f5'
            '4ba3d7f26328e7dcd66d4a84587d8739d650f6ee8ea9da426c019bf11216d87e'
            'c4aa63d75f0b1639bc77bb0f3b52e65b0e6e03ba31dd8f6d0c075712903bae6a'
            'f2cf198b3dd867286a7535182adbd969a7f7bfa0c70f7825d83848ba72b13a5f'
            'd2b1b6e4e9201832e94e6f9231b6c32488cb76ea30c4ef82ca3fac35ec2f0b66')
install=$pkgname.install

package()
{
  mkdir -p $pkgdir/usr/share/fonts/TTF
  install -m644 $srcdir/*.ttf $pkgdir/usr/share/fonts/TTF

  install -Dm644 $srcdir/BabelStoneOFL.txt $pkgdir/usr/share/licenses/$pkgname/LICENSE
}
