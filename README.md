# Linux kernel port for Lumia 950/XL smartphones
------------------------






## Currently supported features:


#### Talkman (msm8992, Lumia 950 non-XL):


- SDHCI/eMMC

- EFIFB



#### Cityman (msm8994, Lumia950XL):


- SDHCI/eMMC

- EFIFB

- Synaptics RMI4 touchscreen

- SD Card (the driver is picky and will only accept SOME cards)



------------------------
## Build guide

make ARCH=arm64 CROSS_COMPILE=/path/to/your/cross/compiler/prefix- lumia_defconfig

make ARCH=arm64 -j$(nproc)

Your kernel image will be at arch/arm64/boot/Image.gz along with the DTB over at arch/arm64/boot/dts/msm899[...].dtb

------------------
Original README can be found at README.linux
