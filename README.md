**** BEWARE ***** - This version of ARCH ARM Allstar gives corrupted sound when used with chan_usbradio on a Raspberry PI

It is work in progress and includes YO3IIU's chan_alsaradio in an attempt to get better sound on the PI 
(It is work in progress….)
Update....23/5/2013 Using an IMIC2 USB soudcard with its built in 8KHz rate sampling, its work fine with clean audio when used on chan_alsaradio for Allstar

Allstar is an Amateur Radio repeater system based on an older version of Asterisk.
This repo contains the dev code for allstar including the mods for Arch Linux such as;
1. Zaptel ZTDummy driver changes ( made by me)
2. chan_usbradio changes to support Arch Linux ( thanks to KD0EAV)
3. Minor changes in Makefile etc...

Its not complete, you may need to symlink the ar binary etc.....
Hopefully we will make a Live CD of this for Arch Linux.
These files will only be usefull to those who compile their own versions of Allstar.
It does not use the ACID install method...

All credit should go to the Allstar creators at https://allstarlink.org/

Regards, Anthony VK2ACP

PS. You may need to do the following to add dependicies to compile... e.g

pacman -S base-devel binutils lrzip autoconf alsa-oss libusb-compat libnewt linux-headers alsa-lib libxml2
