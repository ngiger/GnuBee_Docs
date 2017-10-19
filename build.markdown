---
layout: default
title: Firmware Build
---

## Sources

https://github.com/gnubee-git/gnubee-openwrt (branch master, with official kernel from Soc vendor, Debian-compatible scripts) 

<!-- Being veri https://github.com/gnubee-git/GnuBee-lede (branch lede-17-01 have Debian-compatible scripts) -->

https://gogs.librecmc.org/ldpinney/GnuBee-libreCMC



## References

https://wiki.openwrt.org/doc/howto/buildroot.exigence

https://wiki.openwrt.org/doc/howto/build

## Commands after source retrieval

######## GIT #########

git pull && ./scripts/feeds update -a && ./scripts/feeds install -a

######## BUILD ########

make menuconfig

make -j1 V=s download

ionice -c 3 nice -n 19 make -j1 V=s \| tee build.log

######## CLEAN ########

make dirclean

make target/linux/clean
