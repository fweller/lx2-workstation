# Solid-Run Links

## Documentation

- [Datasheet](https://www.solid-run.com/wp-content/uploads/2021/01/HoneyComb-LX2-Datasheet.pdf)
- [SolidRun Developer Center](https://solidrun.atlassian.net/wiki/spaces/developer/overview)
- [SolidRun LX2 Quick Start Guide](https://solidrun.atlassian.net/wiki/spaces/developer/pages/197494288/HoneyComb%2BLX2%2BClearFog%2BCX%2BLX2%2BQuick%2BStart%2BGuide)
- [Arm SystemReady ES V1.0: Errata Document](https://armkeil.blob.core.windows.net/developer/Files/pdf/certificate-list/arm-systemready-errata-document-solidrun-lx2-ver6.pdf)
- [SolidRun LX2160A Developer Pages](https://solidrun.atlassian.net/wiki/spaces/developer/pages/197493977/LX2160A%2BBased%2BProducts)
- [Github SolidRun's LX2160A COM express type 7 build scripts](https://github.com/SolidRun/lx2160a_build)
- [Github SolidRun's LX2160A COM express type 7 UEFI build](https://github.com/SolidRun/lx2160a_uefi)
- [SolidRun is ARM SystemReady ES Compliant](https://www.solid-run.com/blog/articles/solidrun-joins-arms-systemready-compliant-partners/)

## Support

- [SolidRun Community](https://community.solid-run.com/c/nxp-lx2160/6)
- [HoneyComb Distro-Installation Part 1 and 2](https://community.solid-run.com/t/honeycomb-distro-installation-part-1-and-2/301)
- [Developer Center](http://developer.solid-run.com/)
- [Developer Ecosystem discord channel](https://discord.gg/yFnRAWF%20)

## Software

- [SolidRun LX2160A Software](https://solidrun.atlassian.net/wiki/spaces/developer/pages/197494345/LX2160A%2BSoftware)
- [SolidRun GitHub](https://github.com/SolidRun)
- [Pre-built images](https://images.solid-run.com/LX2k/lx2160a_build) based on Ubuntu 20.04
  - The prebuilt images are configured for SO-DIMM DDR4 with speed of 3200, 2900, 2600 and 2400 Mtps (with or without ECC support)
  - Images that have the prefix lx2160a\_xspi are intended to be flashed into SPI and recommended for later use after being booted from micro SD
  - `$ xz -dc lx2160acex7_2000_700_....img.xz | dd of=/dev/sdX bs=4k conv=fdatasync`
  - Ubuntu username and password are ‘root’ and ‘root’.
- [UEFI firmware pre-built](https://images.solid-run.com/LX2k/lx2160a_uefi)
- [Build your own image](https://github.com/SolidRun/lx2160a_build)
