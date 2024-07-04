# ULO Builder for OpenWRT
 ULO OpenWRT Builder
 
https://github.com/armarchindo/ULO-Builder/assets/7347993/1aeef098-b9ce-49df-92db-585a0eaa3e94

## Features
 - Support for Amlogic S905x Devices
 - Support for Amlogic S905x2 Devices
 - Support for Amlogic S905x3 Devices
 - Support for Amlogic S905x4 Devices
 - Support for Allwinner H618 Devices
 - Support for Allwinner H6 Devices
 - Support for Rockchip RK3566 Devices
   
## Requirements
 - `lolcat` and default packages from Linux
   
## Usage
 - Clone This repository `git clone https://github.com/armarchindo/ULO-Builder.git`
 - Copy Kernel to folder `core/kernel/kernelversion`
 - Copy ROOTFS files to folder `openwrt or debian`
 - run ULO script with superuser `sudo ./ulo`
 - select used SOC/Processor
   <p align="left">
     <img src="https://raw.githubusercontent.com/armarchindo/ULO-Builder/main/img/1.png" width="75%" />
   </p>
 - select used Kernel Version for use
   <p align="left">
     <img src="https://raw.githubusercontent.com/armarchindo/ULO-Builder/main/img/2.png" width="75%" />
   </p>
 - setting size of ROOTFS Partition
   <p align="left">
     <img src="https://raw.githubusercontent.com/armarchindo/ULO-Builder/main/img/3.png" width="75%" />
   </p>
 - Building OpenWRT/Debian Firmware
   <p align="left">
     <img src="https://raw.githubusercontent.com/armarchindo/ULO-Builder/main/img/4.png" width="75%" />
   </p>
 - Done, OpenWRT/Debian image at folder `out`

 ### ULO script information
```bash
Usage:
  ulo [options]

Options:
    -h, --help
    -c, --clean
    -k                  set the kernel (-k 5.9.16)
    -m                  set the device (-m s905x2)
    -s, --size=SIZE     set size (-s 768)
```
## About
> Script ULO ini dibuat karena mbah sepuh lagi gabut.
