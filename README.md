Linux kernel 5.10.6 for RTD1295 (Qua station)
===

!!THIS KERNEL DOESN'T WORK!!
  Becouse it maybe arch/arm64/* or some address wrong.



## make
  
*Export env
```bash
$ export ARCH=arm64;export BOARD=BPI-W2-720P;export SOC=rtd1295;export MACH=rtd129x;export CROSS_COMPILE=toolchains/gcc-arm-10.2-2020.11-x86_64-aarch64-none-linux-gnu/bin/aarch64-none-linux-gnu-;export GPU_TYPE="mali820";export TARGET_PLATFORM=realtek;export TARGET_PRODUCT=bpi-w2
```
  
*make 
```bash
$ make -j8 ARCH=arm64 CROSS_COMPILE=toolchains/gcc-arm-10.2-2020.11-x86_64-aarch64-none-linux-gnu/bin/aarch64-none-linux-gnu- INSTALL_MOD_PATH=output UIMAGE_LOADADDR=0x03000000 LOADADDR=0x03000000 modules Image dtbs
```
