---
title: "Reboot-to-Windows: Simple service to reboot Linux to ANY system"
draft: false
date: 2023-10-15
description: "Many computing computers I use have multi-systems (Windows+Ubuntu). I use GRUB to select the system, and the default one is Linux. I need to be able to reboot from Linux to any other system when the computer is unattended."
language: 'Shell'
platform: 'Linux (GRUB)'
link: 'https://github.com/InkosiZhong/reboot-to-windows'
tags:
  - Developments
---

Computer with multi-systems, *e.g.*, `Ubuntu+Windows`, often use GRUB to manage booting.
In a remote enviroment, neither `ssh` nor `GUI remote controller` control the computer until the system is started. 
This project can realize system switching of unattended computers by manipulating GRUB menu.

``` sh
> r2w
### GRUB boot menu ###
1: Ubuntu
2: Advanced options for Ubuntu
3: Windows Boot Manager (on /dev/nvme0n1p1)
4: UEFI Firmware Settings

Select the index of the target system:
> 3
Selected system: Windows Boot Manager (on /dev/nvme0n1p1)

> r2w 3
### GRUB boot menu ###
1: Ubuntu
2: Advanced options for Ubuntu
3: Windows Boot Manager (on /dev/nvme0n1p1)
4: UEFI Firmware Settings
Selected system: Windows Boot Manager (on /dev/nvme0n1p1)
```