# Cyberoam CR50iNG → Sophos Firewall Home Edition Conversion Guide

This repository documents converting a Cyberoam CR50iNG appliance into a working Sophos Firewall Home Edition system.

## Hardware Specs

CPU: Intel Celeron E3400 @ 2.60GHz
RAM: Upgraded from 2GB to 4GB (2 × 2GB DDR3 matched bus speed)
Storage: Internal HDD
Console: Serial (RJ45)
BIOS: Phoenix AwardBIOS

## Steps Performed

1. Increased RAM from 2GB to 4GB using 2 × 2GB DDR3 modules (matching bus speed).
2. Cleaned the internal hard disk and temporarily removed CompactFlash storage.
3. Changed boot priority in BIOS and enabled USB boot.
4. Connected via serial console (PuTTY) using 38400 baud rate and booted installer from USB.
5. Followed Sophos installation instructions.
6. Accessed firewall UI via https://172.16.16.16:4444 and completed setup wizard.

## Port Mapping (Observed)

| Physical Port | Sophos Interface |
|--------------|-----------------|
| Port H | Port 2 |
| Port G | Port 1 |
| Port F | Port 8 |
| Port E | Port 7 |
| Port D | Port 6 |
| Port C | Port 5 |
| Port B | Port 4 |
| Port A | Port 3 |

Always verify mapping manually before assigning WAN/LAN.

## Recommended Sophos Version

Sophos Firewall Home Edition 19.5.x

## Author

Nazmul Haque
