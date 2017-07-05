# GnuBee_Docs

## GnuBee USB to UART

Most embedded System-on-chips come with an UART or TTL integrated into the System-on-chip to allow debugging, firmware replacement or serial connection.

The GnuBee Personal Cloud routes the UART connection to a 3.5mm (1/8") Audio Jack for convenient use.

The GnuBee USB to UART uses a Winchiphead CH340G USB to serial chip from Nanjing QinHeng Electronics Co.,Ltd. to convert the UART signal to USB.

The Linux kernel identifies this chipset as the "QinHeng Electronics HL-340 USB-Serial adapter"

Users of other Operating Systems can find drivers in the drivers directory.

## UART and TFTP

Common methods to change firmware in case of any problems.

I use [GNU Screen]https://www.gnu.org/software/screen/ AND [tftpd-hpa]https://packages.debian.org/buster/tftpd-hpa

screen /dev/ttyUSB0 57600

Windows users can download an install [PuTTY](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html) AND [TFTP32](http://tftpd32.jounin.net))

 Baud Rate: 57600 / Data Bits: 8 / Parity Control: NO / Stop Bits: 1 / Handshake: NO
