# Custom Recovery Tree
Buils your own custom recovery for Nokia 5.3 (CAP_sprout).

![cap_sprout](https://static1.xdaimages.com/wordpress/wp-content/uploads/2018/04/TWRP-Feature-Image.png)

| Device                  | Nokia 5.3                                          |
| ----------------------- | ---------------------------------------------------------|
| SoC                     | Qualcomm Snapdragon 665 (11 nm)                      |      
| CPU                     | SM6125  |
| GPU                     | Adreno 610                                             |
| ROM                     | 64 GB Storage                 |
| RAM                     | 4 GB RAM                 |
| Model                   | CAP_sprout |


Blocking checks
- [✓] Correct screen/recovery size
- [✓] Working Touch, screen
- [✓] Backup to internal/microSD
- [✓] Restore from internal/microSD
- [✓] reboot to system
- [✓] ADB

Medium checks
- [✓] update.zip sideload
- [✓] UI colors (red/blue inversions)
- [✓] Screen goes off and on
- [✓] F2FS/EXT4 Support, exFAT/NTFS where supported
- [✓] all important partitions listed in mount/backup lists
- [✓] backup/restore to/from external (USB-OTG) storage (not supported by the device)
- [x] backup/restore to/from adb (https://gerrit.omnirom.org/#/c/15943/)
- [✓] decrypt /data
- [✓] Correct date

Minor checks
- [✓] MTP export
- [✓] reboot to bootloader
- [✓] reboot to recovery
- [✓] poweroff
- [✓] battery level
- [✓] temperature
- [✓] encrypted backups
- [✓] input devices via USB (USB-OTG) - keyboard, mouse and disks (not supported by the device)
- [✓] USB mass storage export
- [✓] set brightness
- [✓] vibrate
- [✓] screenshot
- [✓] partition SD card


# Notes
- Despite using A/B partition scheme, this device has dedicated ramdisk (recovery partition). So just flash it like in any other A-only partition: `fastboot flash recovery twrp-name.img`, it will automatically flash in the active slot.

```
# Copyright (C) 2023 The Android Open Source Project
# Copyright (C) 2023 SebaUbuntu's TWRP device tree generator
# SPDX-License-Identifier: Apache-2.0
```
