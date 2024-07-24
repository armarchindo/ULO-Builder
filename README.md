# ULO Builder for OpenWRT
 ULO (Universal Linux OpenWrt) Builder 
 adalah sebuah software pembuat firmware OpenWRT untuk berbagai device dan SOC (AMLogic, ALLWinner, Rockchip)
 penggunaan sangat mudah dan lebih manusiawi, cocok untuk semua kalangan.
 
https://github.com/armarchindo/ULO-Builder/assets/7347993/1aeef098-b9ce-49df-92db-585a0eaa3e94

## Supported Devices
| Amlogic | Alwinner | Rockchip |
| -------- | ------- | ------- | 
| S905X | H616 (Orange Pi Zero 3) | RK3566 (Orange Pi 3B) |
| S905X2 | H6 (Orange Pi 3 LTS) | RK3588S (Orange Pi 5) |
| S905X3 | - | - |
| S905X4 | - | - |
   
## Requirements
 - `lolcat,pigz` and default packages from Linux
   
## Usage
 - Clone This repository `git clone --depth=1 --brach=main https://github.com/armarchindo/ULO-Builder.git`
 - Directory Kernel: `core/kernel/`
 - Directory ROOTFS:  `rootfs`
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
