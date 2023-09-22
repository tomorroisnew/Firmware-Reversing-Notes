# Firmware-Reversing-Notes
The first command ran is the `/etc/inittab` which contains different scripts and executable

If there are multiple squashfs files, they are reffered to as /dev/mtdblock{ID}. can be mounted with `/bin/mount -t squashfs /dev/mtdblock${ID} /mount_point`
