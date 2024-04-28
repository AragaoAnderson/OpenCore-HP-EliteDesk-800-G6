# OpenCore for HP EliteDesk 800 G6 Mini PC

1. OpenCore Version: 1.0.0
2. All used Kernel Extensions are updated until 04-26-24
3. Latest macOS Sonoma version Supported
4. Generate a valid SMBios for your installation. The files includes a Generic one
   
## Configuration

- CPU：Intel Core i5 10500
- Graphics: Intel UHD Graphics 630
- RAM：16GB 2667MHz DDR4
- HardDisk：SSD NVMe KINGSTON SNVS500G 500GB
- Wi-Fi：FENVI Broadcom 4360 Wireless (For built-in Intel use OpenIntelWireless)

## What's Working

1. All DP/HDMI Ports with Audio Output
2. All USB and USB-C 3.x Ports
3. Built-in Audio and Speaker with Boot Chime support
4. Dualboot with Windows 11 Pro using Custom UpdateSMBIOSMode to avoid issues with Windows Activation
5. AirPlay using FeatureUnlock.kext when using Mac mini SMBios

## What's not Working

1. DRM of Apple TV and Apple Music like all Hackintosh's using Intel iGPU

## Installation

Please refer to the detailed installation tutorial [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/).

## UEFI BIOS Setup

| Variable                                                              | Default         | Desired         |
| --------------------------------------------------------------------- | --------------- | --------------- |
| Security > Secure Boot Configuration > Secure Boot                    | Enabled         | Disabled        |
| Advanced > Boot Options > Fast Boot                                   | Enabled         | Disabled        |
| Advanced > Built-In Device Options > Wake on WLAN                     | Enabled         | Disabled        |
| Advanced > Power Management Options > PCI Express Power Management    | Enabled         | Disabled        |

## Special Thanks to

[RehabMan](https://github.com/RehabMan) and [Acidanthera](https://github.com/acidanthera).
