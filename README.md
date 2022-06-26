# MSI-B460M-i5-10400-Hackintosh

My personal OpenCore hackintosh for MSI B460M i5-10400 UHD 630.

> THIS IS A BETA VERSION, PLEASE BE KNOWN.

## Update Log

- OC version: 0.8.2
- Latest update: 2022-06-26
- Kexts and tools based on [HackinPlugins](https://github.com/bugprogrammer/HackinPlugins)@2022-06-25
- Support macOS Monterey 12.4


## Hardware

| #           | Type                      | Price        | Buy Where |
| ----------- | ------------------------- | ------------ | --------- |
| CPU         | i5-10400(UHD630)          | Suit 1762.51 | JD        |
| Graphic     | HP GT630（2G）            | 198          | XY        |
| Motherboard | MSI B460M                 | Suit 1762.51 | JD        |
| Power       | 酷冷至尊 GX450            | 234.99       | JD        |
| Case        | 雷匠 静默者               | 51           | JD        |
| Cooling     | 九州风神 玄冰400          | 64           | JD        |
| Fan         | 先马 游戏风暴*2           | 11.79        | JD        |
| SSD         | 阿斯加特 AN2 500G         | 328.5        | JD        |
| HHD         | 500G                      | N/A          | N/A       |
| Memory      | 光威 悍将 2666 16*2       | 299*2        | JD        |
| Display1    | AOC U27U2G6R4B 27-inch 4K | 3012         | JD        |
| Display2    | KOIOS K2721UD 27-inch 4K  | 980          | JD        |


## Issues

Test by yourself or you tell me.


## Config

```console
EFI/OC » tree . -L 2
.
├── ACPI
│   ├── SSDT-AWAC.aml
│   ├── SSDT-GPRW.aml
│   ├── SSDT-PLUG.aml
│   └── SSDT-USBX.aml
├── Drivers
│   ├── CrScreenshotDxe.efi
│   ├── OpenCanopy.efi
│   ├── OpenHfsPlus.efi
│   └── OpenRuntime.efi
├── Kexts
│   ├── AppleALC.kext
│   ├── Lilu.kext
│   ├── LucyRTL8125Ethernet.kext
│   ├── NVMeFix.kext
│   ├── SMCProcessor.kext
│   ├── SMCSuperIO.kext
│   ├── VirtualSMC.kext
│   └── WhateverGreen.kext
├── OpenCore.efi
├── Tools
│   ├── CleanNvram.efi
│   ├── CsrUtil.efi
│   ├── OpenControl.efi
│   ├── OpenShell.efi
│   └── ResetSystem.efi
└── config.plist
```


## Notes

- Change your own SMBIOS and determine the validity of it
- To enable NVIDIA GTX series(Kepler) graphic card support, you can check [here](https://heipg.cn/drivers/geforce-kepler-patcher-v3.html) and [here](https://github.com/chris1111/Geforce-Kepler-patcher)
- If you use the different network card and bluetooth model with mine, you may need to load BlueToolFixup.kext, reference [here](https://dortania.github.io/OpenCore-Install-Guide/extras/monterey.html#bluetooth)
- In this version, USB ports need to be re-customized by yourself, you can check [here](https://apple.sqlsec.com/6-实用姿势/6-1.html) to re-customized it
- In my config.plist, SIP is enabled by default, you can disable SIP in Recovery system by running command `csrutil disable ; csrutil disable authenticated-root`
- If you want to make your own OpenCore config.plist, please follows the steps [here](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html)
- There may lots of issues, please be careful if you want to use my EFI config


## References

- [https://apple.sqlsec.com/](https://apple.sqlsec.com/)
- [https://dortania.github.io/OpenCore-Install-Guide/](https://dortania.github.io/OpenCore-Install-Guide/)
- [https://heipg.cn/tutorial/how-to-hackintosh.html](https://heipg.cn/tutorial/how-to-hackintosh.html)
- [https://heipg.cn/tutorial/b460m-install-big-sur.html](https://heipg.cn/tutorial/b460m-install-big-sur.html)
- [https://shuiyunxc.github.io/2020/04/23/xiaobai/index/](https://shuiyunxc.github.io/2020/04/23/xiaobai/index/) [以及对应的视频](https://space.bilibili.com/405490165?spm_id_from=333.788.b_765f7570696e666f.2)
