# ASUS-Vivobook-X512JA

This repo includes an OpenCore EFI for the ASUS Vivobook X512JA.

Testing on:

Model | ASUS Vivobook X512JA
------------- | ---------------
CPU | Intel Core i3-1005G1
iGPU | Intel UHD Graphics G1
RAM | 8 GB DDR4
WiFi | Intel Wireless-AC 9260
macOS | Sonoma 14.3

## What works?

- Audio
- Battery readout
- Boot
- Brightness Control
- GPU acceleration
- Keyboard + Trackpad
- Power Management
- SD card reader
- Sleep
- USB
- Speaker

## What doesn't work?

- HDMI Output
    -Deleted apple driver for Icelake (never fix)
- Intel Optane H10 (stock SSD)
    - Either change your SSD or use an external drive
        - If you are using an external drive, add `nvme=-1` to your boot-args to avoid kernel panics
-Webcam USB2.0 UVC WebCam
    -Some vivobook series Firmware Webcam not supported 

## BIOS settings

- Secure Boot: Disabled
- TBD

## Credits

* [acidanthera](https://github.com/acidanthera) (for OpenCore and the kexts)
* [dortania](https://dortania.github.io/OpenCore-Install-Guide/) (for their awesome guide)
* [jwise](https://github.com/jwise) (for HoRNDIS)
* [VoodooI2C](https://github.com/VoodooI2C) (for VoodooI2C)
* [OpenIntelWireless](https://github.com/OpenIntelWireless/itlwm) (for Intel WiFi)
* our tester
