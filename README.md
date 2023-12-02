# Orangefox Recovery device tree for Infinix Note 10 Pro ID (X695C)

### Blocking checks

- [X] Correct screen/recovery size
- [X] Working Touch, screen
- [X] Backup to internal/microSD
- [X] Restore from internal/microSD
- [ ] reboot to system
- [X] ADB

### Medium checks

- [X] update.zip sideload
- [X] UI colors (red/blue inversions)
- [X] Screen goes off and on
- [X] F2FS/EXT4 Support, exFAT/NTFS where supported
- [X] all important partitions listed in mount/backup lists
- [X] backup/restore to/from external (USB-OTG) storage
- [X] [backup/restore to/from adb](https://gerrit.omnirom.org/#/c/15943/)
- [X] decrypt /data
- [X] Correct date

### Minor checks

- [X] MTP export
- [X] reboot to bootloader
- [X] reboot to recovery
- [X] poweroff
- [X] battery level
- [X] temperature
- [X] input devices via USB (USB-OTG) - keyboard, mouse and disks
- [X] USB mass storage export
- [X] set brightness
- [X] vibrate
- [X] screenshot
- [X] partition SD card

## Building

```bash
source build/envsetup.sh
lunch twrp_X695C-eng
mka bootimage
```

