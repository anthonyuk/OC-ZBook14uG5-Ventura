# OC-ZBook14uG5-Ventura
Opencore 0.87 files for HP Zbook G5 MacOS 13 Ventura

You must add your own serial to the Platform Info section of the config.plist

# Spec
- Intel i5-8350u
- 16Gb RAM (2x 8Gb)



# Working

- UHD630 with 2560MB VRAM
- Brightness controls (inc. Sureview privacy filter)
- USB ports (2.0 & 3.0)
- Audio with internal speakers & audio jack
- Wifi - Native Apple BCM card
- Bluetooth
- Synaptics trackpad, up to 5 finger gestures
- PS2 keyboard
- Battery management
- USB type C data and video inc. dock
- Power Management
- Sleep
- iService
- Airdrop
- Continuity cam

# Not working

- Thunderbolt
- Built-in webcam
- Ethernet needs reconnecting to obtain DHCP lease
- Touchscreen/Card Reader not used so disabled in BIOS
- File Vault or Secure Boot is not configured

# BIOS setup

## Disable

- As much as possible until installed then you can try re-enabling if required

### These are a must though

- Fast Boot
- Secure Boot 
- VT-d (can be enabled if you set DisableIoMapper to YES)
- Compatibility Support Module (CSM) (Must be off in most cases, GPU errors/stalls like gIO are common when this option is enabled)
- Thunderbolt(For initial install, as Thunderbolt can cause issues if not setup correctly)
- Intel SGX
- Intel Platform Trust


## Enable
- VT-x
- Hyper-Threading
- DVMT Pre-Allocated(iGPU Memory): 64MB or higher
- SATA Mode: AHCI

