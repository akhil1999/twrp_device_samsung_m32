# Samsung Galaxy M32 4G SM-M325F/FV TWRP Device Tree

TWRP Device tree for the Samsung Galaxy M32 4G MediaTek

This tree compatible with TWRP 3.6.11 as of 30/04/2022

---
![Samsung Galaxy M32 4G](https://fdn2.gsmarena.com/vv/pics/samsung/samsung-galaxy-m32-1.jpg)


# About Device

Samsung Galaxy M32 4G MediaTek (m32)

### Specifications

Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Octa-core 6x1.8GHz Cortex-A55 + 2x2.0Ghz Cortex-A75, ARM big.LITTLE
Chipset | MediaTek Helio G80
GPU     | ARM Mali G52 MC2
Memory  | 4 GB / 6 GB / 8 GB
Shipped Android Version | 11.0
Updated Android Version | N/A
Storage | 64 GB / 128 GB
MicroSD | Up to 256 GB
Battery | 6000 mAh (non-removable) (SM-M325F) / 5000 mAh (non-removable) (SM-M325FV)
Dimensions | 159.3 x 74 x 8.4 mm (SM-M325FV) or 9.3 mm (SM-M325F)
Display | 1080 x 2400 pixels, 6.4" Super AMOLED
Rear Camera  | 64 MP, f/1.8, 26mm (wide), 1/1.97", 0.7µm, PDAF, 8 MP, f/2.2, 123˚, (ultrawide), 1/4.0", 1.12µm, 2 MP, f/2.4, (macro), 2 MP, f/2.4, (depth), LED Flash
Front Camera | 20 MP, f/2.2, (wide)

---

#  Steps to Compile

 Place the device tree in proper location $SOURCE_HOME/device/samsung/k3gxx/ 
 
 Add AOSP TWRP Source or Minimal TWRP Source
 
 `repo init -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-11`
 
Then Run `repo sync` 

```sh
. source ./build/envsetup.sh && lunch twrp_m32-eng && make clean && make -j# recoveryimage
```
`# = No. of CPU threads of your PC'

#  Kernel Source here

 Kernel Source from which the prebuilt kernel is built is here, twrp-6.0 branch.
 
 Will be added shortly.

### Thanks to:
 * Me, akhil1999
 * TeamWin

