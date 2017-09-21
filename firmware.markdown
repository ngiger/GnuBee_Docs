---
layout: default
title: Install firmware
---

Assuming that you have GnuBee PC1 without any upgraded firmware nor installed linux distribution you have two choices using the built-in webserver or using a USB-stick.

The GnuBee PC 1 has a 32MB soldered on Flash-chip. It contains 6 parts. Their names (u-boot,
u-boot-env, factory,firmware,kernel,rootfs,rootfs_data) should be self-explanatory.

Upgrading the firmware as documented here, will replace the content of  the firmware,kernel,rootfs and rootfs_data.

All the firmware discussed here, have the following common characteristics:

* The mount a read/write overlay partition, where changes are preserverd over reoboots. This allows you to add more packages, download scripts, change password, etc.
* By default there is no root password.
* After the startup you may access the device
** either with a USB-to-UART cable as 


## Via built-in webserver

Is documented under [built-in webserver](firmware_webserver.html)

## Via USB-Stick

Download a firmware (Check whether there are newer files present). Depending on what you want to achieve you choose:

### Choose the desired firmware
1. **Debian**<br>
https://github.com/gnubee-git/gnubee-git.github.io/raw/master/debian/librecmc-ramips-mt7621-gb-pc1-squashfs-sysupgrade_2017-07-22.bin (around 17 MB)
1. **LEDE**<br>
https://github.com/gnubee-git/GnuBee_Docs/raw/master/GB-PC1/firmware/LEDE/GnuBee/GnuBee-lede-17.01-full-0915.bin (around 29MB)
1. **libreCMC**<br>
https://github.com/gnubee-git/GnuBee_Docs/raw/master/GB-PC1/firmware/libreCMC/GnuBee/GnuBee-librecmc-sysupgrade-full-0911.bin (around 10 MB)

### Copy firmware to USB-Stick (MS-DOS format)

Use a USB-stick with a MSDOS partition table and a vfat or fat partition. Copy the downloaded file and rename it to gnubee.bin. Unmount the USB-stick.

### Flash the firmware
Place your USB-stick into any of the 3 USB connectors. Reboot the GnuBee via a SW command or by pressing twice the red power on/off button.

While loading the new firmware the LEDs will give an indication or reading/writing.
Lower LED fast blink = read, slow blink = write, solid = done. (This may take several minutes.)
When the upper LED changes from off to on solid it's time to remove the USB Stick and reboot into the new firmware.

 
