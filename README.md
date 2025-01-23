# Lenovo Legion 5 15ARH05A Ryzentosh

This repository contains the necessary files and instructions to install macOS 15 Sequoia on a Lenovo Legion 5 15ARH05A using OpenCore.

## Hardware Specifications

- **Model:** Lenovo Legion 5 15ARH05A
- **CPU:** AMD Ryzen 5 5600H
- **GPU:** NVIDIA Geforce RTX 2060 (we will disable it)
- **RAM:** 16GB
- **Storage:** Western Digital 1TB NVME SSD
- **Wi-Fi & Bluetooth:** Intel AX200
- **Integrated GPU:** AMD Radeon RX Vega 6

## Requirements
- A BaseSystem.dmg for macos Sequoia

## Preparation
- Download the EFI
- Use OCAT to disable NootedRed and enable WhateverGreen in kernel tab
## Installation

1. **BIOS Configuration:**
   - Update to the latest BIOS version.
   - Set BIOS settings to default.
   - Configure the following settings:
     - Disable Secure Boot.

2. **Boot from USB:**
   - Insert the USB installer into the laptop.
   - Press F12 to boot to boot mewnu

3. **OpenCore Bootloader:**
   - Use OpenCore to boot into the macOS installer.
   - Follow the on-screen instructions to install macOS.

4. **Post-Installation:**
   - Copy the EFI folder from the USB drive to the macOS drive.
   - Disable WhateverGreen.kext and enable NootedRed.kext again

## Troubleshooting

- **Common Issues:**
- Sound from speakers not working with AppleALC, only works with external sound card
- ***Some apps are not working on AMD CPU, use [AMDhelper](https://github.com/alvindimas05/AMDHelper) to patch these

## Credits

- [OpenCore Team](https://dortania.github.io/OpenCore-Install-Guide/)
- [Hackintosh Community](https://www.tonymacx86.com/)
- [OpCoreSimplify team](https://github.com/lzhoang2801/OpCore-Simplify/)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.