# ULO Builder for OpenWRT
 ULO (Universal Linux OpenWrt) Builder 
 adalah sebuah software pembuat firmware OpenWRT untuk berbagai jenis device dan SOC (AMLogic, ALLWinner, Rockchip)
 penggunaan sangat mudah dan manusiawi, cocok untuk semua kalangan.
 
https://github.com/user-attachments/assets/8a8802e7-96b2-4566-85cc-aad165e4f606

## Supported Devices
| Amlogic | Allwinner | Rockchip |
| -------- | ------- | ------- | 
| S905X | H6 (Orange Pi One Plus) | RK3566 (Orange Pi 3B) |
| S905X2 | H6 (Orange Pi 3 LTS) | RK3588S (Orange Pi 5) |
| S905X3 | H616 (Orange Pi Zero 2) | RK3588 (Orange Pi 5 Plus) |
| S905X4 | H618 (Orange Pi Zero 3) | - |
   
## Requirements
 - `lolcat,pigz` and default packages from Linux
   
## Usage
 - clone this repository `git clone --depth=1 --branch=main https://github.com/armarchindo/ULO-Builder.git`
 - directory Kernel: `core/kernel/`
 - directory ROOTFS:  `rootfs`
 - run ULO script with superuser `sudo ./ulo`
 - select SOC/Device
   <p align="left">
     <img src="https://raw.githubusercontent.com/armarchindo/ULO-Builder/main/img/1.png" width="75%" />
   </p>
 - select rootfs
   <p align="left">
     <img src="https://raw.githubusercontent.com/armarchindo/ULO-Builder/main/img/2.png" width="75%" />
   </p>
 - select kernel version
   <p align="left">
     <img src="https://raw.githubusercontent.com/armarchindo/ULO-Builder/main/img/3.png" width="75%" />
   </p>
 - setting size of ROOTFS Partition
   <p align="left">
     <img src="https://raw.githubusercontent.com/armarchindo/ULO-Builder/main/img/4.png" width="75%" />
   </p>
   building OpenWRT firmware
   <p align="left">
     <img src="https://raw.githubusercontent.com/armarchindo/ULO-Builder/main/img/5.png" width="75%" />
   </p>
 - done, the OpenWRT image is located in the `out` folder 

 ### ULO script information
```bash
Usage:
  ulo [options]

Options:
    -h, --help
    -c, --clean
    -k                  set the kernel (-k 6.6.6)
    -m                  set the device (-m s905x2)
    -s, --size=SIZE     set size (-s 768)
```
## About
> Script ULO ini dibuat karena mbah sepuh lagi gabut.
