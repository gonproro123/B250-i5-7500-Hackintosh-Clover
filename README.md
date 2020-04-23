# B250 i5-7500 Hackintosh Clover
## Introduction

## This repository contains the following folders:
- `EFI`: put this in your EFI partition in EFI folder, including BOOT, CLOVER & APPLE sub-folders
- `L/E` kexts': kexts that should be installed in `L/E`

## Tested on `Catalina, 10.15.4` with the following hardware:
- Intel i5-7500
- Mainboard: MSI B250 Mortar
- GPU: NVIDIA 1050ti 
- 1920x1080 (FHD HDMI) and 1024*768 (DP)
- DDR4 2400 16GB (8Gb x 2)
- Intel 660p !? (OEM version)
- Audio : ALC892

## It's a 95% working hackintosh, including:
- Apfs disk partitions: ApfsDriverLoader-64 efi
- Audio on speakers: AppleALC kext
- Graphical acceleration (QE/CI): WhatEverGreen kext
- Trim enabled
- (for MSI mainboard)OsxAptioFix2Drv-free2000.efi
# Setup
## BIOS Settings
- The BIOS must be properly configured before installing MacOS.
- Save & Exit → Restore Defaults : Yes
- Advanced \ Integrated Peripherals → Network Stack : [Disabled]
- Advanced \Integrated Peripherals  → Intel Serial IO : [Disabled]
- Advanced \ USB Configuration → XHCI Hand-off : [Enabled]
- Advanced \ USB Configuration → Legacy USB Support : [Auto]
- Advanced \ Windows OS Configuration → MSI Fast Boot : [Disabled]
- Advanced \ Windows OS Configuration → Fast Boot : [Disabled]
- Overclocking  → Extreme Memory Profile(X.M.P) : [Enabled]
- Overclocking \ CPU Features → Intel Virtualization Tech : [Enabled]
- Overclocking \ CPU Features → Intel VT-D Tech : [Disabled]
- Boot → Boot mode select : [LEGACY+UEFI]

### Now you can go through the install.

## What's next?
- To finish the setup, you need to:
+ Install the latest Clover_EFI_bootloader.
+ Copy `EFI folder from USB` flash drive to `local drive EFI partition` (like you did for the USB drive). It will make the local drive bootable (so you can get rid of the USB drive now)
+ Coppy kexts in `L/E_Kexts` into `L/E`

## You're almost done! Reboot and enjoy macOS on your Imac 18.2


# Big thanks to 

- Rehabman.
- hackintosher.com
- hackintosh.vn



