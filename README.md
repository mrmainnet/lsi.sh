# Install MegaCLI on CentOS 6.x, 7.x (.rpm)
```bash
# cd /usr/local/src
# wget https://docs.broadcom.com/docs-and-downloads/raid-controllers/raid-controllers-common-files/8-07-14_MegaCLI.zip
# unzip 8-07-14_MegaCLI.zip
# rpm -Uvh Linux/MegaCli-8.07.14-1.noarch.rpm
# /opt/MegaRAID/MegaCli/MegaCli64 -h
```

# Install MegaCLI on Debian, Ubuntu, Proxmox (.deb)
```bash
# cd /usr/local/src
# wget https://docs.broadcom.com/docs-and-downloads/raid-controllers/raid-controllers-common-files/8-07-14_MegaCLI.zip
# unzip 8-07-14_MegaCLI.zip
# alien Linux/MegaCli-8.07.14-1.noarch.rpm
# dpkg -imegacli_8.07.14-1_all.deb
# /opt/MegaRAID/MegaCli/MegaCli64 -h
```
# lsi.sh

This is a public repository for the lovely [wrapper script](https://calomel.org/megacli_lsi_commands.html) created by [Calomel.org](https://calomel.org/) for the LSI hardware RAID command line tool MegaCLI, [provided](https://calomel.org/calomel_at.html) Creative Commons Attribution-ShareAlike 4.0 International [license](http://creativecommons.org/licenses/by-sa/4.0/).

Their original description was simply:

```
Calomel.org 
    https://calomel.org/megacli_lsi_commands.html
    LSI MegaRaid CLI 
    lsi.sh @ Version 0.05

description: MegaCLI script to configure and monitor LSI raid cards.
```

Building on the shoulder of giants, I have added a little
"autoconfiguration", pathing for the default Ubuntu package, and a
couple small additions to their script to make dealing with an LSI
RAID system a little easier.

I'm hoping by putting this out there to encourage further development and extensions to try and bring `MegaCLI` under control.

# Environment

I'm working under an CentOS environment and I'm have been using this script for a year.

# Improvement
Send alert via Telegram

# More information 
An additional shout out to the useful RAID wiki on kernel.org for [their information](https://raid.wiki.kernel.org/index.php/Hardware_Raid_Setup_using_MegaCli) on MegaCli.
