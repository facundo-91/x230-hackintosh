# Thinkpad X230 Hackintosh

## Logs:
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
| WiFi                | TL-WN725N Nano USB Adapter      |
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
- [banhbaoxamlan](https://github.com/banhbaoxamlan): Using his repository to make mine.
- [n4ru](https://github.com/n4ru/): For his software-based "jailbreak" to softmod custom bios images.
- [acidanthera](https://github.com/acidanthera): For his Kexts: AppleALC, Lilu, Whatevergreen, etc.
- [Clover](https://github.com/CloverHackyColor/CloverBootloader): Bootloader for macOS.
