# Firmware-Reversing-Notes
The first command ran is the `/etc/inittab` which contains different scripts and executable

If there are multiple squashfs files/part of the firmware, they are reffered to as /dev/mtdblock{ID}. can be mounted with `/bin/mount -t squashfs /dev/mtdblock${ID} /mount_point`
```
cat /proc/mtd 
dev:    size   erasesize  name
mtd0: 01000000 00001000 "whole_flash"
mtd1: 00020000 00001000 "bootloader"
mtd2: 00060000 00001000 "userconfig"
mtd3: 004c0000 00001000 "filesystem1"
mtd4: 00300000 00001000 "kernel1"
mtd5: 00300000 00001000 "kernel2"
mtd6: 004c0000 00001000 "filesystem2"
```
