# Haiku-riscv
Haiku port to RISC-V architecture

Latest version: revision 3.

[HiFive Unmatched](https://www.sifive.com/boards/hifive-unmatched) board is supported. Radeon graphics card is required for booting to desktop, text mode is not supported.

Booting instructions for HiFive Unmatched:

1. Connect USB keyboard and mouse.

2. Write release image to USB drive. USB 3 drive is recomended.

3. Connect board to UEFI terminal.

4. Start board and press any key on UART terminal to stop boot process.

5. Type following commands in UART u-boot promt: `pci enum ; usb start ; run bootcmd_usb0`.

6. When Haiku boot loader menu appear on UART terminal (not on screen) hit Enter key 3 times.

7. Boot process whould start and eventually desktop will be loaded.


Patchset is provided. Exact Haiku version should be used when appliying patchset.

![](https://raw.githubusercontent.com/X547/Haiku-riscv/main/screenshot.png)

Detail disscussion:

* https://discuss.haiku-os.org/t/my-haiku-risc-v-port-progress/10663

* https://discuss.haiku-os.org/t/my-progress-on-real-risc-v-hardware/10963
