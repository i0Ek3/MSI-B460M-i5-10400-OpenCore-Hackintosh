# MSI-B460M-i5-10400-OpenCore-Hackintosh

> It will take a while to enter the installation interface, please be patient.

My personal OpenCore hackintosh for MSI B460M i5-10400 UHD 630, very streamlined.

## Update Log

- OC version: 0.8.5
- Latest update: 2022-09-18
- Kexts and tools based on [HackinPlugins](https://github.com/bugprogrammer/HackinPlugins)@2022-09-16
- Support macOS Monterey/Ventura(Beta7)
- Details
    - Regular version upgrade
    - Enable HDMI output
    - Replace the computer case and re-customize the interface
    - Enable SIP by default
    - English installation by default
    - Find yourself


## Hardware

- Motherboard: MSI B460M
- CPU: Intel i5-10400
- Graphic: Intel UHD630
- SSD
    - Asgard 500GB AN2: macOS Monterey
    - Asgard 500GB AN3: Windows 11
- HDD: Seagate 2T
- Memory: Gloway DDR4 2666Hz 16GB * 3
- WiFi+Bluetooth: Fenvi T919 BCM94360CD
- Display
    - AOC U27U2G6R4B 27-inch 4K
    - KOIOS K2721UD 27-inch 4K
- Cooling: DEEPCOOL 玄冰 400 V5
- Fan: SAMA 12cm * 1
- Power: CoolerMaster GX450
- Computer Case: JONSBO U3

## BIOS Setting

Only some core options are turned on or off here, others can be set according to personal preferences.

### Disable

- Fast Boot
- Secure Boot
- VT-d
- CSM
- SGX
- CFG

### Enable

- VT-x


## Notes

- **Backup your data first.**
- Change your own SMBIOS and determine the validity of it.
- More details of boot args please check [here](https://github.com/acidanthera/WhateverGreen#boot-arguments) and [here](https://www.mfpud.com/topics/8785/).
- To enable NVIDIA GTX series(Kepler) graphic card support, you can check [here](https://heipg.cn/drivers/geforce-kepler-patcher-v3.html) and [here](https://github.com/chris1111/Geforce-Kepler-patcher).
- If you use the different network card and bluetooth model with mine, you may need to load BlueToolFixup.kext, reference [here.](https://dortania.github.io/OpenCore-Install-Guide/extras/monterey.html#bluetooth)
- In this version, USB ports need to be re-customized by yourself, you can check [here](https://apple.sqlsec.com/6-实用姿势/6-1.html) to know how to re-customized it. Of course, if you have same case with mine(JONSBO U3), you can use it directly.
- In my config.plist, SIP is enabled by default, you can disable SIP in Recovery system by running command `csrutil disable ; csrutil disable authenticated-root` or enable SIP toggle button on the boot interface.
- Remember clean NVRAM cache before you use my EFI config.
- If you want to make your own OpenCore config.plist, please follows the steps [here.](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html)
- There may lots of issues, please be careful if you want to use my EFI config directly.

## Issues

Test by yourself or you tell me.


## References

- [https://apple.sqlsec.com/](https://apple.sqlsec.com/)
- [https://dortania.github.io/OpenCore-Install-Guide/](https://dortania.github.io/OpenCore-Install-Guide/)
- [https://heipg.cn/tutorial/how-to-hackintosh.html](https://heipg.cn/tutorial/how-to-hackintosh.html)
- [https://heipg.cn/tutorial/b460m-install-big-sur.html](https://heipg.cn/tutorial/b460m-install-big-sur.html)
- [https://shuiyunxc.github.io/2020/04/23/xiaobai/index/](https://shuiyunxc.github.io/2020/04/23/xiaobai/index/)
