My settings for a FAT32 USB having several distros, for testing, fun, rescue files, fix computer problems...

USB should have an ext3 partition named `persistence` for use persistence in Kali. This partition should contain a file named `persistence.conf` with the content `/ union`.

You could have persistence for other distros too with other partitions, but I'm only interested in having kali tools up-to-date.

For System Rescue CD, modify `boot/grub/grub.cfg` and in System Rescue entry, change img_label=`MY_USB` with the label of your FAT32 partition holding the isos
