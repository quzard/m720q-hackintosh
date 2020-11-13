# OpenCore EFI for Lenovo M720Q (macOS 10.15.7)
## Just for backup

## Specification
| **Component** | **Model** |
| ------------- | --------- |
| CPU | Intel i5-9500T |
| Motherboard | Intel B360 |
| RAM | 8GB DDR4-2133 |
| Audio Chipset | ALC235 |
| GPU | Intel® UHD Graphics 630 (DP, HDMI, VGA) |
| OS Disk (NVMe) | LITEON T10 NVMe 256G |
| WIFI | DW 1820A |

**macOS version**: 10.15.7
**OpenCore version**: 0.6.2

## How to use

1. Make your USB installer with [**this guide**](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)
2. Clone the repository and paste "BOOT" and "OC" directories into your's pendrive "EFI" folder
3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select **Generate SMBIOS**, as the model select **Macmini8,1**.
4. Open config.plist with [**ProperTree**](https://github.com/corpnewt/ProperTree) and go to PlatformInfo > Generic. Set MLB (Board Serial), SystemSerialNumber (Serial) and SystemUUID (SmUUID) to generated values. Change ROM to your network card's MAC address without the `:` character. [**How to get MAC Address?**](https://www.wikihow.com/Find-the-MAC-Address-of-Your-Computer)
5. Boot it!

## All work

- CPU
- Dual monitors (Displayport & HDMI & VGA)
- Audio (ALC235)
- Ethernet
- USB
- Wifi
- Airdrop, Hand-off, Sidecar
- App store, iCloud, iMessage, iTunes, FaceTime, etc
- Sleep, Wakeup, Shutdown, Restart

# Acknowledgements

[m720q-OpenCore-Catalina](https://github.com/tobagin/m720q-OpenCore-Catalina)

[M720q-Hackintosh-EFI](https://github.com/leonardoi7/M720q-Hackintosh-EFI)