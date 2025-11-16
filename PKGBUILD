################################################################
#[PACKAGE]: PKGBUILD
#Copyright © 2024 Allison Munn
#FULL COPYRIGHT NOTICE IS IN README
################################################################
# CONTRIBUTIOR: [FIRST NAME] [LAST NAME] ([EMAIL])
#

# PACKAGE DETAILS
pkgname='';
pkgdesc='';
url='';
license=('GPL-2.0-only');

# group='';
# conflicts=('foobar');
# provides=('foobar=0.0.0');
# replaces=('foobar');

# VERSION DETAILS
arch=('x86_64');
pkgver='0.0.0';
pkgrel=0;
# epoch=0;

# DEPENDENCIES
# depends=( 'dependency-a>=0.0.0' 'dependancy-b>=0.0.0' );
# makedepends=( '' );
# checkdepends=( 'dependency-c>=0.0.0' );
# optdepends=( 'dependency-d: feature support' );

# protocol='https://'
# site='';
source=(
  # "${pkgname}-${pkgver}.tar.gz::${protocol}${site}/${pkgname}-${pkgver}.tar.gz"
  'ICON.png'
  'LICENSE'
  'README.md'         
);
sha512sums=( 'SKIP' 'SKIP' 'SKIP' );

package()
{
  # INSTALL LICENSE
  install -Dm644 'LICENSE' "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE";

  # MAKE DESKTOP ENTRY
  echo -n ''>${pkgname}.desktop;
  echo '[Desktop Entry]'>>${pkgname}.desktop;
  echo 'Type=Application'>>${pkgname}.desktop;
  echo 'Version=1.0'>>${pkgname}.desktop;
  echo 'Name='"${pkgname}">>${pkgname}.desktop;
  echo 'Comment='"${pkgdesc}">>${pkgname}.desktop;
  echo 'Exec='"${pkgname}">>${pkgname}.desktop;
  echo 'Icon='"${pkgname}">>${pkgname}.desktop;
  echo 'Exec='"${pkgname}">>${pkgname}.desktop;

  # INSTALL DESKTOP ENTRY
  install -Dm644 "${pkgname}.desktop" "${pkgdir}/usr/share/applications/${pkgname}.desktop"

  cp "ICON.png" "${pkgname}.png"

  # INSTALL DESKTOP ICON
  install -Dm644 "${pkgname}.png" "${pkgdir}/usr/share/pixmaps/${pkgname}.png"
}

pre_install()
{
  packageVerNew=${1};
}

post_install()
{
  packageVerNew=${1};
}

pre_upgrade()
{
  packageVerNew=${1};
  packageVerOld=${2};
}

post_upgrade()
{
  packageVerNew=${1};
  packageVerOld=${2};
}

pre_remove()
{
  packageVerOld=${1};
}

post_remove()
{
  packageVerOld=${1};
}
