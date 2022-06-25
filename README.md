# MSI-B460M-i5-10400-Hackintosh

My personal OpenCore hackintosh for MSI B460M i5-10400 UHD 630.

## Update Log

- OC version: 0.8.2
- Latest update: 2022-06-25
- Kexts and tools based on [HackinPlugins](https://github.com/bugprogrammer/HackinPlugins)@2022-06-25
- Support macOS Monterey 12.4


## Hardware

| #           | Type                    | Price        | Buy Where |
| ----------- | ----------------------- | ------------ | --------- |
| CPU         | i5-10400                | 套装         | JD        |
| Graphic     | UHD630 + HP GT630（2G） | 198          | XY        |
| Motherboard | MSI B460M               | 套装 1762.51 | JD        |
| Power       | 酷冷至尊 GX450          | 234.99       | JD        |
| Case        | 雷匠 静默者             | 51           | JD        |
| Cooling     | 九州风神 玄冰400        | 64           | JD        |
| Fan         | 先马 游戏风暴*2         | 11.79        | JD        |
| SSD         | 阿斯加特 AN2 500G       | 328.5        | JD        |
| HHD         | 500G                    | 拆机         |           |
| Memory      | 光威 悍将 2666 16*2     | 自有         | JD        |
| Display     | AOC 4K + KOIOS 4K       | 3012 + 980   | JD        |


## Issues

Test by yourself or you tell me.


## Config

```console
EFI/OC » tree . -L 2
.
├── ACPI
│   ├── SSDT-AWAC.aml
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
│   └── OpenShell.efi
└── config.plist
```


## Notes

- Change your own SMBIOS and determine the validity of it
- Enable NVIDIA GTX series(Kepler) graphic card support, you can check [here](https://heipg.cn/drivers/geforce-kepler-patcher-v3.html) and [here](https://github.com/chris1111/Geforce-Kepler-patcher)
- If you use the other network card and bluetooth model, you may need to load BlueToolFixup.kext
- In this version, USB ports need to be re-customized by yourself, you can check [here](https://apple.sqlsec.com/6-实用姿势/6-1.html) to re-customized it


## References

- [https://apple.sqlsec.com/](https://apple.sqlsec.com/)
- [https://dortania.github.io/OpenCore-Install-Guide/](https://dortania.github.io/OpenCore-Install-Guide/)
- [https://heipg.cn/tutorial/how-to-hackintosh.html](https://heipg.cn/tutorial/how-to-hackintosh.html)
- [https://heipg.cn/tutorial/b460m-install-big-sur.html](https://heipg.cn/tutorial/b460m-install-big-sur.html)
- [https://shuiyunxc.github.io/2020/04/23/xiaobai/index/](https://shuiyunxc.github.io/2020/04/23/xiaobai/index/) [以及对应的视频](https://space.bilibili.com/405490165?spm_id_from=333.788.b_765f7570696e666f.2)
