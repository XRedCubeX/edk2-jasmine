# EDK2 for Xiaomi Mi A2.

Based on Danct12's port for Xiaomi Redmi Note 7 (lavender) (https://github.com/dreemurrs-embedded/edk2-lavender).

## Status 

What works:
- Display
- UEFI Shell

What does not work:
- Clocks
- eMMC (SdccDxe requires Clocks)
...


## Building
Tested on Arch Linux.

First, clone EDK2.

```
cd ..
git clone https://github.com/tianocore/edk2.git --recursive
git clone https://github.com/tianocore/edk2-platforms.git
```

You should have all three directories side by side.

Finally, ./build.sh.

Then `fastboot boot uefi.img`.

# Credits

This is based on Danct12's port for Xiaomi Redmi Note 7 (lavender) (https://github.com/dreemurrs-embedded/edk2-lavender),which is based on fxsheep's [Mi6 port](https://github.com/fxsheep/edk2-sagit/), which is based on zhuowei's [edk2-pixel3](https://github.com/Pixel3Dev/edk2-pixel3).  
SimpleFbDxe screen driver is from imbushuo's [Lumia950XLPkg](https://github.com/WOA-Project/Lumia950XLPkg).  
Special thanks to @lemon1ice and @imbushuo for guidance.
