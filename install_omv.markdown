---
layout: default
title: Install OpenMediaVault
---

## OpenMediaVault

The OpenMediaVault installation is documented [here](install_omv.html) as several points have to be considered.
You should be familiar with Debian or be familiar using linux system commands on the command line.


### download and install the firmware supporting Debian

Refer to [Debian Installation](install_debian.html) for the firmware supporting Debian download and installation procedure.

### Install OpenMediaVault

You can install OpenMediaVault with the following commands. Please keep in mind that kernel modules installation is mandatory, and as such is included on this script too:

    wget https://raw.githubusercontent.com/gnubee-git/gnubee-git.github.io/master/debian/omv-jessie-install
    chmod +x omv-jessie-install
    ./omv-jessie-install

