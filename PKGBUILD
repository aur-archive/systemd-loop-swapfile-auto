# Maintainer: Timofey <Nefelim4ag@gmail.com>
pkgname=systemd-loop-swapfile-auto
_pkgname=systemd-loop-swapfile-auto
pkgver=1.21
pkgrel=1
pkgdesc="Auto create dinamic growing swap file and mount it via loop"
arch=('any')
url="https://btrfs.wiki.kernel.org/index.php/FAQ#Does_btrfs_support_swap_files.3F"
license=('GPL')
source=(systemd-loop-swapfile.*)
depends=('systemd')
md5sums=('b4e7c4efc3ebc243434c379d82488e01'
         '001ad5c6bb57ab17be0375f3a343d67b'
         '36e1c6338326f297686a2e115f432289')

package() {
  install -Dm755 systemd-loop-swapfile.service $pkgdir/etc/systemd/system/systemd-loop-swapfile.service
  install -Dm755 systemd-loop-swapfile.sh $pkgdir/usr/lib/systemd/scripts/systemd-loop-swapfile.sh
  install -Dm755 systemd-loop-swapfile.conf $pkgdir/etc/systemd-loop-swapfile.conf
}