This directory contains the second stage bootloader and firmware for
booting the Raspberry Pi as a mass-storage device. The files here are
embedded into the `rpiboot` executable as part of the build process.

************************************************************************
This is not supported on Pi5 and deprecated on CM4
please use the mass-storage-gadget64 instead.

```bash
sudo rpiboot -d mass-storage-gadget64
```

************************************************************************

To load the files from this directory directly, run:  

```bash
cd msd
../rpiboot -d .
```
