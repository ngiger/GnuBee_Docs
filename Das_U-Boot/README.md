# GnuBee_Docs

## GnuBee Das U-Boot

The GnuBee Personal Cloud One uses the Das U-Boot -- the Universal Boot Loader.

## USB firmware update

One can easily update the firmware using the bootloader :

Place the new firmware on a USB stick (msdos format)

RENAME the firmware gnubee.bin

Then reboot the device ... the Boot Loader reads the file then updates the firmware.

While loading the new firmware the LEDs will give an indication of reading/writing.

Lower LED : 
fast blink = reading 
slow blink = write 
solid = done.

Upper LED : 
OFF during the update 
ON remove the USB Stick and reboot.


## TODO:
* Web Recovery 

