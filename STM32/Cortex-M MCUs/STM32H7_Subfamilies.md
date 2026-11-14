# STM32H7 Device Family: Subfamilies and Part Details

*Generated: 14 Nov 2026*

## Part 1: Subfamily List

| Group | Subfamily | CPU | Max MHz | Flash | RAM |
|---|---|---|---|---|---|
| Dual-core | STM32H747/757 | Cortex-M7 + M4 | 480 + 240 | up to 2 MB | 1 MB |
| Dual-core | STM32H745/755 | Cortex-M7 + M4 | 480 + 240 | up to 2 MB | 1 MB |
| Single-core | STM32H743/753 | Cortex-M7 | 480 | up to 2 MB | 1 MB |
| Single-core | STM32H742 | Cortex-M7 | 480 | up to 2 MB | ~692 KB |
| Single-core | STM32H7A3/7B3 | Cortex-M7 | 280 | up to 2 MB | ~1.4 MB |
| Single-core | STM32H725/735 | Cortex-M7 | 550 | up to 1 MB | 564 KB |
| Single-core | STM32H723/733 | Cortex-M7 | 550 | up to 1 MB | 564 KB |
| Value line | STM32H750 | Cortex-M7 | 480 | 128 KB | 1 MB |
| Value line | STM32H7B0 | Cortex-M7 | 280 | 128 KB | ~1.4 MB |
| Value line | STM32H730 | Cortex-M7 | 550 | 128 KB | 564 KB |
| H7RS (newer) | STM32H7R3/7S3 | Cortex-M7 | 600 | 64 KB user | 620 KB |
| H7RS (newer) | STM32H7R7/7S7 | Cortex-M7 | 600 | 64 KB user | see datasheet |

**Notes**

- ST states the series has 12 product lines, 130+ part numbers, and pin counts from 64 to 240, in QFN, WLCSP, LQFP and BGA packages.
- Sources: ST product pages, ST product overview, ST migration note AN5996 (H7R/S).

### What "Group" Means

"Group" is ST's way of sorting the STM32H7 subfamilies into product line groups, based on how many CPU cores they have and how they are positioned (performance vs. cost). ST's own overview slides split the series into dual-core lines, single-core lines, value lines, and the newer bootflash lines.

| Group | Meaning | Typical use |
|---|---|---|
| **Dual-core** | Two CPUs on one chip: a Cortex-M7 (up to 480 MHz) plus a Cortex-M4 (up to 240 MHz). Tasks can be split between the cores. Includes H745/755 and H747/757. | Complex apps that separate real-time control from UI or communications, such as industrial HMI and connected systems. |
| **Single-core** | One Cortex-M7 core. Larger flash (up to 2 MB) and RAM, with the widest peripheral and package choice. Includes H743/753, H742, H7A3/7B3, H723/733 and H725/735. | General high-performance designs: motor control, audio, graphics, communications. |
| **Value line** | Single-core parts cut down in cost, with only 128 KB of internal flash. They rely on external memory (such as QSPI flash) for the main program. Includes H750, H7B0 and H730. | Cost-sensitive designs that already use external flash. |
| **H7RS (bootflash)** | Newer lines (H7R3/7S3, H7R7/7S7) with small on-chip flash (64 KB user) used mainly for secure boot, with the application in external memory. | Designs needing secure firmware updates and external memory. |

**How this relates to your part:** the STM32H7B3RI is in the **Single-core** group (H7A3/7B3 line). It has 2 MB of internal flash, unlike the **Value line** H7B0, which has only 128 KB.

## Part 2: Part Number Details

Status key:

- **VERIFIED**: seen in a source during this session.
- **DS-CHECK**: from ST naming convention and general knowledge; confirm in the datasheet before ordering.

### H7B3 (280 MHz)

| Part no. | Pins | Flash | Package | Status |
|---|---|---|---|---|
| STM32H7B3RIT6 | 64 | 2 MB | LQFP64 10x10 | VERIFIED |
| STM32H7B3VIT6Q | 100 | 2 MB | LQFP100 14x14 | VERIFIED |
| STM32H7B3VIH6Q | 100 | 2 MB | TFBGA100 8x8 | VERIFIED |
| STM32H7B3ZIT6Q | 144 | 2 MB | LQFP144 20x20 | VERIFIED |
| STM32H7B3IIT6 | 176 | 2 MB | LQFP176 24x24 | VERIFIED |
| STM32H7B3IIT6Q | 176 | 2 MB | LQFP176 24x24 | VERIFIED |
| STM32H7B3LIH6Q | 225 | 2 MB | TFBGA225 | VERIFIED |

### H7B0 value line (280 MHz)

| Part no. | Pins | Flash | Package | Status |
|---|---|---|---|---|
| STM32H7B0RBT6 | 64 | 128 KB | LQFP64 | VERIFIED |
| STM32H7B0VBT6 | 100 | 128 KB | LQFP100 | VERIFIED |
| STM32H7B0IBK6Q | 176+25 | 128 KB | UFBGA176+25 | VERIFIED |

### H723 / H733 / H730 (550 MHz)

| Part no. | Pins | Flash | Package | Status |
|---|---|---|---|---|
| STM32H733VGT6 | 100 | 1 MB | LQFP100 | VERIFIED |
| STM32H733VGH6 | 100 | 1 MB | TFBGA100 | VERIFIED |
| STM32H733ZGT6 | 144 | 1 MB | LQFP144 | VERIFIED |
| STM32H733ZGI6 | 144 | 1 MB | UFBGA144 | VERIFIED |
| STM32H723VGT6 | 100 | 1 MB | LQFP100 | VERIFIED |
| STM32H723VET6 | 100 | 512 KB | LQFP100 | VERIFIED |
| STM32H723ZGT6 | 144 | 1 MB | LQFP144 | VERIFIED |
| STM32H723ZET6 | 144 | 512 KB | LQFP144 | VERIFIED |
| STM32H730VBT6 | 100 | 128 KB | LQFP100 | VERIFIED |
| STM32H730ZBT6 | 144 | 128 KB | LQFP144 | VERIFIED |
| STM32H730 (Q variant) | 68 | 128 KB | VFQFPN68 | VERIFIED (family has a 68-pin QFN) |

### H725 / H735 (550 MHz)

| Part no. | Pins | Flash | Package | Status |
|---|---|---|---|---|
| STM32H725VET6 | 100 | 512 KB | LQFP100 | VERIFIED (part exists) |
| STM32H725/735 xG | 100 to 176 | 1 MB | LQFP / TFBGA / UFBGA | DS-CHECK |

### H7A3 (280 MHz)

| Part no. | Pins | Flash | Package | Status |
|---|---|---|---|---|
| STM32H7A3RIT6 | 64 | 2 MB | LQFP64 | DS-CHECK |
| STM32H7A3VIT6 | 100 | 2 MB | LQFP100 | DS-CHECK |
| STM32H7A3ZIT6 | 144 | 2 MB | LQFP144 | DS-CHECK |
| STM32H7A3IIT6 | 176 | 2 MB | LQFP176 | DS-CHECK |

### H743 / H753 (480 MHz)

| Part no. | Pins | Flash | Package | Status |
|---|---|---|---|---|
| STM32H743VIT6 | 100 | 2 MB | LQFP100 | DS-CHECK |
| STM32H743ZIT6 | 144 | 2 MB | LQFP144 | DS-CHECK |
| STM32H743IIT6 | 176 | 2 MB | LQFP176 | DS-CHECK |
| STM32H743BIT6 | 208 | 2 MB | LQFP208 | DS-CHECK |
| STM32H743XIH6 | 240+25 | 2 MB | TFBGA240+25 | DS-CHECK |

### H742 (480 MHz)

| Part no. | Pins | Flash | Package | Status |
|---|---|---|---|---|
| STM32H742VIT6 | 100 | 2 MB | LQFP100 | DS-CHECK |
| STM32H742ZIT6 | 144 | 2 MB | LQFP144 | DS-CHECK |
| STM32H742IIT6 | 176 | 2 MB | LQFP176 | DS-CHECK |

### H750 value line (480 MHz)

| Part no. | Pins | Flash | Package | Status |
|---|---|---|---|---|
| STM32H750VBT6 | 100 | 128 KB | LQFP100 | DS-CHECK |
| STM32H750ZBT6 | 144 | 128 KB | LQFP144 | DS-CHECK |
| STM32H750IBT6 | 176 | 128 KB | LQFP176 | DS-CHECK |
| STM32H750XBH6 | 240+25 | 128 KB | TFBGA240+25 | DS-CHECK |

### H745 / H755 dual-core

| Part no. | Pins | Flash | Package | Status |
|---|---|---|---|---|
| STM32H745ZIT6 | 144 | 2 MB | LQFP144 | DS-CHECK |
| STM32H745IIT6 | 176 | 2 MB | LQFP176 | DS-CHECK |
| STM32H745BIT6 | 208 | 2 MB | LQFP208 | DS-CHECK |
| STM32H745XIH6 | 240+25 | 2 MB | TFBGA240+25 | DS-CHECK |

### H747 / H757 dual-core

| Part no. | Pins | Flash | Package | Status |
|---|---|---|---|---|
| STM32H747ZIT6 | 144 | 2 MB | LQFP144 | DS-CHECK |
| STM32H747IIT6 | 176 | 2 MB | LQFP176 | DS-CHECK |
| STM32H747BIT6 | 208 | 2 MB | LQFP208 | DS-CHECK |
| STM32H747XIH6 | 240+25 | 2 MB | TFBGA240+25 | DS-CHECK |

### H7R3 / H7S3 / H7R7 / H7S7

| Part no. | Pins | Flash | Package | Status |
|---|---|---|---|---|
| Several parts | not collected | 64 KB | BGA / QFN options | DS-CHECK |

## Suffix Guide (ST convention)

| Code | Meaning |
|---|---|
| R / V / Z / I | 64 / 100 / 144 / 176 pins |
| B / X / L | 208 pins / 240+25 balls / 225 balls |
| Flash B / E / G / I | 128 KB / 512 KB / 1 MB / 2 MB |
| T / H / K | LQFP / TFBGA / UFBGA |
| 6 | -40 to 85 °C |
| Q suffix | SMPS-capable (varies by line) |
