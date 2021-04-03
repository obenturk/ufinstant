# ufinstant
mdb dump of ufinstant

flash dump made with following commands

9601C# sf probe 0
9601C# sf read 0x80000000 0x0 0x1000000
9601C# md.b 0x80000000 0x1000000

then converted to bin file with python3 uboot_mdb_to_image.py < uf_mdb_dump.txt > flash.bin

both files are included in repo.

binwalk

[CODE]obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk flash.bin

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
104928        0x199E0         uImage header, header size: 64 bytes, header CRC: 0x29C42FC4, created: 2019-11-01 09:40:29, image size: 73144 bytes, Data Address: 0x81C00000, Entry Point: 0x81C00000, data CRC: 0x47E6CAB0, OS: Firmware, CPU: MIPS, image type: Firmware Image, compression type: lzma, image name: "U-Boot 2011.12.NA for rtl9601C"
104992        0x19A20         LZMA compressed data, properties: 0x5D, dictionary size: 16777216 bytes, uncompressed size: 191344 bytes
278528        0x44000         JFFS2 filesystem, big endian
381008        0x5D050         Zlib compressed data, compressed
381468        0x5D21C         Zlib compressed data, compressed
382552        0x5D658         Zlib compressed data, compressed
383636        0x5DA94         JFFS2 filesystem, big endian
389200        0x5F050         Zlib compressed data, compressed
389540        0x5F1A4         Zlib compressed data, compressed
390608        0x5F5D0         Zlib compressed data, compressed
391808        0x5FA80         Zlib compressed data, compressed
392364        0x5FCAC         JFFS2 filesystem, big endian
392776        0x5FE48         Zlib compressed data, compressed
393216        0x60000         JFFS2 filesystem, big endian
421968        0x67050         Zlib compressed data, compressed
422196        0x67134         Zlib compressed data, compressed
423388        0x675DC         Zlib compressed data, compressed
423932        0x677FC         Zlib compressed data, compressed
424768        0x67B40         JFFS2 filesystem, big endian
425040        0x67C50         Zlib compressed data, compressed
425984        0x68000         JFFS2 filesystem, big endian
467024        0x72050         Zlib compressed data, compressed
467472        0x72210         Zlib compressed data, compressed
468016        0x72430         Zlib compressed data, compressed
469104        0x72870         Zlib compressed data, compressed
470340        0x72D44         JFFS2 filesystem, big endian
470476        0x72DCC         Zlib compressed data, compressed
471120        0x73050         Zlib compressed data, compressed
471420        0x7317C         Zlib compressed data, compressed
471956        0x73394         Zlib compressed data, compressed
472492        0x735AC         Zlib compressed data, compressed
473028        0x737C4         Zlib compressed data, compressed
473564        0x739DC         Zlib compressed data, compressed
474100        0x73BF4         Zlib compressed data, compressed
474564        0x73DC4         JFFS2 filesystem, big endian
494180        0x78A64         Zlib compressed data, compressed
495272        0x78EA8         JFFS2 filesystem, big endian
495696        0x79050         Zlib compressed data, compressed
495936        0x79140         JFFS2 filesystem, big endian
496876        0x794EC         Zlib compressed data, compressed
497964        0x7992C         Zlib compressed data, compressed
499208        0x79E08         Zlib compressed data, compressed
499724        0x7A00C         JFFS2 filesystem, big endian
500832        0x7A460         Zlib compressed data, compressed
501696        0x7A7C0         Zlib compressed data, compressed
502792        0x7AC08         Zlib compressed data, compressed
503364        0x7AE44         Zlib compressed data, compressed
503888        0x7B050         Zlib compressed data, compressed
504252        0x7B1BC         Zlib compressed data, compressed
504800        0x7B3E0         Zlib compressed data, compressed
505880        0x7B818         Zlib compressed data, compressed
507080        0x7BCC8         Zlib compressed data, compressed
507580        0x7BEBC         JFFS2 filesystem, big endian
507696        0x7BF30         Zlib compressed data, compressed
507796        0x7BF94         JFFS2 filesystem, big endian
507984        0x7C050         Zlib compressed data, compressed
508668        0x7C2FC         Zlib compressed data, compressed
509144        0x7C4D8         JFFS2 filesystem, big endian
509272        0x7C558         Zlib compressed data, compressed
510152        0x7C8C8         Zlib compressed data, compressed
511044        0x7CC44         Zlib compressed data, compressed
512160        0x7D0A0         Zlib compressed data, compressed
512628        0x7D274         JFFS2 filesystem, big endian
512752        0x7D2F0         Zlib compressed data, compressed
513796        0x7D704         Zlib compressed data, compressed
514332        0x7D91C         Zlib compressed data, compressed
515452        0x7DD7C         Zlib compressed data, compressed
516176        0x7E050         JFFS2 filesystem, big endian
516296        0x7E0C8         Zlib compressed data, compressed
516632        0x7E218         Zlib compressed data, compressed
516744        0x7E288         Zlib compressed data, compressed
516896        0x7E320         JFFS2 filesystem, big endian
517020        0x7E39C         Zlib compressed data, compressed
517812        0x7E6B4         JFFS2 filesystem, big endian
517932        0x7E72C         Zlib compressed data, compressed
518976        0x7EB40         Zlib compressed data, compressed
520192        0x7F000         JFFS2 filesystem, big endian
524288        0x80000         uImage header, header size: 64 bytes, header CRC: 0xF307F7DC, created: 2019-11-01 09:44:09, image size: 1017779 bytes, Data Address: 0x80000000, Entry Point: 0x80000000, data CRC: 0x15E35227, OS: Linux, CPU: MIPS, image type: OS Kernel Image, compression type: lzma, image name: "Linux Kernel Image"
524352        0x80040         LZMA compressed data, properties: 0x5D, dictionary size: 16777216 bytes, uncompressed size: 3448068 bytes
3670016       0x380000        Squashfs filesystem, little endian, version 4.0, compression:lzma, size: 2226519 bytes, 403 inodes, blocksize: 131072 bytes, created: 2019-11-01 09:44:08
8585216       0x830000        uImage header, header size: 64 bytes, header CRC: 0xF307F7DC, created: 2019-11-01 09:44:09, image size: 1017779 bytes, Data Address: 0x80000000, Entry Point: 0x80000000, data CRC: 0x15E35227, OS: Linux, CPU: MIPS, image type: OS Kernel Image, compression type: lzma, image name: "Linux Kernel Image"
8585280       0x830040        LZMA compressed data, properties: 0x5D, dictionary size: 16777216 bytes, uncompressed size: 3448068 bytes
11730944      0xB30000        Squashfs filesystem, little endian, version 4.0, compression:lzma, size: 2226519 bytes, 403 inodes, blocksize: 131072 bytes, created: 2019-11-01 09:44:08
16646144      0xFE0000        JFFS2 filesystem, big endian
16650440      0xFE10C8        Zlib compressed data, compressed
16650900      0xFE1294        JFFS2 filesystem, big endian
[/CODE]
