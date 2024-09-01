To update the SPI EEPROM bootloader on a Compute Module 4.

* Modify the EEPROM configuration in `boot.conf` as desired
* Optionally, replace pieeprom.original.bin with a custom version. The default
  version here is the latest stable release recommended for use on Compute Module 4.
* Run `update-eeprom.sh` to create the image to flash

```bash
cd recovery
./update-pieeprom.sh
../rpiboot -d .
```

N.B The `bootcode4.bin` file in this directory is actually the `recovery.bin`
file used on Raspberry Pi 4 bootloader update cards.

