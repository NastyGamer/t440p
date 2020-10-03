## This is a fork of [https://github.com/jloisel/t440p](https://github.com/jloisel/t440p).

This setus has been tested and confirmed to work on High Sierra, Mojave and Catalina.

## Compatibility

### What works

- Wifi
- Trackpad-gestures
- Power management
- Temperature sensors
- Battery status
- Brightness control
- Speakers
- USB ports
- Graphic acceleration (QE/CI)
- Audio Jack
- Display Port
- Ethernet
- Docking-station Ethernet / USB / Power / Audio Jack
- Bluetooth

### What doesn't work

- SD-Card reader
- Docking-station audio / display-connectors
- VGA



## Setup

### Bios Settings

The bios has to be configured properly prior to installing MacOS.

.
|-- Security  
|   |-- Security  
|   |   \`-- Security Chip  
|   |       \`-- Disabled  
|   |-- Memory Protection  
|   |   \`-- Execution Prevention  
|   |       \`-- Enabled  
|   |-- Internal Device Access  
|   |   \`-- Bottom Cover Tamper Detection  
|   |       \`-- Disabled  
|   |-- Anti-Theft  
|   |   \`-- Current Setting  
|   |       \`-- Disabled  
|   \`-- Secure Boot  
|       \`-- Secure Boot  
|           \`-- Disabled  
\`-- Startup  
    |-- UEFI / Legacy Boot  
    |   \`-- Both  
    |-- UEFI / Legacy Priority  
    |   \`-- UEFI First  
    \`-- CSM Support  
        \`-- Yes  


## SSD Enable Trim

To enable trim on your SSD, run:

```
sudo trimforce enable
```