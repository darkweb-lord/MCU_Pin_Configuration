# STM32 MPU Family Reference

## Complete Reference Guide: STMicroelectronics STM32 Arm Cortex-A / Cortex-M Microprocessor Portfolio

**Document Version:** 1.0  
**Last Updated:** September 2026  
**Scope:** STM32MP1 and STM32MP2 microprocessor families  
**Architecture:** Heterogeneous Arm Cortex-A + Cortex-M processing

> **Important:** STM32MP devices are **microprocessors (MPUs)**, not Cortex-M-only microcontrollers (MCUs). They combine application-class Cortex-A processors with real-time Cortex-M processors. ST separates the STM32 MPU portfolio from its STM32 Cortex-M MCU portfolio.

---

## 📋 Quick Navigation

| Family | Main Application Core | Real-Time Core | Maximum Application-Core Speed | Typical Position |
|---|---|---|---:|---|
| **STM32MP1** | Cortex-A7 | Cortex-M4 on selected lines | Up to 1 GHz | General-purpose embedded Linux / industrial MPU |
| **STM32MP2** | Cortex-A35 | Cortex-M33; Cortex-M0+ on MP25x | Up to 1.5 GHz | Secure, multimedia and edge-AI MPU |

---

# 🟦 STM32MP1 SERIES

## Overview

**Category:** General-purpose 32-bit MPU  
**Application Core:** Arm Cortex-A7  
**Real-Time Core:** Arm Cortex-M4 on selected MP15x devices  
**Application-Core Frequency:** Up to 1 GHz on MP13x; up to 800 MHz on MP15x  
**M4 Frequency:** Up to 209 MHz on MP15x  
**Operating Environment:** Embedded Linux, bare metal and RTOS combinations  
**Graphics:** 3D GPU on selected MP15x devices  
**Connectivity:** Ethernet, USB, CAN/FDCAN and extensive serial interfaces

ST describes STM32MP1 as a general-purpose microprocessor portfolio ranging from single Cortex-A7 devices to dual Cortex-A7 + Cortex-M4 configurations. The MP13x line focuses on entry-level Linux, bare-metal or RTOS-based systems, while the MP15x line adds Cortex-M4 real-time processing and richer peripherals on selected devices. citeturn0search0turn0search1

---

## STM32MP1 Product Lines

### STM32MP13x

The STM32MP13x line uses a **single Cortex-A7 application processor** and is intended for applications where Linux-class processing is required without the Cortex-M4 real-time core found on MP15x devices.

| Product | Application Core | Maximum Speed | Notable Capabilities |
|---|---|---:|---|
| **STM32MP131** | Cortex-A7 | Up to 1 GHz | Ethernet |
| **STM32MP133** | Cortex-A7 | Up to 1 GHz | CAN FD, dual Ethernet |
| **STM32MP135** | Cortex-A7 | Up to 1 GHz | Camera, dual Ethernet, LCD parallel interface |

ST's current MP1 portfolio identifies MP131, MP133 and MP135 in this line. citeturn0search0turn0search1

### STM32MP15x

The STM32MP15x line combines Cortex-A7 application processing with a Cortex-M4 real-time core.

| Product | Application Core | Real-Time Core | Maximum Speeds | Notable Capabilities |
|---|---|---|---|---|
| **STM32MP151** | Single Cortex-A7 | Cortex-M4 | A7 up to 800 MHz; M4 209 MHz | LCD-TFT, Ethernet |
| **STM32MP153** | Dual Cortex-A7 | Cortex-M4 | A7 up to 800 MHz; M4 209 MHz | CAN FD, Ethernet, LCD-TFT |
| **STM32MP157** | Dual Cortex-A7 | Cortex-M4 | A7 up to 800 MHz; M4 209 MHz | 3D GPU, DSI display, CAN FD, Ethernet |

ST lists MP151, MP153 and MP157 as the principal MP15x configurations. citeturn0search0

---

## STM32MP1 Architecture

```text
                    STM32MP1
                       │
             ┌─────────┴─────────┐
             │                   │
        Cortex-A7             Cortex-M4
      Application CPU        Real-Time CPU
             │                   │
        Embedded Linux       Bare Metal / RTOS
             │                   │
             └─────────┬─────────┘
                       │
             Shared STM32 Peripherals
                       │
       ┌───────────────┼────────────────┐
       │               │                │
    Ethernet          USB             CAN/FDCAN
       │               │                │
       └───────────────┼────────────────┘
                       │
              External DDR Memory
```

### Cortex-A7 Role

Typical responsibilities include:

- Embedded Linux
- High-level application processing
- Networking
- User interfaces
- File systems
- Application frameworks
- Multimedia applications

### Cortex-M4 Role

On MP15x devices, the Cortex-M4 can be used for:

- Real-time control
- Deterministic I/O processing
- Motor/control loops
- Peripheral handling
- Bare-metal firmware
- RTOS-based tasks
- Real-time co-processing

---

## STM32MP1 Key Features

- Single or dual Cortex-A7 configurations
- Cortex-M4 real-time processor on MP15x devices
- Linux-capable application processing
- Ethernet
- CAN / FDCAN on selected devices
- USB host/device/OTG capabilities
- LCD-TFT display interfaces
- MIPI-DSI on selected devices
- Camera interfaces on selected devices
- 3D GPU on STM32MP157
- External DDR memory controller
- Extensive UART, SPI and I2C connectivity
- STM32Cube ecosystem
- STM32CubeProgrammer support
- STM32CubeMX support
- Linux ecosystem and partner distributions

ST highlights an STM32 ecosystem that includes STM32Cube tools, STM32CubeProgrammer, STM32CubeMX and Linux support. citeturn0search0turn0search1

---

## STM32MP1 Typical Applications

- Industrial HMI
- Industrial gateways
- Factory automation
- Embedded Linux controllers
- Networking equipment
- Smart building systems
- Metering
- Consumer embedded systems
- Display controllers
- Camera-enabled systems
- Industrial communication gateways
- Real-time Linux + MCU co-processing systems

---

# 🟪 STM32MP2 SERIES

## Overview

**Category:** Second-generation STM32 MPU  
**Application Core:** Arm Cortex-A35  
**Real-Time Core:** Arm Cortex-M33  
**Additional Core:** Cortex-M0+ on STM32MP25x devices  
**Application-Core Frequency:** Up to 1.5 GHz  
**Cortex-M33 Frequency:** Up to 400 MHz  
**Cortex-M0+ Frequency:** Up to 200 MHz on STM32MP25x  
**Target:** Secure industrial, multimedia and edge-AI applications

ST describes STM32MP2 as a second-generation MPU platform using single or dual Cortex-A35 processors together with Cortex-M33 and, on MP25x devices, Cortex-M0+. The Cortex-M33 can operate at up to 400 MHz, while the Cortex-M0+ on MP25x devices can operate at up to 200 MHz. citeturn0search6turn0search4

---

## STM32MP2 Product Families

### STM32MP21x

Single Cortex-A35 + Cortex-M33 configuration.

| Product Family | Cortex-A35 | Cortex-M33 | Notable Capabilities |
|---|---:|---:|---|
| **STM32MP211** | Up to 1.5 GHz | Up to 300 MHz | Ethernet, security options |
| **STM32MP213** | Up to 1.5 GHz | Up to 300 MHz | Dual Ethernet, 2× FDCAN, CSI-2 on selected variants |
| **STM32MP215** | Up to 1.5 GHz | Up to 300 MHz | Dual Ethernet, 2× FDCAN, display, CSI-2 |

ST's current MP2 portfolio lists MP211, MP213 and MP215 configurations with Cortex-A35 up to 1.5 GHz and Cortex-M33 up to 300 MHz. citeturn0search1turn0search4

---

### STM32MP23x

Dual Cortex-A35 + Cortex-M33 configuration.

| Product Family | Cortex-A35 | Cortex-M33 | Notable Capabilities |
|---|---:|---:|---|
| **STM32MP231** | Up to 1.5 GHz | Up to 400 MHz | Ethernet, security variants |
| **STM32MP233** | Up to 1.5 GHz | Up to 400 MHz | Dual Ethernet, 2× FDCAN |
| **STM32MP235** | Up to 1.5 GHz | Up to 400 MHz | 3D GPU, H.264 decoding, AI/NN, LVDS/DSI |

ST lists MP231, MP233 and MP235 products in the MP23x group. citeturn0search4turn0search13

---

### STM32MP25x

The MP25x family adds a Cortex-M0+ processing domain alongside Cortex-A35 and Cortex-M33.

| Product Family | Application Core | Real-Time / Auxiliary Cores | Maximum Speeds | Notable Capabilities |
|---|---|---|---|---|
| **STM32MP251** | Cortex-A35 | Cortex-M33 + Cortex-M0+ | A35 1.5 GHz; M33 400 MHz; M0+ 200 MHz | Ethernet, CSI-2, security |
| **STM32MP255** | Dual Cortex-A35 | Cortex-M33 + Cortex-M0+ | A35 1.5 GHz; M33 400 MHz; M0+ 200 MHz | 3D GPU, H.264, AI/NN, LVDS/DSI |
| **STM32MP257** | Dual Cortex-A35 | Cortex-M33 + Cortex-M0+ | A35 1.5 GHz; M33 400 MHz; M0+ 200 MHz | 3× Ethernet, 3× FDCAN, GPU, AI/NN |

The current ST portfolio identifies the MP25x line as the STM32MP2 configuration that includes a Cortex-M0+ processor in addition to Cortex-A35 and Cortex-M33. citeturn0search4turn0search6

---

## STM32MP2 Architecture

```text
                         STM32MP2
                            │
             ┌──────────────┼──────────────┐
             │              │              │
        Cortex-A35      Cortex-M33     Cortex-M0+
        Application     Secure /       Low-power /
        Processing      Real-Time      Auxiliary
             │              │              │
        Linux / Apps     RTOS / FW     Peripheral/
        Multimedia       Security      SmartRun
             │              │              │
             └──────────────┼──────────────┘
                            │
                 High-Speed System Fabric
                            │
       ┌────────────────────┼────────────────────┐
       │                    │                    │
    Ethernet              USB                 FDCAN
       │                    │                    │
       ├────────────────────┼────────────────────┤
       │                    │                    │
     Camera             Display             AI / GPU
```

---

## Cortex-A35 Role

Typical responsibilities:

- Embedded Linux
- High-level application software
- Networking
- Graphical user interfaces
- Multimedia
- File systems
- Data processing
- Edge computing
- Application frameworks

---

## Cortex-M33 Role

The Cortex-M33 provides a real-time and security-oriented processing domain.

Typical responsibilities:

- Real-time control
- Secure boot / trusted-domain functions
- Critical peripheral control
- Deterministic firmware
- RTOS applications
- Hardware security functions
- Management of selected system resources

ST specifically describes the Cortex-M33 as capable of acting as a bootable trusted domain for securing the system and managing Cortex-A35 startup and resets. citeturn0search6

---

## Cortex-M0+ Role on STM32MP25x

On MP25x devices, the Cortex-M0+ provides an additional low-power processing domain.

ST states that the MP25x Cortex-M0+ can operate up to **200 MHz**, or slow to **16 MHz** for minimal-power operation, supporting SmartRun-domain operation while other cores are stopped. citeturn0search6

Typical uses include:

- Low-power peripheral processing
- Background operations
- Auxiliary control
- Power-efficient always-on functions
- Peripheral activity while higher-performance cores are stopped

---

# ⚙️ STM32MP1 vs STM32MP2

| Feature | STM32MP1 | STM32MP2 |
|---|---|---|
| MPU generation | 1st generation | 2nd generation |
| Application CPU | Cortex-A7 | Cortex-A35 |
| Application CPU width | 32-bit | 64-bit |
| Application CPU speed | Up to 1 GHz | Up to 1.5 GHz |
| Real-time CPU | Cortex-M4 on MP15x | Cortex-M33 |
| Additional MCU core | — | Cortex-M0+ on MP25x |
| Linux | Yes | Yes |
| GPU | 3D GPU on selected MP15x | 3D GPU on selected MP23x/MP25x |
| AI acceleration | Limited / application-dependent | AI/NN acceleration on selected devices |
| Ethernet | Up to dual Ethernet on selected devices | Up to 3 Ethernet interfaces on selected devices |
| CAN | CAN/FDCAN on selected devices | FDCAN on selected devices |
| Camera | Selected devices | Advanced camera interfaces on selected devices |
| Display | LCD-TFT; MIPI-DSI on selected devices | LCD-TFT, MIPI-DSI/LVDS on selected devices |
| Primary positioning | General-purpose embedded Linux | Secure industrial, multimedia and edge AI |

ST's current portfolio distinguishes MP1 as the earlier Cortex-A7 generation and MP2 as the newer Cortex-A35 generation with substantially expanded multimedia, security and edge-AI capabilities. citeturn0search1turn0search12

---

# 🧠 MCU vs MPU — Important Difference

| Characteristic | STM32 Cortex-M MCU | STM32 MPU |
|---|---|---|
| Typical core | Cortex-M | Cortex-A + Cortex-M |
| Main software | Bare metal / RTOS | Linux + RTOS / bare metal |
| External DDR | Usually not required | Commonly required |
| MMU | Generally absent | Cortex-A includes MMU |
| Boot complexity | Lower | Higher |
| Power management | MCU-oriented | Multi-domain system management |
| GUI capability | MCU graphics peripherals | High-end display/GPU options |
| Application processing | Real-time embedded | Linux-class application processing |
| Typical use | Control, sensing, motor, communication | HMI, gateway, Linux, multimedia, edge computing |

ST explicitly distinguishes its STM32 Cortex-M MCU portfolio from its STM32 MPU portfolio, with the MPU range using heterogeneous Cortex-A and Cortex-M architectures. citeturn0search1turn0search2

---

# 🛠️ STM32 MPU Development Ecosystem

## Hardware

- STM32MP1 Evaluation Boards
- STM32MP1 Discovery Kits
- STM32MP2 Evaluation Boards
- STM32MP2 Discovery Kits
- System-on-Modules from ST-authorized partners

## Software

- STM32CubeMX
- STM32CubeProgrammer
- STM32CubeIDE
- STM32Cube firmware components
- Linux
- Open-source Linux ecosystem
- RTOS / bare-metal firmware for Cortex-M cores
- GCC-based development tools

ST highlights the common STM32 ecosystem, including STM32CubeMX, STM32CubeProgrammer, GCC-based development tools and Linux support. citeturn0search0turn0search1

---

# 🎯 Application Selection Guide

## Industrial Automation

**STM32MP1**
- Industrial HMI
- Gateways
- Linux control systems
- Display controllers
- Industrial networking

**STM32MP2**
- Advanced industrial HMI
- Edge computing
- Machine vision
- AI-enabled automation
- High-performance gateways

## Camera / Vision

**STM32MP1**
- Camera-enabled embedded systems on selected MP13x/MP15x devices

**STM32MP2**
- MIPI CSI-2
- Advanced image-processing applications
- Machine vision
- Edge AI on selected devices

## HMI / Display

**STM32MP1**
- LCD-TFT
- MIPI-DSI on selected devices
- 3D GPU on STM32MP157

**STM32MP2**
- LCD-TFT
- MIPI-DSI
- LVDS
- 3D GPU on selected devices
- Video processing on selected devices

---

# 🔐 Security

STM32MP devices provide security features across the MPU ecosystem.

### STM32MP1

Selected devices provide security functions aimed at IoT, industrial and payment applications. ST also lists certified-security options on the STM32MP13 product line. citeturn0search0

### STM32MP2

Security capabilities include:

- Secure boot
- Cryptographic acceleration
- Trusted execution/isolation features
- TrustZone on Cortex-A and Cortex-M domains
- Protected system resources
- DRAM encryption/decryption on selected devices
- PKA on selected devices

ST identifies security capabilities such as secure boot, cryptography and DRAM encryption/decryption on selected MP2 products. citeturn0search4turn0search7

---

# 📊 Family Summary

| Family | Cortex-A | Cortex-M | Key Strength |
|---|---|---|---|
| **STM32MP1** | Cortex-A7 | Cortex-M4 on MP15x | Embedded Linux + real-time control |
| **STM32MP2** | Cortex-A35 | Cortex-M33; M0+ on MP25x | Secure high-performance edge computing |

---

# 📚 Official STMicroelectronics References

- [STM32 Arm Cortex MPUs](https://www.st.com/en/microcontrollers-microprocessors/stm32-arm-cortex-mpus.html)
- [STM32MP1 Series](https://www.st.com/en/microcontrollers-microprocessors/stm32mp1-series)
- [STM32MP2 Series](https://www.st.com/en/microcontrollers-microprocessors/stm32mp2-series)
- [STM32MP1 Documentation](https://www.st.com/en/microcontrollers-microprocessors/stm32mp1-series/documentation.html)
- [STM32MP2 Documentation](https://www.st.com/en/microcontrollers-microprocessors/stm32mp2-series/documentation.html)

---

# 📌 Notes & Disclaimers

1. Specifications shown are **family/portfolio-level values** and can vary by exact part number.
2. Not every STM32MP device contains every peripheral or accelerator listed.
3. External DDR and board-level power/clock design requirements depend on the exact MPU.
4. Linux support, boot architecture and Cortex-M firmware architecture should be evaluated together during system design.
5. Always consult the exact ST datasheet, reference manual, errata and hardware design guidelines before production design.
6. STM32MP1 and STM32MP2 are **MPUs**, not Cortex-M-only MCUs.
7. The Cortex-M cores inside an MPU do not make the entire device a Cortex-M MCU.

---

**Document Version:** 1.0  
**Status:** STM32 MPU Family Reference — verified against current STMicroelectronics portfolio

For the latest information and detailed datasheets, visit [STMicroelectronics Official Website](https://www.st.com/stm32).
