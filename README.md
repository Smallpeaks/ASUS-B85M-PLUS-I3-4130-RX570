## ASUS-B85M-PLUS-I3-4130-RX570
华硕 B85M-PLUS-I3-4130-RX570-OC1.0.5-Mac15.4

硬件配置：

Opencore: 1.0.5 

Version: macOS Sequoia 15.xx

我这台黑苹果主机的整体配置清单如下：

cpu： 英特尔 I3 4130

主板：华硕 B85M F PLUS

显卡：华硕 RX570 8G

音频: Realtek ALC887 8 声道音效芯片

网卡: Realtek RTL8111GR 千兆网卡

硬盘：SL500 1TB  SSD

内存条：威刚 16G 1600* DDR3

无线网卡：ntel AX210

图形: ntel® HD Graphics 4400 显卡   禁用 

ASUS-B85M-PLUS系列主板 MacOS 15.4 完善程度：

CPU睿频正常

板载音频正常

核显支持HDMI/DP 显示输出

前后3.5音频输出皆正常

睡眠唤醒正常，支持USB唤醒

有线网卡RealtekRTL8111正常使用

方案一：板载intel AX210 蓝牙 和WIFi都可以驱动，网速非常不错 ，但不支持隔空随航；MacOS 15需搭配heliport APP使用WIFI功能

方案二：板载intel AX210 蓝牙 和WIFi都可以驱动，网速非常不错 ，但不支持隔空随航；MacOS 15 需要OCLP修补 这里使用方案二

若想实现隔空随航附加功能 需要买一张NVME M.2 SSD 转接黑果无线网卡

引导默认可支持独显（RX560/570/590/5500/5600/5700/等等系列）

就不一一说了

### OpenCore Configuration

### ACPI

| ACPIs                    |
|--------------------------|
|  SSDT-PLUG               |
|  SSDT-EC                 |
|  SSDT-GPRW               |
|  SSDT-PM                 | 
|  SSDT-PMC                |

### Drivers

| Driver Name     |
|-----------------|
| HfsPlus         |
| OpenCanopy      |
| OpenRuntime     |
| ResetNvramEntry |
| ToggleSipEntry  |

### Kexts


| Kext Name                             |
|---------------------------------------|
| Lilu.kext                             |
| VirtualSMC.kext                       |
| WhateverGreen.kext                    |
| SMCProcessor.kext                     |
| SMCSuperIO.kext                       |
| AppleALC.kext                         |
| RestrictEvents.kext                   |
| HoRNDIS.kext                          |
| RadeonSensor.kext                     |
| RealtekRTL8111.kext                   | 
| UTBMap.kext                           | 
| USBToolBox.kext                       | 
| IO80211FamilyLegacy.kext              | 
| IOSkywalkFamily                       |
| AirportItlwm-15.5Sequoia.kext         | 
| IntelBTPatcher.kext                   | 
| IntelBluetoothFirmware.kext           |
| BlueToolFixup.kext                    |
| AMFIPass.kext                         |


bios 设置参考：

Internal graphics >enable

Security

Intel Platform Trust Technology: Unchecked

Intel Software Guard Extension (SGX): Disabled

Thunderbold Security Level: Legacy mode

Boot

Secure Boot: Disabled

Fast Boot: Unchecked

若有其他问题请加Q群： 738882434
