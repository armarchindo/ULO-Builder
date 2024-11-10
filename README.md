# ULO Builder for OpenWRT
 ULO (Universal Linux OpenWrt) Builder 
 adalah sebuah software pembuat firmware OpenWRT untuk berbagai jenis device dan SOC (AMLogic, ALLWinner, Rockchip)
 penggunaan sangat mudah dan manusiawi, cocok untuk semua kalangan.
 
https://github.com/user-attachments/assets/f9b25d81-a364-4bc9-8b84-173cfa0e099e

## Supported Devices
| Amlogic | Allwinner | Rockchip |
| -------- | ------- | ------- |
| **S905**  | **A64** (`bananapi-m64`, `nanopi-a64`) | **RK3328** (`-`) |
| **S905W** | **H5** (`Orange Pi Zero Plus 2`, `Orange Pi Zero Plus`, `Orange Pi Prime`, `Orange Pi PC2`) | **RK3399** (`-`) |
| **S905D** | **H6** (`Orange Pi 1 Plus`, `Orange Pi Lite 2`, `Orange Pi 3 LTS`, `Orange Pi 3`, `Tanix TX6`) | **RK3528** (`-`) |
| **S905L** | **H313** (`x96q-lpddr3`) | **RK3566** (`Orange Pi 3B`) |
| **S905X** | **H616** (`Orange Pi Zero 2`, `X96-Mate`) | **RK3568** (`-`) |
| **S912** | **H618** (`Orange Pi Zero 3`, `Orange Pi Zero 2W`) | **RK3588S** (`Orange Pi 5`) | 
| **a311d** | - | **RK3588** (`Orange Pi 5 Plus`) |
| **s922x** | - | - |
| **S905Y4** | - | - |
| **S905X4** | - | - |
## Requirements
 - `lolcat, pigz, aria2` and default packages from Linux
   
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
 
 OLD KERNEL CHECK HERE
 ```bash
 https://github.com/armarchindo/kernel/releases
 ```
### ULO script information
 - ULO Repository Template : [ULO Repository](https://github.com/armarchindo/ULO-repository)
 - How to change `ULO Repository` at `ULO Builder`
   1. Fork [ULO Repository](https://github.com/armarchindo/ULO-repository) on your github
   2. You can edit a `firmware`, `rootfs`, `kernel` files at your `ULO Repository`
   3. Edit your ULO Script at lines `25`<br>
   Change default ULO Repository to your URL Repository, example...
   ```bash
     # DEFAULT REPOSITORY
     # Kernel & Firmware Repository
     repos="https://github.com/armarchindo/ULO-repository"
   ``` 
   to
   ```bash
     # YOUR CUSTOM REPOSITORY
     # Kernel & Firmware Repository
     repos="https://github.com/xxx/ULO-repository"
   ```
 - ULO Command list :
```bash
Usage:
  ulo [options]

Options:
    -h, --help      : Show this Text
    -c, --clean     : Cleaning old cache
    -u, --update    : Update Kernel, ROOTFS, and Firmware files from ULO-Repository
                      (Will Destroy your old Kernel, ROOTFS, and Firmware files!!!)
    -k              : set the kernel       (-k 5.9.16)
    -m              : set the device       (-m s905x2)
    -r              : set the rootfs files (-r ImmortalWrt-21.02.7-DBAI-armvirt-rootfs.tar.gz)
    -s, --size=SIZE : set size             (-s 768)
```
## About
> Script ULO ini dibuat karena mbah sepuh lagi gabut.
