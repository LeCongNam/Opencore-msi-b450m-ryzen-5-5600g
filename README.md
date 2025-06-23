# OpenCore EFI for MSI B450M PRO-M2 MAX II

## Overview

This is an open-source EFI folder for running macOS on the MSI B450M PRO-M2 MAX II motherboard using the latest version of OpenCore. The configuration is tailored for AMD Ryzen systems and aims for maximum compatibility and stability.

## Features

- **Motherboard:** MSI B450M PRO-M2 MAX II
- **Bootloader:** OpenCore (latest version)
- **macOS Version:** macOS Ventura 13 (currently running)
- **Status:** Fully working except for Apple Services (iMessage, FaceTime, etc.)
- **AMD Power Management:** Not yet implemented

## What Works

- Booting macOS
- Audio, Ethernet, USB, and most hardware components
- Sleep/Wake
- Basic display output

## What Doesn't Work

- Apple Services (iMessage, FaceTime, etc.)
- Native AMD power management (chưa thể add quản lí năng lượng AMD)
- GPU hardware acceleration (unsupported GPU)

## Folder Structure

- `BOOT/` — Contains OpenCore bootloader files
- `OC/` — Main OpenCore configuration and resources
  - `ACPI/` — Custom SSDTs for hardware compatibility
  - `Drivers/` — OpenCore drivers
  - `Kexts/` — Kernel extensions for macOS support
  - `Tools/` — OpenCore tools
  - `config.plist` — Main OpenCore configuration file

## How to Use

1. Copy the contents of this EFI folder to the EFI partition of your USB or system drive.
2. Update `config.plist` as needed for your hardware (serials, SMBIOS, etc.).
3. Boot from the USB or system drive using OpenCore.

## Notes

- Make sure to generate unique SMBIOS information for your system.
- This EFI is provided as-is. Test thoroughly before using on your main system.
- Contributions and improvements are welcome!

## Credits

- OpenCore team and the Hackintosh community
- Developers of all included kexts and tools

---

_Last updated: June 23, 2025_
