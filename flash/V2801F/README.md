# V2801F

```
obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk rootfs

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             Squashfs filesystem, little endian, version 4.0, compression:lzma, size: 1880366 bytes, 623 inodes, blocksize: 131072 bytes, created: 2020-11-04 01:41:32

obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk uImage

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             uImage header, header size: 64 bytes, header CRC: 0xEE89A0DD, created: 2020-11-04 01:41:33, image size: 1199462 bytes, Data Address: 0x80000000, Entry Point: 0x80000000, data CRC: 0x4DEA4EF6, OS: Linux, CPU: MIPS, image type: OS Kernel Image, compression type: lzma, image name: "Linux Kernel Image"
64            0x40            LZMA compressed data, properties: 0x5D, dictionary size: 16777216 bytes, uncompressed size: 3923728 bytes

obenturk@HomeAssistant:~/uboot-mdb-dump$

```