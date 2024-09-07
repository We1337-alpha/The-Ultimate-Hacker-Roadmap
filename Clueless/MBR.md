**MBR** (Master Boot Record) is a critical sector on a hard disk drive (HDD) or solid-state drive (SSD) that contains essential information about the disk's partitioning scheme and the location of the operating system's boot loader.

### Components of MBR:

- **Partition Table:** A table that defines the partitions on the disk, including their starting sector, size, and type.
- **Boot Loader:** A small program that loads the operating system's kernel into memory.

### How MBR Works:

1. **BIOS/UEFI reads MBR:** When a computer is powered on, the BIOS or UEFI (Unified Extensible Firmware Interface) reads the MBR from the first sector of the disk.
2. **Partition Table is checked:** The BIOS/UEFI examines the partition table to determine the active partition (the partition containing the operating system).
3. **Boot Loader is loaded:** The BIOS/UEFI loads the boot loader from the active partition.
4. **Operating System is loaded:** The boot loader transfers control to the operating system's kernel, which initializes the system and loads the rest of the operating system.

### Limitations of MBR:

- **Maximum partition size:** MBR has a maximum partition size limit of 2 TB.
- **Maximum partitions:** MBR can support a maximum of four primary partitions.

### GPT (GUID Partition Table)

To overcome the limitations of MBR, **GPT** (GUID Partition Table) was introduced. GPT allows for larger partitions and supports more than four partitions. Many modern systems now use GPT instead of MBR.

**In summary, MBR is a crucial component of a disk's partitioning scheme. It contains information about the disk's partitions and the location of the boot loader. While MBR has limitations, GPT is a more modern and flexible alternative.**
