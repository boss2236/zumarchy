# Zumarchy ISO (archiso profile)

This directory holds the [archiso](https://wiki.archlinux.org/title/Archiso) profile
used to build the bootable Zumarchy live/install medium.

```bash
sudo pacman -S --needed archiso
sudo mkarchiso -v -w /tmp/zumarchy-work -o ./out iso/profile
# -> ./out/zumarchy-<version>-x86_64.iso
```

The profile is derived from Arch's `releng` profile, rebranded for Zumarchy
(boot menus, volume label, MOTD logo) and shipping `zumarchy-install` plus the
Zumarchy logo in `airootfs/`. Built ISOs are not committed (too large); build
locally with the command above.
