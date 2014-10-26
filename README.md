
Different stuff just like a memo (primary for usage by myself):
it will be (possibly) reordered by topics...

copy of entire 512GiB HDD content including MBR and partitions table from /dev/sda to files with gzip compression and 2GiB split:
`dd if=/dev/sda bs=8M count=65536 | gzip | split -d -b 2G /media/sfSHARED/hdd512GiB.img.gz_`

append existing user "user1" into existing group "vboxsf" (for example for VirtualBox shared folder usage)
`sudo usermode -a -G vboxsf user1`

a few commands usable for dealing with partitions
`sudo blkid`  `fdisk -l`
