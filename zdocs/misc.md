# ROM

The Old World ROM is always 4 megabytes (MB). The first three MB are reserved for the 68k code, while the last MB is for the PowerPC boot-up code.

# Serial

For serial, it replicates the functionality of a Zilog ESCC. There are two different ports - one located at 0xF3013000 for the printer, and the other at 0xF3013020 for the modem.

# DBDMA

The Description-Based Direct Memory Access relies on memory-based descriptions, minimizing CPU interrupts.

# SWIM 3

The SWIM 3 (Sanders-Wozniak integrated machine 3) is the floppy drive.

# NVRAM

Mac OS relies on 8 KB of NVRAM at minimum to run properly. It's usually found at IOBase (ex.: 0xF3000000 for Power Mac G3 Beige) + 0x60000.

# Miscellaneous

The Power Mac G3 Beige has an additional register at 0xFF000004, which is dubbed varyingly as the "cpu-id" (by OpenFirmware), the ""systemReg" (display driver) or "MachineID" (platform driver).