---
layout: default
title: Internals of the GnuBee PC 1 
---
This page lists the internals of the GnuBee PC 1. 
<img width="128" src='GB-PC1/Assembly/7.jpg' align='right'>

Component| Comment
------------ | -------------
Processor | MediaTek MT7621A<br>dual core, multi thread (Linux kernel sees four cores)<br>880 MHz, overclockable to 1.2 GHz)
Memory | 512 MB DDR3 RAM (maximum amount for the MediaTek chip)<br>soldered to main board
Flash ROM | 32 MB SPI contains U-Boot bootloader and<br>LEDE firwmare (Factory default)<br>resettable to factory defaults
Storage  | microSD card slot (tested up to 64 GB cards so far)<br>6 x 2.5” drives (HDD, SSD, or mix and match; drives not included)<br>Recommended RAID levels are 0 and 1 under LVM and MD, and Linux MD RAID 10
Connectivity | 2 x Gigabit Ethernet<br>1 x USB 3.0 port<br>2 x USB 2.0 ports<br>Serial port (3-pin J1 connector or 3.5 mm audio-type jack)
RTC | ???
Fan | No
Power | 12 VDC @ 3 A maximum<br>5.5 mm x 2.1 mm, center-positive barrel jack
Dimensions | Bounding box: 8.5” (L) x 2.75” (W) x 5.5” (H)<br>Weight: ~210 g (without drives)
Enclosure | 2 x anodized aluminum side plates<br>4 x threaded brackets and screws<br>24 x drive screws (four per drive)
Boot loader | U-Boot
Software |  Debian<br>openmediavault<br>LEDE<br>libreCMC
Sources & Documentation|documentation and schematics available as PDFs under CC-BY-SA 4.0<br>all firmware and code FLOSS

