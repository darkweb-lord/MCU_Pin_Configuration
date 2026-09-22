# STM32 Cortex-M MCU Family Reference
## Complete Reference Guide: STMicroelectronics 32-bit Arm Cortex-M MCU Portfolio

**Last Updated:** September 2026  
**Cortex-M Families Covered:** 24  
**Platform:** Arm Cortex-M0/M0+/M3/M4/M7/M33/M55

---

## 📋 Quick Navigation by Category

| Category | Families | Use Cases |
|----------|----------|-----------|
| **Mainstream/General Purpose** | C0, F0, F1, G0 | Entry-level, industrial, consumer appliances |
| **High-Performance** | F2, F3, F4, F7, G4, H5, H7 | DSP, motor control, graphics, edge AI |
| **Ultra-Low Power** | L0, L1, L4, L4+, L5, U0, U3, U5 | Wearables, IoT sensors, battery-operated devices |
| **Wireless/Connectivity** | WB, WB0, WBA, WL | Bluetooth, Zigbee, Thread, LoRa, sub-GHz |
| **AI & Edge Computing** | N6 | Neural processing, edge AI applications |

---

## 🔷 MAINSTREAM / GENERAL PURPOSE FAMILIES

### STM32C0 Series
**Category:** Entry-Level Mainstream MCU  
**ARM Core:** Cortex-M0+  
**Max Frequency:** 48 MHz  
**Flash Memory:** 16 - 256 KB  
**SRAM:** 8 - 36 KB  

#### Architecture
- 3-stage pipeline
- Armv6-M instruction set (Thumb, Thumb-2)
- Single core design
- No floating-point unit (FPU)
- Memory Protection Unit (MPU): No

#### Features
- 8 to 64 pin packages
- Low power consumption
- Integrated peripherals: UART, SPI, I2C, ADC
- Minimal cost - competes with 8/16-bit microcontrollers
- ECOPACK2 compliant

#### Use Cases
- **Entry-level cost-sensitive applications**
- Simple automation and control
- Replacing legacy 8-bit/16-bit systems
- IoT edge nodes
- Consumer electronics (basic)
- Smart meters (simple)
- Industrial switches/relays

---

### STM32C5 Series
**Category:** Entry-Level High-Performance MCU  
**ARM Core:** Cortex-M33F (with FPU)  
**Max Frequency:** 144 MHz  
**Flash Memory:** 128 KB - 1 MB  
**SRAM:** 32 - 256 KB  

#### Architecture
- Armv8-M Mainline architecture
- Dual-core capable (optional)
- Enhanced pipeline with L1 cache support
- Built-in FPU with DSP extensions
- TrustZone security extensions
- 16 MPU regions

#### Features
- Performance-to-cost optimized
- 64+ pin packages available
- CAN, USB, Ethernet capable variants
- Advanced security features
- LCD display support
- Sub-$1 pricing target

#### Use Cases
- **Smart IoT devices**
- Industrial control panels
- Advanced consumer appliances
- Medical device interfaces
- Building automation
- Security systems (basic)
- Smart home controllers

---

### STM32F0 Series
**Category:** Mainstream Entry-Level MCU  
**ARM Core:** Cortex-M0  
**Max Frequency:** 48 MHz  
**Flash Memory:** 16 - 256 KB  
**SRAM:** 4 - 32 KB  

#### Architecture
- 3-stage pipeline
- Armv6-M instruction set
- Smallest, lowest-cost 32-bit option
- No FPU, no DSP instructions
- Single core design

#### Features
- 20-100 pin packages
- 12-bit ADC with dual channels
- Multiple UART/SPI/I2C interfaces
- Analog comparators
- Timers and PWM outputs
- CAN bus support (select models)

#### Use Cases
- **Replacement for 8-bit MCUs**
- Simple motor control
- LED drivers and lighting control
- Temperature monitoring
- Simple sensor interfaces
- Consumer appliances
- Industrial timers/counters

---

### STM32F1 Series
**Category:** Mainstream General Purpose  
**ARM Core:** Cortex-M3  
**Max Frequency:** 72 MHz  
**Flash Memory:** 16 - 1024 KB  
**SRAM:** 4 - 96 KB  

#### Architecture
- 3-stage pipeline
- Armv7-M instruction set
- Thumb, Thumb-2 instruction support
- Single core design
- 8 MPU regions
- Embedded Trace Macrocell (ETMv3)

#### Features
- Highly compatible and widely used
- 36-144 pin packages
- Performance Line, Access Line, Value Line variants
- Rich peripheral set: UART, SPI, I2C, CAN, USB, ADC
- General purpose timers
- Watchdog timers
- Excellent community support

#### Use Cases
- **Industrial automation**
- Motor control applications
- Robotics and drone controllers
- Home automation devices
- Power management systems
- Data logging
- Educational/prototyping projects
- Medical equipment (basic)

---

### STM32G0 Series
**Category:** Mainstream Low-Cost High-Value  
**ARM Core:** Cortex-M0+  
**Max Frequency:** 64 MHz  
**Flash Memory:** 32 - 512 KB  
**SRAM:** 8 - 144 KB  

#### Architecture
- 2-stage pipeline (more efficient than M0)
- Armv6-M instruction set
- Better energy per instruction than M0
- MPU support with 8 regions
- Integrated Trace Buffer (MTB)

#### Features
- 48-176 pin packages
- 12-bit ADC with 16 channels
- Advanced timer capabilities
- CAN and FDCAN support
- USB, UART, SPI, I2C interfaces
- Temperature monitoring
- Excellent power efficiency

#### Use Cases
- **Next-gen entry-level IoT**
- Industrial control and monitoring
- Wireless sensor networks (base)
- Smart city applications
- Building management systems
- Asset tracking (simple)
- Appliance control
- Power conversion systems

---

## 🔴 HIGH-PERFORMANCE FAMILIES

### STM32F2 Series
**Category:** High-Performance Mainstream  
**ARM Core:** Cortex-M3  
**Max Frequency:** 120 MHz  
**Flash Memory:** 128 KB - 1 MB  
**SRAM:** 64 - 128 KB  

#### Architecture
- 3-stage pipeline
- Armv7-M instruction set
- Enhanced performance over F1 series
- Advanced Encryption Standard (AES) support
- 8 MPU regions

#### Features
- 100-144 pin packages
- Advanced security features
- High-speed USB device/OTG
- Multiple CAN channels
- 16-channel ADC
- High-resolution timers
- Cryptographic accelerator

#### Use Cases
- **Secure IoT gateways**
- Industrial communication devices
- Medical device controllers
- Payment terminals
- Secure firmware updates
- Network security applications
- Encrypted communication nodes

---

### STM32F3 Series
**Category:** Mixed-Signal & DSP Processing  
**ARM Core:** Cortex-M4F (with FPU & DSP)  
**Max Frequency:** 72 MHz  
**Flash Memory:** 32 - 512 KB  
**SRAM:** 12 - 80 KB  

#### Architecture
- 3-stage pipeline
- Armv7-M instruction set
- Single-precision FPU (32-bit)
- DSP instructions (SIMD, MAC operations)
- 8 MPU regions
- Embedded Trace Macrocell (ETMv3)

#### Features
- 48-176 pin packages
- Advanced analog features
- CORDIC math accelerator
- Unique for mixed-signal applications
- Multiple high-speed ADCs
- Comparators with windowing
- Real-time PWM control
- CAN and USB support

#### Use Cases
- **Precision motor control (brushless DC, stepper)**
- Sensor signal processing
- Power factor correction
- Digital signal processing
- High-frequency switching power supplies
- Programmable logic controllers (PLC)
- Real-time control systems
- Phase measurement

---

### STM32F4 Series
**Category:** High-Performance Standard  
**ARM Core:** Cortex-M4F (with FPU & DSP)  
**Max Frequency:** 180 MHz  
**Flash Memory:** 64 - 2048 KB  
**SRAM:** 64 - 384 KB  

#### Architecture
- 3-stage pipeline
- Armv7-M instruction set
- Full-featured FPU
- Complete DSP instruction set
- 8 MPU regions
- Embedded Trace Macrocell (ETMv4)

#### Features
- 100-176 pin packages (LQFP, BGA options)
- Industry standard for DSP/signal processing
- High-speed ADC with DMA
- Multiple SPI/I2C/UART interfaces
- Ethernet (select models)
- Camera interface (DCMI)
- LCD controller
- USB device/host/OTG

#### Use Cases
- **Audio processing and signal analysis**
- Digital signal processing (DSP)
- Machine vision (image processing)
- Sensor hubs (multi-sensor fusion)
- Industrial gateways
- Automotive applications
- Scientific instruments
- Network security appliances
- High-end consumer electronics

---

### STM32F7 Series
**Category:** High-Performance Advanced  
**ARM Core:** Cortex-M7F (with FPU & DSP)  
**Max Frequency:** 216 MHz  
**Flash Memory:** 64 - 2048 KB  
**SRAM:** 64 - 512 KB  

#### Architecture
- 6-stage superscalar pipeline
- Armv7-M instruction set
- L1 instruction & data cache (up to 32 KB each)
- Dual-precision FPU
- Advanced DSP instructions
- 8 MPU regions
- Embedded Trace Macrocell (ETMv4)

#### Features
- 100-176 pin packages (LQFP, BGA)
- Instruction and data caches
- High-speed performance
- LCD/TFT display controller
- Ethernet controller
- USB OTG device/host
- Advanced ADC with multiple channels
- CAN with multiple channels

#### Use Cases
- **Rich graphical interfaces (GUI)**
- Industrial automation systems
- Advanced measurement instruments
- Real-time audio/video processing
- Embedded vision applications
- Network appliances
- HMI (Human Machine Interface)
- High-speed data acquisition
- Automotive infotainment

---

### STM32G4 Series
**Category:** Mixed-Signal Advanced DSP  
**ARM Core:** Cortex-M4F (with FPU & DSP)  
**Max Frequency:** 170 MHz  
**Flash Memory:** 64 - 512 KB  
**SRAM:** 32 - 128 KB  

#### Architecture
- 3-stage pipeline optimized for DSP
- Armv7-M instruction set
- Single-precision FPU
- Full DSP instruction set (CORDIC, FMAC)
- 8 MPU regions with MPU-enabled vector tables

#### Features
- 64-176 pin packages
- CORDIC math accelerator (sine, cosine, etc.)
- FMAC instruction support
- High-resolution ADCs
- Precision comparators with windowing
- Advanced timer capabilities
- CAN and FDCAN support
- Thermal management features

#### Use Cases
- **Advanced motor control (FOC, sensorless)**
- Power factor correction (PFC)
- Digital power management
- Renewable energy systems (solar inverters, wind turbines)
- Smart power supplies
- High-frequency switching control
- Phase-shift PWM generators
- Real-time parameter estimation

---

### STM32H5 Series
**Category:** High-Performance Secure  
**ARM Core:** Cortex-M33F (with FPU & DSP)  
**Max Frequency:** 250 MHz  
**Flash Memory:** 128 KB - 4 MB  
**SRAM:** 128 - 640 KB  

#### Architecture
- Armv8-M Mainline architecture
- Superscalar pipeline with branch prediction
- TrustZone security (hardware isolation)
- Single-precision FPU with DSP extensions
- 16 MPU regions
- Enhanced trace capabilities (ETMv4)

#### Features
- 100-176 pin packages (LQFP, BGA)
- Hardware TrustZone for secure/non-secure partitioning
- Hardware acceleration for cryptography
- Secure boot capabilities
- Memory protection mechanisms
- High-speed interfaces (USB OTG, Ethernet)
- ADC with multiple high-speed channels
- CAN FD support

#### Use Cases
- **IoT edge computing with security**
- Industrial control with authentication
- Secure payment terminals
- Medical device gateways
- Smart home controllers (secure)
- Connected vehicle systems
- Building access control
- Industrial 4.0 nodes with security
- Firmware protection systems

---

### STM32H7 Series
**Category:** High-Performance Flagship  
**ARM Core:** Cortex-M7F + Cortex-M4F (dual-core options)  
**Max Frequency:** Up to 600 MHz (M7); 240 MHz (M4 on dual-core variants)  
**Flash Memory:** 256 KB - 2 MB  
**SRAM:** 256 KB - 1060 KB  

#### Architecture
- 6-stage superscalar pipeline (M7)
- Armv7-M instruction set
- L1 instruction & data caches
- Dual-precision FPU
- Advanced DSP instructions
- 16 MPU regions
- Embedded Trace Macrocell (ETMv4)
- Optional dual-core architecture

#### Features
- 144-176+ pin packages (LQFP, BGA)
- Highest performance in STM32 portfolio
- Dual-core variants (M7 + M4)
- Dedicated hardware accelerators
- LCD/TFT/HDMI display support
- Gigabit Ethernet (select models)
- USB 3.1 high-speed (select models)
- Multiple CAN FD channels
- Advanced memory controllers

#### Use Cases
- **Edge AI and neural networks**
- Advanced industrial robotics
- Machine vision and image processing
- Real-time video streaming
- 3D graphics rendering
- Network security gateways
- Industrial automation controllers
- Autonomous systems
- High-speed data acquisition/analysis
- Complex embedded systems

---

## 🔵 ULTRA-LOW POWER FAMILIES

### STM32L0 Series
**Category:** Ultra-Low Power Entry-Level  
**ARM Core:** Cortex-M0+  
**Max Frequency:** 32 MHz  
**Flash Memory:** 4 - 192 KB  
**SRAM:** 2 - 20 KB  

#### Architecture
- 2-stage pipeline
- Armv6-M instruction set
- Energy-optimized design
- Integrated low-power oscillators
- 8 MPU regions (optional)

#### Features
- 24-100 pin packages
- Ultra-low active current: ~250µA/MHz
- Stop2 mode: ~1µA with RAM retention
- Real-time clock (RTC)
- Multiple low-power modes
- LCD controller support
- UART, SPI, I2C interfaces
- Watchdog and timers

#### Use Cases
- **Ultra-low power IoT sensors**
- Wearable devices (watches, fitness trackers)
- Smart meters and gas meters
- Building occupancy sensors
- Environmental monitoring nodes
- Wireless sensor networks
- Battery-powered remote controls
- Energy-harvesting applications
- Long-life medical sensors

---

### STM32L1 Series
**Category:** Ultra-Low Power Mainstream  
**ARM Core:** Cortex-M3  
**Max Frequency:** 32 MHz  
**Flash Memory:** 4 - 384 KB  
**SRAM:** 4 - 48 KB  

#### Architecture
- 3-stage pipeline
- Armv7-M instruction set
- Energy-optimized design
- Integrated RTC
- 8 MPU regions

#### Features
- 48-144 pin packages
- Balanced performance and power
- Multiple low-power modes
- LCD controller support
- Advanced timers
- UART, SPI, I2C, CAN interfaces
- Temperature monitoring
- Comparators with windowing

#### Use Cases
- **Portable measurement instruments**
- Handheld testers and multimeters
- Environmental data loggers
- Smart thermostats
- Portable medical devices
- Low-power data acquisition
- Wireless condition monitoring
- Portable audio devices
- Industrial portable tools

---

### STM32L4 Series
**Category:** Ultra-Low Power High-Value  
**ARM Core:** Cortex-M4F (with FPU & DSP)  
**Max Frequency:** 80 MHz  
**Flash Memory:** 64 KB - 1 MB  
**SRAM:** Up to 320 KB  

#### Architecture
- 3-stage pipeline
- Armv7-M instruction set
- Single-precision FPU
- DSP instructions
- 8 MPU regions
- Integrated cache controller

#### Features
- 64-176 pin packages
- Ultra-low active current: ~70µA/MHz
- Stop2 mode: ~1µA with RAM retention
- DMA controllers with multiple channels
- Advanced ADC (12-bit, 16 channels)
- Multiple SPI, I2C, UART channels
- USB device interface
- Touch sensing support
- Timers for PWM and capture

#### Use Cases
- **Battery-powered IoT devices**
- Smart fitness trackers
- Wireless weather stations
- Portable medical monitors
- Handheld data collectors
- Industrial portable sensors
- Smart water/gas meters
- Smart locks and security devices
- Wireless body area network (WBAN)
- Asset tracking with extended battery

---

### STM32L4+ Series
**Category:** Ultra-Low Power Enhanced  
**ARM Core:** Cortex-M4F (with FPU & DSP)  
**Max Frequency:** 120 MHz  
**Flash Memory:** 512 KB - 2 MB  
**SRAM:** Up to 640 KB  

#### Architecture
- 3-stage pipeline optimized for energy
- Armv7-M instruction set
- Single-precision FPU with DSP
- Enhanced clock management
- 8 MPU regions
- Dual DMA controllers

#### Features
- 64-176 pin packages
- Step-up from STM32L4
- 20% faster than STM32L4
- Improved DSP capabilities
- High-resolution timers
- Multiple display interfaces
- Advanced analog features
- CAN and FDCAN support
- Ethernet capable (select models)

#### Use Cases
- **Advanced wearable devices**
- Smart home display panels
- Industrial smart meters
- Medical monitoring systems
- Portable diagnostic devices
- Wireless sensor gateways
- Real-time parameter estimation
- Signal processing applications
- Connected fitness equipment

---

### STM32L5 Series
**Category:** Ultra-Low Power Secure  
**ARM Core:** Cortex-M33F (with FPU & DSP)  
**Max Frequency:** 110 MHz  
**Flash Memory:** 32 - 512 KB  
**SRAM:** Up to 256 KB  

#### Architecture
- Armv8-M Mainline architecture
- TrustZone security extensions
- Single-precision FPU with DSP
- 16 MPU regions
- Enhanced trace capabilities

#### Features
- 100-176 pin packages (LQFP, BGA)
- Hardware TrustZone partitioning
- Secure boot mechanisms
- Cryptographic accelerator
- Advanced security features
- USB device/host interface
- Ethernet interface
- Advanced analog and timing capabilities
- LCD/TFT display support

#### Use Cases
- **Secure IoT edge nodes**
- Connected medical devices
- Smart home security systems
- Industrial IoT with authentication
- Building access control
- Secure payment terminals
- Firmware-protected devices
- Encrypted sensor networks
- Healthcare monitoring with HIPAA compliance

---

### STM32U0 Series
**Category:** Ultra-Low Power Entry-Level (Latest)  
**ARM Core:** Cortex-M0+  
**Max Frequency:** 56 MHz  
**Flash Memory:** 16 - 256 KB  
**SRAM:** 8 - 36 KB  

#### Architecture
- Enhanced 2-stage pipeline
- Armv6-M instruction set
- Optimized for battery life
- Integrated low-power modules
- MPU support (optional)

#### Features
- 32-100 pin packages
- Ultra-low active and sleep currents
- Background DMA capabilities
- Multiple low-power timers
- UART, SPI, I2C interfaces
- ADC with DMA
- Watchdog timer
- Integrated RTC

#### Use Cases
- **Next-gen entry-level IoT**
- Simple battery-operated sensors
- Wireless remote controls
- Smart doorbell systems
- Portable environmental monitors
- Low-cost medical alert devices
- Asset tags and beacons
- Industrial sensor nodes
- Smart city applications

---

### STM32U3 Series
**Category:** Ultra-Low Power High-Performance  
**ARM Core:** Cortex-M33F (with FPU & DSP)  
**Max Frequency:** 96 MHz  
**Flash Memory:** 512 KB - 2 MB  
**SRAM:** Up to 640 KB  

#### Architecture
- Armv8-M Mainline architecture
- TrustZone security (optional)
- Single-precision FPU with DSP
- 16 MPU regions
- Integrated memory accelerators

#### Features
- 64-176 pin packages
- Autonomous background operations (LPBAM)
- Peripherals function while core sleeps
- Advanced low-power modes
- Multiple DMA channels
- High-resolution ADC
- USB device interface
- CAN and FDCAN support
- Graphics and touch support

#### Use Cases
- **Market-leading power-efficient IoT**
- Always-on sensor monitoring
- Smart metering (electricity, water, gas)**
- Portable medical devices with displays
- Wearable fitness and health trackers
- Industrial IoT with graphics
- Smart home panels and controllers
- Connected wellness devices
- Background data collection systems

---

### STM32U5 Series
**Category:** Ultra-Low Power Flagship  
**ARM Core:** Cortex-M33F (with FPU & DSP)  
**Max Frequency:** 160 MHz  
**Flash Memory:** 128 KB - 4 MB  
**SRAM:** Up to 3 MB  

#### Architecture
- Armv8-M Mainline architecture
- TrustZone security extensions
- Single-precision FPU with DSP
- 16 MPU regions
- Dual DMA controllers
- Cache controller (optional)

#### Features
- 100-176 pin packages (LQFP, BGA)
- Autonomous background mode (LPBAM) - ST's flagship feature
- Graphics and display support
- USB device/host/OTG
- Ethernet interface
- Advanced cryptographic accelerator
- High-speed ADC and DAC
- CAN FD support
- Multiple communication interfaces

#### Use Cases
- **Ultra-low power edge AI**
- Portable medical diagnostic devices
- Advanced wearables (smartwatches with display)**
- Smart home gateways with local processing
- Industrial portable measurement tools
- Graphics-capable battery-powered devices
- Secure biometric systems
- Health monitoring hubs
- Connected appliance controllers
- IoT gateways with security

---

## 📡 WIRELESS / CONNECTIVITY FAMILIES

### STM32WB Series
**Category:** Wireless Dual-Core Multiprotocol  
**ARM Cores:** Cortex-M4F (64 MHz) + Cortex-M0+ (32 MHz)  
**Max Frequency:** 64 MHz (Application), 32 MHz (Network)  
**Flash Memory:** 256 - 1024 KB  
**SRAM:** 64 - 256 KB  

#### Architecture
- Dual-core design for efficient wireless processing
- Cortex-M4F for application logic
- Cortex-M0+ dedicated for radio stack
- Inter-Processor Communication Controller (IPCC)
- Hardware semaphores for resource sharing
- Single 2.4 GHz radio transceiver

#### Features
- 48-100 pin packages (UQFN, VQFN, WLCSP)
- Bluetooth Low Energy (BLE) 5.4 support
- IEEE 802.15.4 MAC/PHY (Zigbee, Thread compatible)
- Concurrent multiprotocol operation
- Matter and Aliro support
- OTA firmware updates (BLE and 802.15.4)
- Quad SPI memory interface with XIP
- AES encryption engine
- Multiple DMA channels

#### Use Cases
- **Smart home automation (Zigbee/Thread)**
- Bluetooth Low Energy fitness trackers
- Wireless sensor networks
- IoT beacon systems
- Home security systems
- Wireless lighting control (Philips Hue compatible)
- Medical fitness devices
- Smart locks and access control
- Wireless audio devices
- Matter-enabled home devices
- Industrial wireless sensors
- Asset tracking systems

---

### STM32WB0 Series
**Category:** Wireless Entry-Level Compact  
**ARM Cores:** Cortex-M0+  
**Max Frequency:** 64 MHz  
**Flash Memory:** 192 - 512 KB  
**SRAM:** Up to 64 KB  

#### Architecture
- Single-core optimized design
- Cortex-M0+ running both application and radio
- Efficient for simple wireless tasks
- 2.4 GHz radio integrated

#### Features
- Ultra-compact packages (WLCSP-49)
- Bluetooth Low Energy support
- Minimal power consumption
- Basic peripheral set
- OTA update capability
- AES-128 encryption

#### Use Cases
- **Cost-sensitive Bluetooth devices**
- Simple wireless sensors
- Compact beacons
- Wearable tags
- Remote control devices
- Smart button controllers
- Wireless switches
- Medical alert devices
- Asset tracking (simple)
- IoT node endpoints

---

### STM32WBA Series
**Category:** Wireless Advanced Multiprotocol  
**ARM Core:** Cortex-M33F (with FPU & DSP)  
**Max Frequency:** 100 MHz  
**Flash Memory:** 512 KB - 2 MB  
**SRAM:** Up to 512 KB  

#### Architecture
- Advanced Cortex-M33 with FPU
- 40nm modern process
- TrustZone security (optional)
- Enhanced 2.4 GHz radio
- Integrated RF front-end

#### Features
- 100-176+ pin packages (LQFP, BGA)
- Bluetooth Low Energy 5.4 + audio support
- IEEE 802.15.4 (Zigbee, Thread, Matter, Aliro)
- +10 dBm transmit power (extended range)
- Graphics and display support
- USB device/OTG
- Ethernet interface (select)
- Advanced ADC and DAC
- CAN and FDCAN support

#### Use Cases
- **Next-generation wireless IoT**
- Advanced Bluetooth audio devices
- High-powered wireless speakers
- Smart displays with connectivity
- Industrial wireless gateways
- Secure wireless controllers
- Enhanced range IoT devices
- Graphics-capable wireless nodes
- Medical wireless hubs
- Premium smart home devices
- Industrial Matter-compliant systems

---

### STM32WL Series
**Category:** Wireless Long-Range Sub-GHz  
**ARM Core:** Cortex-M4 (48 MHz) + Cortex-M0+ (48 MHz, optional)  
**Max Frequency:** 48 MHz  
**Flash Memory:** 64 - 256 KB  
**SRAM:** 20 - 64 KB  

#### Architecture
- Single or dual-core architecture
- Dedicated sub-GHz radio transceiver
- Support for long-range modulations
- LoRa, FSK, GFSK, MSK, BPSK modulation support
- Multi-band radio (European/US/Asian)

#### Features
- 48-100 pin packages
- Long-range communication (up to 40+ km LoRa)
- Sub-GHz frequency bands (868/915 MHz)
- Dual power amplifiers (+15 dBm, +22 dBm)
- LoRa RX sensitivity: -148 dBm (SF12)
- LoRaWAN stack support
- Sigfox compatible
- W-MBUS support (smart metering)
- mioty protocol support
- Multiple modulation flexibility

#### Use Cases
- **Long-range IoT networks (LoRaWAN)**
- Smart metering and utility monitoring
- Remote environmental sensors
- Wide-area sensor networks
- Industrial asset tracking (wide range)
- Smart city applications
- Agricultural monitoring systems
- Remote building/facility monitoring
- Energy management systems
- Sigfox-based IoT applications
- W-MBUS smart meters

---

## 🤖 EDGE AI / NEURAL PROCESSING

### STM32N6 Series
**Category:** AI Edge Computing Accelerator  
**ARM Core:** Cortex-M55  
**Max Frequency:** 800 MHz  
**On-Chip Memory:** Up to 4.2 MB SRAM  

#### Architecture
- Cortex-M55 superscalar pipeline
- Armv8.1-M instruction set
- Helium vector extensions (SIMD)
- Integrated Neural Processing Unit (NPU)
- Dual 32-bit MAC per cycle capability
- Advanced cache hierarchy

#### Features
- 100-176+ pin packages (LQFP, BGA)
- On-chip neural network inference
- Tensor Flow Lite Micro support
- STM32Cube AI integration
- High-speed ADC with DMA
- Advanced signal processing
- USB OTG interface
- Ethernet interface
- CAN and FDCAN support
- Multiple communication protocols

#### Use Cases
- **Edge AI and machine learning**
- Real-time audio processing (speech recognition)**
- Computer vision (object detection, classification)
- Anomaly detection in IoT sensors
- Predictive maintenance systems
- Medical signal analysis
- Industrial defect detection
- Smart sensor data interpretation
- Neural network inference at the edge
- On-device AI without cloud connectivity
- Biometric authentication
- Real-time gesture recognition

---

## 📊 COMPARISON MATRIX: Architecture & Performance

### By ARM Core Type

| Core | Architecture | Pipeline | FPU | DSP | Cache | MPU | Max Speed | Series |
|------|--------------|----------|-----|-----|-------|-----|-----------|--------|
| **M0** | Armv6-M | 3-stage | No | No | No | No | 48 MHz | F0 |
| **M0+** | Armv6-M | 2-stage | No | No | No | No/Yes | 64 MHz | C0, G0, L0, U0, WB0 |
| **M3** | Armv7-M | 3-stage | No | No | No | 8 | 120 MHz | F1, F2, L1 |
| **M4F** | Armv7-M | 3-stage | Yes | Yes | No | 8 | 180 MHz | F3, F4, G4, L4, WB |
| **M7F** | Armv7-M | 6-stage | Yes | Yes | Yes | 8 | 550 MHz | F7, H7 |
| **M33F** | Armv8-M | Modern | Yes | Yes | No | 16 | 250 MHz | C5, H5, L5, U3, U5, WBA |
| **M55** | Armv8.1-M | Modern | Yes | Yes | Yes | 16 | 800 MHz | N6 |

### By Performance Tier

| Tier | Series | Speed | Flash | SRAM | FPU | Typical Price |
|------|--------|-------|-------|------|-----|----------------|
| **Ultra-Low Cost** | C0, F0 | 48 MHz | ≤256KB | ≤32KB | No | $0.50-$1.50 |
| **Entry-Level** | G0, L0, U0 | 32-64 MHz | ≤512KB | ≤144KB | No | $1.00-$3.00 |
| **Mainstream** | F1, C5 | 72-144 MHz | ≤1MB | ≤256KB | Opt. | $2.00-$6.00 |
| **Mixed-Signal** | F3, G4 | 72-170 MHz | ≤512KB | ≤128KB | Yes | $3.00-$8.00 |
| **High-Perf DSP** | F4 | 180 MHz | ≤2MB | ≤384KB | Yes | $5.00-$15.00 |
| **Flagship HP** | F7, H5, H7 | 216-550 MHz | ≤2MB | ≤1MB | Yes | $8.00-$25.00 |
| **Ultra-Low Pwr** | L4, L5, U5 | 80-160 MHz | ≤2MB | ≤786KB | Opt. | $4.00-$12.00 |
| **Wireless** | WB, WBA, WL | 48-400 MHz | ≤2MB | ≤512KB | Opt. | $6.00-$20.00 |
| **AI Edge** | N6 | 800 MHz | ≤2MB | ≤1MB | Yes | $12.00-$30.00 |

---

## 🎯 QUICK SELECTION GUIDE

### By Application Type

#### 🔧 **Industrial Automation & Control**
- **Simple PLC**: STM32F1, STM32G0
- **Advanced Motion Control**: STM32F4, STM32G4
- **High-Speed Real-Time**: STM32H7
- **Secure Gateway**: STM32H5
- **Edge Computing**: STM32H7, STM32N6

#### 📱 **IoT & Wireless**
- **Ultra-Low Power Sensor**: STM32L0, STM32U0
- **Smart Meter**: STM32U3, STM32WL
- **Smart Home Device**: STM32WB, STM32WBA
- **Long-Range IoT**: STM32WL (LoRa)
- **Secure IoT Node**: STM32L5, STM32U5

#### 🏥 **Medical Devices**
- **Simple Monitor**: STM32L1, STM32L4
- **Portable Diagnostic**: STM32L4+, STM32L5
- **Secure Gateway**: STM32H5, STM32U5
- **Wearable Health**: STM32L0, STM32U3

#### 🎮 **Consumer Electronics**
- **Smart Home**: STM32WB, STM32WBA
- **Wearables**: STM32L0, STM32L4, STM32U3
- **Smart Appliances**: STM32C0, STM32G0
- **Rich Display**: STM32L4+, STM32H5, STM32H7

#### 🚗 **Automotive**
- **Body Electronics**: STM32F1, STM32G0
- **Motor Control**: STM32G4, STM32H7
- **Infotainment**: STM32F7, STM32H7
- **Advanced ADAS**: STM32H7, STM32N6

#### 🔐 **Security & Authentication**
- **Secure Devices**: STM32L5, STM32H5, STM32U5
- **Payment Terminals**: STM32F2, STM32H5
- **Access Control**: STM32F4, STM32L5

#### 🤖 **AI & Machine Learning**
- **Edge Inference**: STM32N6 (with NPU)
- **Signal Processing**: STM32H7, STM32F7
- **Audio Processing**: STM32F4, STM32N6

---

## 📝 KEY SELECTION CRITERIA MATRIX

| Criteria | Priority | Recommended Series |
|----------|----------|-------------------|
| **Lowest Cost** | High | C0, F0 |
| **Ultra-Low Power** | High | L0, U0, L4+ |
| **Wireless Connectivity** | High | WB, WL, WBA |
| **Performance (Speed)** | High | H7, N6 |
| **DSP/Signal Processing** | High | F4, G4, H7 |
| **Security/TrustZone** | High | L5, H5, U5 |
| **Graphics Support** | High | F7, H5, H7, U5, WBA |
| **Simple Features** | High | C0, F0, G0 |
| **Automotive Compatible** | Medium | F4, H7, H5 |
| **Educational/Prototyping** | Medium | F1, F4, Nucleo boards |
| **Medical Grade** | Medium | L4+, L5, U5 |

---

## 🛠️ DEVELOPMENT ECOSYSTEM

### Common Development Boards (Nucleo Series)
- **Nucleo-32**: STM32C0, F0, L4, G4 (compact, 32 pins)
- **Nucleo-64**: STM32F1, F4, L4, H7 (standard, 64 pins)
- **Nucleo-144**: STM32H7, F7, U5 (full-featured, 144 pins)
- **Discovery Boards**: Educational development
- **Evaluation Boards**: Production-ready reference designs

### Software Tools
- **STM32CubeMX**: Device configuration and code generator
- **STM32CubeIDE**: Integrated development environment (free)
- **IAR Embedded Workbench**: Professional IDE
- **Keil µVision**: ARM-based development
- **STM32Cube HAL**: Hardware abstraction layer
- **LL (Low Layer)**: Register-level API
- **STM32Cube AI**: Machine learning framework
- **FreeRTOS**: Real-time operating system support
- **Zephyr RTOS**: Open-source RTOS

### Debugging & Programming
- ST-Link USB debugger (included with Nucleo boards)
- SEGGER J-Link support
- Serial Wire Debug (SWD), JTAG interfaces
- On-chip debugging with breakpoints
- Real-time trace (Embedded Trace Buffer/ETM)

---

## 📚 ADDITIONAL RESOURCES

### Official STMicroelectronics
- **Web:** https://www.st.com/stm32
- **Wiki:** https://wiki.stmicroelectronics.com/stm32mcu
- **Datasheets:** Available for all series
- **Reference Manuals:** Complete technical documentation
- **Application Notes:** Specific use case guidance

### Community & Support
- **STM32 Community Forum:** Active user support
- **GitHub:** STM32 code examples and projects
- **ARM CMSIS:** Common microcontroller software interface
- **Cortex Microcontroller Software Interface Standard (CMSIS)**

---

## ✅ SUMMARY TABLE: CORTEX-M FAMILIES (A-Z)

| Family | Arm Core | Max Speed | Flash | SRAM | Primary Position |
|--------|----------|-----------|-------|------|------------------|
| **C0** | Cortex-M0+ | 48 MHz | 16 - 256 KB | Up to 36 KB | Mainstream / cost-sensitive |
| **C5** | Cortex-M33 | 144 MHz | 128 KB - 1 MB | Up to 256 KB | Mainstream / performance |
| **F0** | Cortex-M0 | 48 MHz | 16 - 256 KB | Up to 32 KB | Mainstream / legacy |
| **F1** | Cortex-M3 | 72 MHz | 16 KB - 1 MB | Up to 96 KB | Mainstream / legacy |
| **F2** | Cortex-M3 | 120 MHz | 128 KB - 1 MB | Up to 128 KB | High performance / legacy |
| **F3** | Cortex-M4 | 72 MHz | 32 - 512 KB | Up to 80 KB | Mixed-signal |
| **F4** | Cortex-M4 | 180 MHz | 64 KB - 2 MB | Up to 384 KB | High performance / DSP |
| **F7** | Cortex-M7 | 216 MHz | 64 KB - 2 MB | Up to 512 KB | High performance / graphics |
| **G0** | Cortex-M0+ | 64 MHz | 16 - 512 KB | Up to 144 KB | Mainstream |
| **G4** | Cortex-M4 | 170 MHz | 32 - 512 KB | Up to 128 KB | Mixed-signal / motor control |
| **H5** | Cortex-M33 | 250 MHz | 128 KB - 4 MB | Up to 1.5 MB | Secure high performance |
| **H7** | Cortex-M7 / Cortex-M4 | Up to 600 / 240 MHz | 64 KB - 2 MB | Up to 1.4 MB | High performance |
| **L0** | Cortex-M0+ | 32 MHz | 8 - 192 KB | Up to 20 KB | Ultra-low power |
| **L1** | Cortex-M3 | 32 MHz | 4 - 384 KB | Up to 48 KB | Ultra-low power / legacy |
| **L4** | Cortex-M4 | 80 MHz | 64 KB - 1 MB | Up to 320 KB | Ultra-low power |
| **L4+** | Cortex-M4 | 120 MHz | 512 KB - 2 MB | Up to 640 KB | Ultra-low power / enhanced |
| **L5** | Cortex-M33 | 110 MHz | 32 - 512 KB | Up to 256 KB | Secure ultra-low power |
| **N6** | Cortex-M55 | 800 MHz | Device-dependent | Up to 4.2 MB SRAM | Edge AI / multimedia |
| **U0** | Cortex-M0+ | 56 MHz | 16 - 256 KB | Up to 20 KB | Ultra-low power |
| **U3** | Cortex-M33 | 96 MHz | 512 KB - 2 MB | Up to 640 KB | Ultra-low power / security |
| **U5** | Cortex-M33 | 160 MHz | 128 KB - 4 MB | Up to 3 MB | Ultra-low power / security |
| **WB** | Cortex-M4 + Cortex-M0+ | 64 / 32 MHz | 256 KB - 1 MB | Up to 256 KB | Wireless |
| **WB0** | Cortex-M0+ | 64 MHz | 192 - 512 KB | Up to 64 KB | Wireless BLE |
| **WBA** | Cortex-M33 | 100 MHz | 512 KB - 2 MB | Up to 512 KB | Wireless multiprotocol |
| **WL** | Cortex-M4 + Cortex-M0+ | 48 / 48 MHz | 64 - 256 KB | Up to 64 KB | Sub-GHz wireless |

> **Verification note:** These are family-level portfolio ranges. Exact memory, peripherals, package options, and clock limits vary by part number and sub-family.

---

## 🔎 VERIFICATION & SCOPE

This document is intentionally limited to **STM32 Cortex-M microcontroller families**. STM32MP microprocessor families such as MP1 and MP2 have been removed because they are heterogeneous MPU platforms rather than Cortex-M-only MCU families.

The family lineup and portfolio-level headline specifications were checked against STMicroelectronics' current STM32 Cortex-M MCU portfolio. ST currently describes STM32 MCUs as Arm Cortex-M based and groups them across mainstream, high-performance, ultra-low-power, and wireless applications.

### Current corrections applied

- **STM32H7:** current ST portfolio reaches **up to 600 MHz** for Cortex-M7 devices; dual-core variants can also include a 240 MHz Cortex-M4.
- **STM32WBA:** current devices use **Cortex-M33 up to 100 MHz**, not 400 MHz; current products extend to 2 MB Flash and up to 512 KB RAM.
- **STM32WB0:** current portfolio lists **Cortex-M0+ up to 64 MHz**, with 192–512 KB Flash and up to 64 KB RAM.
- **STM32N6:** current devices use **Cortex-M55 at 800 MHz** and provide up to **4.2 MB SRAM**; selected devices include the Neural-ART accelerator.
- **STM32U5:** current portfolio reaches **4 MB Flash and up to 3 MB RAM** at the family level.
- **STM32L4 / L4+:** current portfolio reaches **1 MB Flash / 320 KB RAM** for L4 and **2 MB Flash / 640 KB RAM** for L4+.
- **STM32U3:** current portfolio reaches **2 MB Flash / 640 KB RAM**.
- **STM32L5:** current portfolio reaches **512 KB Flash / 256 KB RAM**.
- **STM32F2 / F3:** current portfolio ranges were corrected to match ST's current family-level portfolio data.
- **STM32WB0:** the earlier wording implying dual-core communication was removed; the family is presented as Cortex-M0+ based.

### Scope note

Older/legacy STM32 Cortex-M families remain in this reference because they are genuine Cortex-M MCU families, even when ST now presents them as legacy products. The document therefore covers both current and legacy Cortex-M families.

For production design, always select the exact MCU part number and verify its datasheet, reference manual, package, temperature grade, lifecycle status, memory configuration, and peripheral availability before schematic or firmware freeze.

---

## 📌 NOTES & DISCLAIMERS

1. **Specifications** are representative and may vary by specific model number
2. **Pricing** is approximate and varies by volume, region, and supplier
3. **Flash & SRAM** values shown are typical maximum; variants exist with less memory
4. **Clock Speeds** may have low-power variants operating at lower frequencies
5. **Availability** may vary by region; check with local distributors
6. **Development Support** varies by series; STM32CubeMX, STM32CubeIDE, HAL/LL, CMSIS and third-party IDE/toolchains are available across the portfolio
7. **Long-term Support** varies by product; check the exact part number for lifecycle information
8. **Compatibility** - Similar STM32 ecosystem concepts ease migration, but peripherals and registers are not identical across families

---

**Document Version:** 2.0  
**Last Updated:** September 2026  
**Status:** Cortex-M Family Reference — verified against current ST portfolio

For the latest information and detailed datasheets, visit [STMicroelectronics Official Website](https://www.st.com/stm32)
