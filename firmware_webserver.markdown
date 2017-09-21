---
layout: default
title: Install firmware via webserver
---


### Ensure that your network is correctly configured

The built-in webserver listens by default on the address 192.168.10.1.

Connect the **black** ethernet RJ-45 to your network.

Open a terminal/console application and enter `ping -c1 192.168.1.1`. If you get an answer like

```bash
PING 192.168.1.1 (192.168.1.1) 56(84) bytes of data.`
64 bytes from 192.168.1.1: icmp_seq=1 ttl=64 time=0.066 ms
1 packets transmitted, 1 received, 0% packet loss, time 0ms
rtt min/avg/max/mdev = 0.066/0.066/0.066/0.000 ms
```

everyhing is okay and you open the address http://192.168.10.1 in your browser and continue with [flash the firmware](#flash_iamge).
Else you must

#### Configure your ethernt to listen on 192.168.10.2

This is done by adding a secondary interface to your primary network interface. Assuming you interface is called eth0 just call the following commands

```bash
sudo ifconfig | grep 192.168.10.
http://192.168.10.1
sudo ifconfig eth0:1 192.168.10.2 up
ping -c1  192.168.10.1
```

### Flashing the image via the browser  <a name="flash_iamge"></a>

Set the root password

<img src="images/libre_cmc_rootpw.png" width="600">

Allow SSH acces (if desired)

<img src="images/libre_cmc_dropbear.png" width="600">

Save the root password and SSH configuration by pressing **SAVE**

<img src="images/libre_cmc_save.png" width="600">

Select on the left menu **Backup / Flash Firmware**

<img src="images/libre_cmc_flash_1.png" width="600">

Select the downloaded firmware image from your PC
<img src="images/libre_cmc_flash_2.png" width="600">

Check the MD5SUM with the one given on github. If it matches press **PROCEED**

<img src="images/libre_cmc_flash_3.png" width="600">

Flashing will take several minutes

<img src="images/libre_cmc_flash_4.png" width="600">

If you have a USB-2-UART cable you can check the boot process by listening on the serial console as explained under [USB_to_UART](/USB_to_UART/README.html)
