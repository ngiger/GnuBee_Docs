---
title: Introducing GnuBee Personal Cloud
permalink: index.html
---

**GnuBee PC-1 is shipping since mid september 2017**


introduction {#introduction}
----------

The GnuBee Personal Cloud 1 (GB-PC1) is a network-attached storage (NAS) device specifically engineered to run free, libre, open source software (FLOSS). The GB-PC1 has all the functionality of any commercial, proprietary NAS, but at a much lower cost and with the transparency, reliability, and accessibility advantages that come with using FLOSS.

Why {#why}
----------------------------

Free as in Freedom

We designed the GnuBee Personal Cloud 1 with the Free Software Foundation’s Respects Your Freedom (RYF) certification in mind and have already initiated the application process with FSF.

The GnuBee Personal Cloud 1 is 100% free of binary blobs. Check out this campaign update to see some of the backstory of how this is possible.
Libre Software

The GnuBee Personal Cloud 1 can run several popular FLOSS suites for managing routers, NAS devices, or just general computing. These are some of the main suites the GB-PC1 can run:

## Debian

Yep, the GB-PC1 can run Debian.

## openmediavault

The openmediavault project is a Debian-based network-attached storage solution designed for home and small office user who lack deep technical experience or knowledge of setting up and and administering an NAS.

## libreCMC

Billed as “the libre embedded GNU/Linux distro,” libreCMC is a fork of OpenWrt that uses only libre components. Recently, our pull request for GB-PC1 compatibility was merged into the staging branch.
## LEDE

The Linux Embedded Development Environment (LEDE) project is a reboot of the OpenWrt community. We’ve created a GB-PC1 fork of the LEDE project and plan on submitting a patch back to the main project once production of the GB-PC1 is underway. (It is unlikely the LEDE developers would accept a patch for a device not yet in production.)

# FLOSS Devices at Reasonable Prices

GnuBee started with a simple idea: instead of hacking commodity hardware, let’s build the toys we want to play with from scratch . We want to show the world what devices running free software can do. The Personal Cloud 1 is our first product, though we have others in the works. If the GB-PC1 is successful, there will be plenty of others to follow!

How do we keep the cost of our devices down? Because we have both Chinese (Xiaoping) and US (Larry) roots, we have some major advantages over other teams. We don’t need to rent expensive living and work space in China (we stay with family!), and we don’t need to hire translators and other go-betweens. We can work directly with vendors and manufacturers. Because we are committed to working only with FLOSS projects, our software development costs are also reduced and distributed.

What is GnuBee {#what}
--------------

## Features & Specifications

    Processor:
        MediaTek MT7621A
        dual core, multi thread (Linux kernel sees four cores)
        880 MHz, overclockable to 1.2 GHz)
    Memory:
        512 MB DDR3 RAM (maximum amount for the MediaTek chip)
        soldered to main board
    Storage:
        microSD card slot (tested up to 64 GB cards so far)
        6 x 2.5” drives (HDD, SSD, or mix and match; drives not included)
        Recommended RAID levels are 0 and 1 under LVM and MD, and Linux MD RAID 10
    Connectivity:
        2 x Gigabit Ethernet
        1 x USB 3.0 port
        2 x USB 2.0 ports
        Serial port (3-pin J1 connector or 3.5 mm audio-type jack)
    Power:
        12 VDC @ 3 A maximum
        5.5 mm x 2.1 mm, center-positive barrel jack
    Dimensions:
        Bounding box: 8.5” (L) x 2.75” (W) x 5.5” (H)
        Weight: ~210 g (without drives)
    Enclosure:
        2 x anodized aluminum side plates
        4 x threaded brackets and screws
        24 x drive screws (four per drive)


Versions {#versions}
---------

-   Personal Cloud 1 (GnuBee PC-1) started shipping in September 2017

-   Future Versions

If the GnuBee Personal Cloud 1 successfully reaches its funding goal and goes to production, we plan to make other variants (e.g., a version compatible with 3.5” drives) and other products (e.g., a wireless router). However, first things first - if you love FLOSS and hardware designed to run it, please support this campaign so we can continue this work!


License and honour {#notices}
------------------------------

Gnubee is a corporation working in Shenzhen, China & Tulsa, OK

* L. D. Pinney Founder and CTO
* Xiaoping Pinney Chairman Ping
* Douglas Gazineu Software Developer
