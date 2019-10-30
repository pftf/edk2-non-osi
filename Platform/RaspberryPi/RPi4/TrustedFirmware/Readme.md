ARM Trusted Firmware for Raspberry Pi 4
=======================================

The `bl31.bin` ATF binary was built on a Debian 10.1 system from
https://github.com/ARM-software/arm-trusted-firmware/tree/cc76d670c152de45c03e6de646a7cfe2e7986e5b
with the command:

```
make PLAT=rpi4 PRELOADED_BL33_BASE=0x20000 RPI3_PRELOADED_DTB_BASE=0x10000 SUPPORT_VFP=1 RPI3_USE_UEFI_MAP=1 DEBUG=0 all
```
