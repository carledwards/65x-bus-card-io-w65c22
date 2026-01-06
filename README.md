# 65x Bus VIA I/O Card (W65C22)

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

A VIA (Versatile Interface Adapter) I/O card for the 65x Bus system.

## Overview

The VIA I/O card provides general-purpose parallel I/O using the WDC 65C22 Versatile Interface Adapter. It offers two 8-bit bidirectional ports, timers, and handshaking capabilities for interfacing with external hardware. The card includes a small prototyping area for adding driver circuits or port expanders.

### Features

- WDC W65C22 VIA (DIP-40)
- Two 8-bit bidirectional I/O ports (Port A and Port B)
- Two 16-bit timers
- Shift register for serial I/O
- Jumper-selectable I/O slot address
- 2×20 IDC headers for port access
- Small prototyping area
- Optional DiagModule connector
- Standard 100mm Eurocard depth

## Specifications

| Parameter | Value |
|-----------|-------|
| Board Format | Eurocard 3U, 160mm × 100mm |
| VIA Chip | WDC W65C22S |
| Default Address | $8000–$80FF (Slot 0) |
| I/O Headers | 2× 20-pin IDC (0.1" pitch) |
| Power | +5V from backplane, < 50 mA |

## Address Selection

Default slot is 0 ($8000). Change via jumpers J0–J3:

| Slot | Address | J3 | J2 | J1 | J0 |
|------|---------|----|----|----|----|
| 0 | $8000 | 0 | 0 | 0 | 0 |
| 1 | $8100 | 0 | 0 | 0 | 1 |
| 2 | $8200 | 0 | 0 | 1 | 0 |
| ... | ... | ... | ... | ... | ... |

## Hardware

KiCad project files are located in the `/hardware/` directory.

### Status

🚧 **In Development**

## Related

- [65x Bus Specification](https://github.com/carledwards/65x-bus-spec) — Full bus specification and documentation

## License

This work is licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/).

You are free to use, modify, and manufacture this design for personal, non-commercial purposes with attribution. Commercial use requires permission from the author.

