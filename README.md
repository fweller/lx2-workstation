# Workstation build using Solid-Run Honeycomb NXP LX2160A ARM Processor

This project documents my build of

- A mini-ITX computer workstation
- Using the [Solid-Run HoneyComb LX2 Workstation](https://www.solid-run.com/arm-servers-networking-platforms/honeycomb-lx2/)
- Which is a combination of a mini-ITX motherboard
- And a COM Express Type 7 module
- That uses the [NXP Layerscape LX2160A 16-core ARM Cortex-A72 digital networking processor](https://www.nxp.com/products/processors-and-microcontrollers/arm-processors/layerscape-processors/layerscape-lx2160a-lx2120a-lx2080a-processors:LX2160A)

## Reference Material

- [Collection of articles](./articles.md) *reviews, instructions, benchmarks*
- [Collection of Solid-Run links](./solidrun-links.md) *documentation, support, software*

## Costs

I purchased all of the components in August of 2022 from either NewEgg or from Solid-Run directly.  The prices I list below are accurate as of that purchase.

| Cost    | Component |
| ------- | ----------------------- |
| $   892 | Motherboard |
| $   138 | RAM |
| $    85 | GPU AMD RX550 |
| $    71 | Chassis |
| $    80 | Power |
| $   100 | SSD |
| $    11 | SSD Heatsink |
| $    26 | Micro SD |
| $    15 | CPU Fan |
| $    54 | Chassis Fan x2 |
| $ 1,472 | TOTAL |

## Component Details

### Motherboard

- [SolidRun HoneyComb LX2](https://www.solid-run.com/arm-servers-networking-platforms/honeycomb-lx2/)
- Uses the Solid-Run CEx7 LX2K COM Express Type 7 Module
- SKU SRLX216S00D00GE064H09CH

### RAM

- Highly recommended to use [RAM that is tested by Solid-Run](https://solidrun.atlassian.net/wiki/spaces/developer/pages/197494332/LX2160A%2BCOM%2BTested%2BSO-DIMM%2BMemory)
- [Kingston FURY Impact 32GB (2 x 16GB) 260-pin SO-DIMM DDR4 3200 MHz CL20](https://shop.kingston.com/products/new-impact-ddr4-laptop-memory?variant=41005827784896)
- SKU [KF432S20IBK2/32](https://www.newegg.com/kingston-32gb-260-pin-ddr4-so-dimm/p/0RM-001W-005Z3?Item=9SIAEYEJ0P4190&Description=KF432S20IBK2%2F32&quicklink=true&cm_re=KF432S20IBK2%2F32-_-0RM-001W-005Z3-_-Product)

### GPU

- Note: Must carefully select a GPU chipset that has aarch64 source and binary support
  - The [AMD Radeon RX 550](https://www.amd.com/en/support/graphics/radeon-500-series/radeon-rx-500-series/radeon-rx-550) is a good choice
  - Nvidia would not be a good choice because they do not provide driver source
- [ASRock Phantom Gaming Radeon RX 550 2GB](https://www.asrock.com/Graphics-Card/AMD/Phantom%2520Gaming%2520Radeon%2520RX550%25202G/)
- [NewEgg](https://www.newegg.com/asrock-radeon-rx-550-rx550-2g/p/N82E16814930001?Item=N82E16814930001&quicklink=true)

### Chassis

- [NZXT H210](https://nzxt.com/product/h210)
- SKU [CA-H210B-BR](https://www.newegg.com/matte-black-red-nzxt-h-series-h210-mini-itx-tower/p/N82E16811146309?Description=NZXT%2520H210&cm_re=NZXT_H210-_-11-146-309-_-Product&quicklink=true)

### Power

- [MSI MPG A650GF 650 W ATX](https://www.msi.com/Power-Supply/MPG-A650GF)
- 80 PLUS GOLD modular
- [NewEgg](https://www.newegg.com/msi-mpg-a650gf-650w/p/N82E16817701011?quicklink=true)

### SSD

- [Western Digital WD_BLACK SN770 M.2 2280 1TB PCIe Gen4 16GT/s](https://www.westerndigital.com/products/internal-drives/wd-black-sn770-nvme-ssd?sku=WDS100T3X0E)
- SKU [WDS100T3X0E](https://www.newegg.com/western-digital-1tb-sn770/p/N82E16820250217?Item=N82E16820250217)

### MicroSD

- Note: MicroSD is used for holding the bootloaders
- SanDisk 64GB Extreme SDXC U3 A2
- SKU [SDSQXA2-064G-GN6MA](https://www.newegg.com/sandisk-64gb-microsdxc/p/N82E16820175006?quicklink=true)

### CPU Fan

- Note: The stock fan that ships with the Solid-Run board is very noisy and should be replaced
- [Noctua NF-A4x20 PWM 40x20mm](https://noctua.at/en/products/fan/nf-a4x20-pwm)
- 12V 40x40x20 PWM fan
- [NewEgg](https://www.newegg.com/noctua-nf-a4x20-pwm-case-fan/p/1YF-000T-00093?Description=Noctua%2520NF-A4x20&cm_re=Noctua_NF-A4x20-_-1YF-000T-00093-_-Product&quicklink=true)

### Chassis Fan

- Note: The stock chassis fans that ship with the chassis are quiet enough, the Notua fans were unnecessary
- [Noctua NF-A14 PWM chromax.black.swap](https://noctua.at/en/nf-a14-pwm-chromax-black-swap)
- [NewEgg](https://www.newegg.com/p/1YF-000T-004J3?Item=9SIAADY6HZ2209)
