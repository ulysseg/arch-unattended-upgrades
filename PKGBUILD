pkgname='unattended-upgrades'
pkgver=0.0.2
pkgrel=1
arch=('any')
license=('GPL')
source=("unattended-upgrades.service"
	"unattended-upgrades.timer"
	"reboot.hook")
sha256sums=(SKIP SKIP SKIP)

package() {
	mkdir -p "$pkgdir/etc/systemd/system" "$pkgdir/etc/pacman.d/hooks"
	cp unattended-upgrades.service unattended-upgrades.timer "$pkgdir/etc/systemd/system"
	cp reboot.hook "$pkgdir/etc/pacman.d/hooks"
}
