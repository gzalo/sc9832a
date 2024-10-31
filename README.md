# SC9832A
This repo will eventually have an open fdl1, bootloader, Linux kernel and filesystem for Spreadtrum SC9832A. It will only work in a particular blu cellphone that has microprocessor (BLU C5 Max). **DO NOT USE IN OTHER MODELS, it will brick them**.

Usage:
- Turn off the device
- Enable USB download mode (short TX and GND)
- Connect the device through USB, it should get detected as "SPRD U2S DIAG"
- Use [SPD research tool](https://spdflashtool.com/category/research-tool) or [yuanxinos_usb](https://github.com/JiaDuo/yuanxinos_usb/tree/master) tools to interact with the device (read/write partitions and such)

Sources:
- FDL1: `BLU ZSL1805` [Could have been one of these](https://firmwarefile.com/?s=sc9832a)

Missing:
- Compile [chipram](https://github.com/jingpad-bsp/bsp_bootloader_chipram) to replace fdl1.bin
- Compile [uboot](https://github.com/jingpad-bsp/bsp_bootloader_u-boot15) + LCD driver additions
- Compile [kernel](https://github.com/jedld/kernel_9832_7)
- Compile basic Linux filesystem

Files provided with absolutely no warranty, use them at your own risk. Don't expect any support. Make backups of all partitions.
License: check each project
