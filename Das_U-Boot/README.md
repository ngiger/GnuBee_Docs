# GnuBee_Docs

## GnuBee Das U-Boot

The GnuBee Personal Cloud One uses the Das U-Boot -- the Universal Boot Loader.

## USB firmware update

One can easily update the firmware using the bootloader :
Place the new firmware on a USB stick (msdos format)
RENAME the firmware gnubee.bin
Then reboot the device ... the boot-loader reads the file then updates the firmware.
While loading the new firmware the LEDs will give an indication or reading/writing.
Lower LED fast blink = read, slow blink = write, solid = done.
When the upper LED changes from off to on solid it's time to remove the USB Stick and reboot into the new firmware.


## TODO:
* Web Recovery 

