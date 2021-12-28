
# Module Introduction 



<img src="ModuleIntroduction.assets/modulenew.png" alt="SMARC-module-logo_500px"  style="zoom: 40%; margin-left: auto; margin-right: auto; display: block;" /> 



[Download Datasheet](https://hq0epm0west0us0storage.blob.core.windows.net/$web/public/SMARC/LEC-EL/documentation/LEC-EL-datasheet-preliminary-20211007.pdf) 




<div class = "bullets">

## The SMARC Formfactor

The SMARC (“Smart Mobility ARChitecture”) is a versatile small form factor computer on Module definition targeting applications that require low power, low costs, and high performance. The Modules will typically use ARM SOCs similar or the same as those used in many familiar devices such as tablet computers and smart phones. Alternative low power SOCs and CPUs, such as tablet oriented X86 devices and other RISC CPUs may be used as well. The Module power envelope is typically under 6W.

Two Module sizes are defined: 82 mm x 50 mm and 82 mm x 80 mm.

The Module PCBs have 314 edge fingers that mate with a low profile 314 pin 0.5 mm pitch right angle connector (the connector is sometimes identified as a 321 pin connector, but 7 pins are lost to the key).

The Modules are used as building blocks for portable and stationary embedded systems. The core CPU and support circuits, including DRAM, boot flash, power sequencing, CPU power supplies, GBE and a single channel LVDS display transmitter are concentrated on the Module. The Modules are used with application specific Carrier Boards that implement other features such as audio CODECs, touch controllers, wireless devices, etc. The modular approach allows scalability, fast time to market and upgradability while still maintaining low costs, low power and small physical size.

<img src="ModuleIntroduction.assets/logo.png" alt="logo" style="zoom:100%; margin-left: auto; margin-right: auto; display: block;" />

SMARC module and carrier specifications are

module and carrier specifications are
available online at : <https://www.sget.org/standards/smarc.html>

## Features

- Dual or quad-core Intel Atom® Series 
- SMARC revision 2.1.1 compliant 
- Up to 8GB LPDDR4 at 4266 MT/s 
- Dual channel LVDS 918/24-bit) 
- DP++, DP++ / HDMI 
- 1x SATA Gen 3 / onboard eMMC up to 256 GB 
- 10 year product availability 
- Dual CAN bus 
- USB2/ USB 3 interfaces 
- Dual 2.5 gigabit ethernet ports



## Specifications

### Core System

**CPU**

  - Intel Atom® X6425E,4 cores, 1.8GHz, 12W TDP

**Note:** We also have other versions

  - Intel Atom® X6413E,4 cores, 1.5GHz, 9W TDP 
  - Intel Atom® X6211E,2 cores, 1.2GHz, 6W TDP
  - Intel Atom® X6200FE,2 cores, 1.0GHz, 4.5W TDP (FUSA)
  - Intel Atom® X6414RE, 4 cores, 1.5GHz, 9W TDP 
  - Intel Atom® X6425RE, 4 cores, 1.9GHz, 12W TDP

**Memory**

  - 2,4,8 GB LPDDR4L-4266 (In Band ECC)

**Cache**

  - 1.5 MB system L2 cache 4MB LLC

**Security**

  - Intel® Boot Guard 
  - Intel® OS Guard 
  - Intel® Platform Trust Technology (Intel® PTT) 
  - Intel® AES-New Instruction, Intel® SHA Extensions 
  - Intel® Secure Key 
  - Digital Rights Management HDCP 2.3-Playready 4 
  - SMx Crypto Support
  - Intel® Virtualization Technology (Intel® VT) 
  - Intel® Dynamic Application Loader (Intel® DAL) 
  - Optional ATECC608 Crypto chip 
  - Optional TPM 2.0 module

### Video

**GPU Core**
  - Gen 11LP 4Kp60 @ 3 displays simultaneous 

**GPU Feature Support**

  - 11th generation Intel ® graphics core architecture with up to 32 execution units (selected SKUs), supports three independent displays 2D and 3D graphics hardware acceleration 
    
  - Support for DirectX 12, OpenGL 4.2, OpenCL 1.2 Video decode HW acceleration for H.265/HEVC, H.264, MPEG2, MVC, VC-1,      WMV9, JPEG/ MJPEG, VP8, VP9Video encode HW acceleration for H.265/HEVC, H.264, MPEG2, MV

**HDMI**
  - HDMI 2.0b 4K@60 Hz 

**LVDS**
  - Dual Channel LVDS 18/24 bit 

### Audio
 **Audio Codec**
  - HDA Audio codec (located on carrier)

### Dual Ethernet
**Primary LAN**

  - 10/100/1000/ 2.5 Gbit Ethernet with TSN

**Secondary LAN**

  - 10/100/1000/ 2.5 Gbit Ethernet with TSN



### Extension Busses

**USB**

  - 2x USB 3.0, 4x USB 2.0

**UART**

  - Four UART interfaces SER1 and SER 2 (CTS/RTS) / SER0 SER3 (TX/RX/CTS/RTS)

**CAN**

  - 2x CAN2.0B only or mixed CAN2.0B and CAN FD mode, data bit rate up to 8 Mbps

**SPI**

  - 2x SPI

**I<sup>2</sup>S**

   2x  I2S interfaces with audio resolution from 16-bits to 32-bits and sample rate up to 192KHz (see Audio Codec support)

**I<sup>2</sup>C**
  - Four I2C interfaces

    - Support for 7-bit and 10-bit address mode
    - Software programmable clock frequency of 100 kbit/s in Standard-mode, 400 kbit/s in the Fast-mode or 1 Mbit/s in Fast-mode Plus 

**GPIO**

  - 14x GPIO with interrupt, one GPIO with PWM 

**PCle**

  - 4x PCIe x1 Gen3

### System Storage

**SDIO**

  - 1x SDIO (4-bit) compatible with SD/SDIO standard, up to version 3.0

**eMMC**

  - 16, 32, 64 or 128 GB (build option)
  - Compatible with eMMC specifications 4.41, 4.51, 5.0 and 5.1

**SATA**
  - 1x SATA Gen3

### SEMA® Board Controller

  - Supports: Voltage/Current monitoring, Power Sequencing, Logistics and
 Forensic Information, Flat Panel Control, I²C Bus Control, GPIO Control, User Flash,
    Failsafe BIOS (dual BIOS), Watchdog Timer and Fan Control 

**Debug Header**

  -   30-pin multipurpose flat cable connector for use with optional DB-30 debug module
  - Provides JTAG, BMC access; UART, power testpoints; diagnostic LEDs, Power, Reset, Boot configuration 

### Power

**Input**

  - 5Vdc +/- 5%

### Mechanical and Environmental

**Form Factor**

  - SGET SMARC Specifications 2.1

**Dimensions**

  - SMARC short size module, 82 mm x 50 mm

**Operating Temperature**

  - Standard: 0°C to +60°C
  - Rugged: -40°C to +85°C (optional)

**Humidity**

  - 5-90% RH operating, non-condensing
  - 5-95% RH storage (and operating with conformal coating)

**Shock and Vibration**

  - IEC 60068-2-64 and IEC-60068-2-27, MIL-STD-202 F, Method 213B, Table 213-I, 
  - Condition A and Method 214A, Table 214-I, Condition D

**HALT**

  - Thermal Stress, Vibration Stress, Thermal Shock and Combined Test

### Operating Systems 

**Standard Support**

  - Yocto Linux BSP

 **Extended Support (BSP)**
  - VxWorks


</div>







