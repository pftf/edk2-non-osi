ARM Trusted Firmware for Raspberry Pi 4
=======================================

The `bl31.bin` ATF binary found in this directory was built from the
[official ATF 2.2 release](https://git.trustedfirmware.org/TF-A/trusted-firmware-a.git/snapshot/trusted-firmware-a-2.2.tar.gz)
through an [AppVeyor build script](https://github.com/pbatard/pitf/blob/master/appveyor.yml)
that is designed to provide evidence that the binary does match a vanilla source.

As per the [AppVeyor build log](https://ci.appveyor.com/project/pbatard/pitf/builds/28565852), the
SHA-256 sum for `bl31.bin` is `be96193501aa93bf5508696bbe058ab7ed76c82c93744d6eaeff58f6a99c53fa`.

For Raspberry Pi 4 usage, ATF was built using the command:
```
make PLAT=rpi4 RPI3_PRELOADED_DTB_BASE=0x20000 PRELOADED_BL33_BASE=0x30000 SUPPORT_VFP=1 DEBUG=0 all
```
