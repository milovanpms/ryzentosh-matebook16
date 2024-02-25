# Milo's Ryzentosh (Matebook 16)

[![MacOS version](https://img.shields.io/badge/Ventura-13.6.4-informational.svg)](https://www.apple.com/macos) [![MacOS version](https://img.shields.io/badge/Sonoma-14.4%20beta4-informational.svg)](https://www.apple.com/macos) \
[![OpenCore version](https://img.shields.io/badge/OpenCore-0.9.8-informational.svg)](https://github.com/acidanthera/OpenCorePkg)\
[![GitHub](https://img.shields.io/github/license/milovanpms/ryzentosh-matebook16?style=flat-square)](https://github.com/milovanpms/ryzentosh-matebook16/blob/master/LICENSE)

<a href="https://postimg.cc/mcWSTcTC" target="_blank"><img src="https://i.postimg.cc/mcWSTcTC/Screenshot_2023-05-19_at_8.26.25_AM.png" alt="Screenshot_2023-05-19_at_8.26.25_AM"/></a> <a href="https://postimg.cc/VJPsThGw" target="_blank"><img src="https://i.postimg.cc/VJPsThGw/temp-Image26-C8-TR.jpg" alt="temp-Image26-C8-TR"/></a> <a href="https://postimg.cc/nMsHLxNZ" target="_blank"><img src="https://i.postimg.cc/nMsHLxNZ/temp-Image45-Yy-Gt.jpg" alt="temp-Image45-Yy-Gt"/></a> <a href="https://postimg.cc/hXFvqfjN" target="_blank"><img src="https://i.postimg.cc/hXFvqfjN/temp-Imagel-KRSx-Y.avif" alt="temp-Imagel-KRSx-Y"/></a>

## Disclaimer
Please don't yell at me if your laptop starts to smell like burnt sausage. Don't forget to generate your personalised SMBIOS and setting it in your config.plist, otherwise it will not work.
Also, the only component I changed is the WiFi/Bluetooth card, there was a non-compatible Realtek card in the laptop, I changed it for an Intel AX210NGW.

## Specification

| Component        | Model                                              |
| ---------------- | ---------------------------------------------------|
| Laptop           | Huawei Matebook 16 2020 (CREM-WFD9)                |
| CPU              | AMD Ryzen 7 5800H                                  |
| WiFi/Bluetooth   | Intel AX210NGW (swapped, it was a Realtek card)    |
| SSD              | WDC PC SN730 SDBPNTY-512G                          |
| RAM              | 2x Soldered 8GB Micron 4ATF1G64HZ-3G2E1 (3200 MHz) |
| iGPU             | AMD Radeon Vega 7 Graphics (with 512MB VRAM)       |


## Working

* iCloud 
* Sound, HDMI and Jack (AppleALC not compatible with any preset, so I used VoodooHDA)
* Graphics Acceleration (with NootedRed)
* WiFi
* iServices

## Not Working

* Bluetooth (I don't have much time to look for a solution, don't hesitate to commit)
* AirDrop (because of Bluetooth)
* Screen Mirroring
* TouchID


## Patches, Drivers & Kexts

* [AppleALC](https://github.com/acidanthera/AppleALC)
* [AppleMCEReporterDisabler](https://github.com/acidanthera/bugtracker/files/3703498/AppleMCEReporterDisabler.kext.zip)
* [Kernel Patches](https://github.com/AMD-OSX/AMD_Vanilla)
* [Lilu](https://github.com/acidanthera/Lilu)
* [OpenCore](https://github.com/acidanthera/OpenCorePkg)
* [RestrictEvents](https://github.com/acidanthera/RestrictEvents)
* [VirtualSMC](https://github.com/acidanthera/VirtualSMC)
* [NootedRed](https://github.com/acidanthera/WhateverGreen)

## Bootloader

I use OpenCore to multiboot Manjaro, Windows(10&11) and MacOS(Catalina, BigSur, Monterey & Ventura)

[![04000725.png](https://i.postimg.cc/ZqdPpQj7/04000725.png)](https://postimg.cc/069JqcTD)

## Credits and links

* [OpenCore install guide](https://dortania.github.io/OpenCore-Install-Guide)
* [Hackintool](https://www.hackintosh-forum.de/forum/thread/38316-hackintool-ehemals-intel-fb-patcher)
* [OpenCore-Legacy-Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher)
* [OpenCore-Legacy-Patcher guide](https://dortania.github.io/OpenCore-Legacy-Patcher)
