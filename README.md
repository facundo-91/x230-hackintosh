# Thinkpad X230 Hackintosh

## Logs:
### 22 June 2020 Update:
- Updated config.plist and removed PNLF.aml for backlight control (Method 1 from WhateverGreen documentation).
- Added IO80211Family.kext for Atheros AR5B95.
- WhateverGreen.kext to 1.4.0
### 13 June 2020 Update:
- Clover: r5119
- Kexts and Drivers updated

## Hardware
| Specifications      | Detail                          |
|:-------------------:|:-------------------------------:|
| CPU                 | Intel Core i5 3320M             |
| RAM                 | 8GB Kingston 1600MHz DDR3L      |
| Storage             | 500GB SSD Western Digital Blue  |
| Bluetooth           | Broadcom BCM20702A0             |
| WiFi                | Atheros AR5B95      						|
| BIOS                | 2.73                            |
| EC									| 1.14                            |

## What's Working
- Power Management
- Intel HD 4000 QE/CI
- Sleep/Wake
- Webcam
- Ethernet
- Battery Status
- Brightness Control
- Keyboard/Trackpad/Trackpoint
- Sound/Headphone Detection
- USB Ports
- Bluetooth

## Issues
#### WiFi:
Because Intel WiFi cards doesn't work out of the box, you have three options:
- Use a whitelisted card/macOS supported Atheros AR5B95 (Lenovo P/N° 20002357) + IO80211Family.kext for 10.14 or newer.
- Flash the BIOS to remove the whitelist (using a hardware programmer or use software based [1vyrain](https://github.com/n4ru/1vyrain)) and use a Broadcom WLAN card.
- Use an USB adapter.
#### Card Reader:
Got kext to recognize it although the system freezes when you put any SD Card inside.
#### Fingerprint Reader:
My unit doesn't have it.
#### VGA Port:
Mac's doesn't have this kind of ports so you will have to use the MiniDP port with an HDMI/VGA adapter.

## Credits
- [Apple](https://www.apple.com/) for MacOS
- [banhbaoxamlan](https://github.com/banhbaoxamlan) for his repository to make mine.
- [n4ru](https://github.com/n4ru/) for [1vyrain](https://github.com/n4ru/1vyrain) to softmod custom bios images.
- [acidanthera](https://github.com/acidanthera), [vit9696](https://github.com/vit9696) for his Kexts: AppleALC, Lilu, Whatevergreen, etc.
- [Clover](https://github.com/CloverHackyColor/CloverBootloader) for Bootloader for macOS.
