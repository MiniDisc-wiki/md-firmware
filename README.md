# md-firmware
Firmware dumps for MiniDisc recorders!

So far we have the firmware for the MZ-R700 (c1.3, non net-md) and the MZ-N510 (v1.6 net-md). These firmwares are likely shared among many same generation devices.

Rom starts at 0x00000000 (load the the roms at this address).
Ram starts at 0x02000000.
Peripherals are at 0x03000000.

The SoC for the R700 uses an ARM7TDMI core (ARMv4t), the MZ-N series probably something similar. Code can perfectly be decompiled and is a mix of ARM and Thumb code.
