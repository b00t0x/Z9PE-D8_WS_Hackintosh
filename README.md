# Z9PE-D8 WS
## Software
* macOS Big Sur 11.2.1 (20D74)
* macOS Catalina 10.15.7 (19H524)
* OpenCore 0.6.6

## Hardware
* MB : ASUS Z9PE-D8 WS ( BIOS `5802` mod )
* CPU : 2x E5-2667 v2
* GPU : SAPPHIRE NITRO+ RADEON RX 470 8G GDDR5 OC

## Benchmark
### Normal
* Geekbench 3 : [52,830](https://browser.geekbench.com/geekbench3/8844446)
* Geekbench 4 : [46,649](https://browser.geekbench.com/v4/cpu/15224978)
* Geekbench 5 : [11,793](https://browser.geekbench.com/v5/cpu/1214139)

### Overclock (BCLK 108 MHz)
* Geekbench 3 : [57,445](https://browser.geekbench.com/geekbench3/8844427)
* Geekbench 4 : [51,385](https://browser.geekbench.com/v4/cpu/15224865)
* Geekbench 5 : [12,909](https://browser.geekbench.com/v5/cpu/1213880)

## OpenCore settings
### kexts
#### from Kext Updater
* AppleALC.kext
* CpuTscSync.kext
* GenericUSBXHCI.kext
* Lilu.kext
* NVMeFix.kext
* SMCProcessor.kext
* SMCSuperIO.kext
* VirtualSMC.kext
* WhateverGreen.kext

#### from others
* AppleMCEReporterDisabler.kext
  * https://dortania.github.io/OpenCore-Install-Guide/ktext.html#extras

* IONetworkingFamilyInjector.kext
  * https://trick77.com/intel-gigabit-ct-kext-macos-sierra-10-12/

## Status
### Working
* Shutdown
* Power management with SSDT-CPU.aml
* Audio ( with `alcid=1` in config.plist )
  * Disable `Above 4G Decoding` in BIOS needed

### Not working
* Wake from sleep
* USB 3.0 in macOS 11 Big Sur

## Other
### BIOS mod
* NVMe Patch  
https://www.bios-mods.com/forum/Thread-Z9PE-D8-WS-Bios-mod-to-support-NVMe-m-2-support
* MSR Patch  
https://www.youtube.com/watch?v=fHAlsQvDMN4