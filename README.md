# VC220-G3u Revenge & Recovery

Collection of rare firmware binaries for the TP-Link VC220-G3u (MediaTek/TrendChip chipset). Since the vendor does not provide public downloads for ISP-locked devices, this repo serves as a lifeboat for bricked modems.

## 📦 Binary Manifest

| Version | Hardware | Build Date | Type | Filename |
| :--- | :--- | :--- | :--- | :--- |
| **1.1.0** | v2 | 2023-12-16 | Stock/Boot | `VC220-G3u_TRv2_1.1.0...bin` |
| **1.0.0** | v2 | 2022-08-29 | Stock/Boot | `VC220-G3uv2_1.0.0...bin` |

## 🔧 Technical Notes

* **Architecture:** MIPS (TrendChip/MediaTek EN75xx)
* **Flash Layout:** Dual Image (OS1/OS2)
* **Format:** These `.bin` files are standard update packages containing Kernel + RootFS (SquashFS) + Bootloader.
* **Recovery Method:** Can be flashed via Web UI (if accessible), TFTP, or raw flash writing via UART/XMODEM (requires splitting Kernel/RootFS).

## 💀 Recovery / Unbricking
If you are stuck at the Bootloader (`CCCCC` or `bldr>`), you can use these files to restore the partitions.
* **Kernel Offset:** `0x1E0000` (Typical)
* **RootFS Offset:** `0x3E0000` (Typical)

*Happy Hacking!*
