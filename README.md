# IdeaPad 3 15ALC6 Opencore

Hackintosh EFI for Lenovo IdeaPad 3 15ALC6 using OpenCore bootloader.

![Hackintosh Screenshot](images/screenshot.png)

## macOS Details

| Category                                               | Version                |
| :----------------------------------------------------- | :--------------------- |
| [OpenCore](https://github.com/acidanthera/OpenCorePkg) | 1.0.5                  |
| macOS support                                          | macOS 10.5 to macOS 26 |

## Hardware Specifications

| Category         | Part                               | Status |
| :--------------- | :--------------------------------- | :----: |
| Model            | Lenovo IdeaPad 3 15ALC6 82KU01ATPH |   ✅   |
| CPU              | Ryzen 7 5700U                      |   ✅   |
| GPU              | AMD Radeon Graphics                |   ✅   |
| RAM              | 20GB (4GB soldered + 16GB SODIMM)  |   ✅   |
| Drive            | 512GB SSD M.2 2242 PCIe NVMe       |   ✅   |
| Audio            | Realtek ALC257                     |   ✅   |
| WiFi + Bluetooth | Qualcomm Atheros QCA6174           |   ❌   |
| Touchpad         | MSFT0001:00 06CB:CE2D              |   ✅   |

## Notes

- It is prefered to use macOS versions 15 and below for stability.
- Add `alcid=101` to `boot-args` for functional audio input and output.
- Use `MacBookPro16,3` (macOS 15 and below) or `MacBookPro16,2` (macOS 26 and below) [SMBIOS](https://github.com/corpnewt/GenSMBIOS).
- Speakers and headphone jack are broken on macOS 26, only HDMI audio is working.
- This EFI comes with `HoRNDIS.kext` to support USB Tethering.
- The built-in networking card is unsupported by MacOS.
- You may want to change your networking card or buy a USB WiFi adapter supported by [chris1111's driver](https://github.com/chris1111/Wireless-USB-OC-Big-Sur-Adapter).
- Set graphics memory to `2GB` through BIOS to avoid stutters.
