# md-firmware
Firmware dumps for MiniDisc recorders!

## About
In this repository you can find the firmware for various portable MiniDisc players. It is part of an ongoing effort to reverse engineer said devices.

## Hardware revisions
The major difference between firmwares is related to the SoC used. 

| **SoC** | **Flash size** | **Ram size** | **Flash start** | **Ram start** | **Peripherals start** | **CPU Core** | **NetMD** |
|---------|----------------|--------------|-----------------|---------------|-----------------------|--------------|-----------|
| CXD2671 | 0x60000 (393k) | 0x4000 (16k) | 0x00000000      | 0x02000000    | 0x03000000            | ARM7TDMI     | No        |
| CXD2677 | 0x70000 (459k) | 0x4800 (18k) | 0x00000000      | 0x02000000    | 0x03000000            | ARM          | Yes       |
| CXD2678 | 0xA0000 (640k) | 0x9000 (36k) | 0x00000000      | 0x02000000    | 0x03000000            | ARM          | Yes       |
| CXD2680 | 0xA0000 (640k) | 0x9000 (36k) | 0x00000000      | 0x02000000    | 0x03000000            | ARM          | Yes       |

## Available dumps
Generally the firmware for devices that share the same SoC is the same (per version), regardless of the exact model. Minor patches may have been applied to the dump (from the factory), so dumps can vary slightly (a couple of bytes) between devices.

| **CXD2671** | **Dumped devices**                                             |
|-------------|----------------------------------------------------------------|
| v1.3        | MZ-R700                                                        |

| **CXD2677** | **Dumped devices**                                             |
|-------------|----------------------------------------------------------------|
| v1.1        | MZ-S1                                                          |
| v1.3        | MZ-N505                                                        |
| v1.4        | MZ-N505, MZ-N1                                                 |

| **CXD2678 - CXD2680** | **Dumped devices**                                             |
|-----------------------|----------------------------------------------------------------|
| v1.0                  | MZ-N920                                                        |
| v1.1                  | MZ-N10                                                         |
| v1.3                  | MZ-N10                                                         |
| v1.4                  | MZ-N910                                                        |
| v1.6                  | MZ-N10, MZ-NE410, MZ-N510, MZ-NF520D, MZ-NF610, MZ-N710, MZ-N910, AIWA AM-NX9 |
| _Note_                | _CXD2678 and CXD2680 devices seem to share the same firmware_ |
