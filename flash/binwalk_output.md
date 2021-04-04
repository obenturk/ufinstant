obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk boot.bin

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
104928        0x199E0         uImage header, header size: 64 bytes, header CRC: 0x29C42FC4, created: 2019-11-01 09:40:29, image size: 73144 bytes, Data Address: 0x81C00000, Entry Point: 0x81C00000, data CRC: 0x47E6CAB0, OS: Firmware, CPU: MIPS, image type: Firmware Image, compression type: lzma, image name: "U-Boot 2011.12.NA for rtl9601C"
104992        0x19A20         LZMA compressed data, properties: 0x5D, dictionary size: 16777216 bytes, uncompressed size: 191344 bytes

obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk cfgfs.bin

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             JFFS2 filesystem, big endian
102480        0x19050         Zlib compressed data, compressed
102940        0x1921C         Zlib compressed data, compressed
104024        0x19658         Zlib compressed data, compressed
105108        0x19A94         JFFS2 filesystem, big endian
110672        0x1B050         Zlib compressed data, compressed
111012        0x1B1A4         Zlib compressed data, compressed
112080        0x1B5D0         Zlib compressed data, compressed
113280        0x1BA80         Zlib compressed data, compressed
113836        0x1BCAC         JFFS2 filesystem, big endian
114248        0x1BE48         Zlib compressed data, compressed
114688        0x1C000         JFFS2 filesystem, big endian
143440        0x23050         Zlib compressed data, compressed
143668        0x23134         Zlib compressed data, compressed
144860        0x235DC         Zlib compressed data, compressed
145404        0x237FC         Zlib compressed data, compressed
146240        0x23B40         JFFS2 filesystem, big endian
146512        0x23C50         Zlib compressed data, compressed
147456        0x24000         JFFS2 filesystem, big endian
161876        0x27854         Zlib compressed data, compressed
162924        0x27C6C         JFFS2 filesystem, big endian
163920        0x28050         Zlib compressed data, compressed
164628        0x28314         Zlib compressed data, compressed
165824        0x287C0         Zlib compressed data, compressed
166312        0x289A8         JFFS2 filesystem, big endian
188496        0x2E050         Zlib compressed data, compressed
188944        0x2E210         Zlib compressed data, compressed
189488        0x2E430         Zlib compressed data, compressed
190576        0x2E870         Zlib compressed data, compressed
191812        0x2ED44         JFFS2 filesystem, big endian
191948        0x2EDCC         Zlib compressed data, compressed
192592        0x2F050         Zlib compressed data, compressed
192892        0x2F17C         Zlib compressed data, compressed
193428        0x2F394         Zlib compressed data, compressed
193964        0x2F5AC         Zlib compressed data, compressed
194500        0x2F7C4         Zlib compressed data, compressed
195036        0x2F9DC         Zlib compressed data, compressed
195572        0x2FBF4         Zlib compressed data, compressed
196036        0x2FDC4         JFFS2 filesystem, big endian
222304        0x36460         Zlib compressed data, compressed
223168        0x367C0         Zlib compressed data, compressed
224264        0x36C08         Zlib compressed data, compressed
224836        0x36E44         Zlib compressed data, compressed
225360        0x37050         Zlib compressed data, compressed
225724        0x371BC         Zlib compressed data, compressed
226272        0x373E0         Zlib compressed data, compressed
227352        0x37818         Zlib compressed data, compressed
228552        0x37CC8         Zlib compressed data, compressed
229052        0x37EBC         JFFS2 filesystem, big endian
229168        0x37F30         Zlib compressed data, compressed
229268        0x37F94         JFFS2 filesystem, big endian
229456        0x38050         Zlib compressed data, compressed
230140        0x382FC         Zlib compressed data, compressed
230616        0x384D8         JFFS2 filesystem, big endian
230744        0x38558         Zlib compressed data, compressed
231624        0x388C8         Zlib compressed data, compressed
232516        0x38C44         Zlib compressed data, compressed
233632        0x390A0         Zlib compressed data, compressed
234100        0x39274         JFFS2 filesystem, big endian
234224        0x392F0         Zlib compressed data, compressed
235268        0x39704         Zlib compressed data, compressed
235804        0x3991C         Zlib compressed data, compressed
236924        0x39D7C         Zlib compressed data, compressed
237648        0x3A050         JFFS2 filesystem, big endian
237768        0x3A0C8         Zlib compressed data, compressed
238104        0x3A218         Zlib compressed data, compressed
238216        0x3A288         Zlib compressed data, compressed
238368        0x3A320         JFFS2 filesystem, big endian
238492        0x3A39C         Zlib compressed data, compressed
239284        0x3A6B4         JFFS2 filesystem, big endian
239404        0x3A72C         Zlib compressed data, compressed
240448        0x3AB40         Zlib compressed data, compressed
241664        0x3B000         JFFS2 filesystem, big endian

obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk env.bin

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------

obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk env2.bin

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------

obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk hw.bin

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             JFFS2 filesystem, big endian
4296          0x10C8          Zlib compressed data, compressed
4756          0x1294          JFFS2 filesystem, big endian

obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk kernel1.bin

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             uImage header, header size: 64 bytes, header CRC: 0xF307F7DC, created: 2019-11-01 09:44:09, image size: 1017779 bytes, Data Address: 0x80000000, Entry Point: 0x80000000, data CRC: 0x15E35227, OS: Linux, CPU: MIPS, image type: OS Kernel Image, compression type: lzma, image name: "Linux Kernel Image"
64            0x40            LZMA compressed data, properties: 0x5D, dictionary size: 16777216 bytes, uncompressed size: 3448068 bytes

obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk kernel2.bin

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             uImage header, header size: 64 bytes, header CRC: 0xF307F7DC, created: 2019-11-01 09:44:09, image size: 1017779 bytes, Data Address: 0x80000000, Entry Point: 0x80000000, data CRC: 0x15E35227, OS: Linux, CPU: MIPS, image type: OS Kernel Image, compression type: lzma, image name: "Linux Kernel Image"
64            0x40            LZMA compressed data, properties: 0x5D, dictionary size: 16777216 bytes, uncompressed size: 3448068 bytes

obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk rootfs1.bin

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             Squashfs filesystem, little endian, version 4.0, compression:lzma, size: 2226519 bytes, 403 inodes, blocksize: 131072 bytes, created: 2019-11-01 09:44:08

obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk rootfs2.bin

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------
0             0x0             Squashfs filesystem, little endian, version 4.0, compression:lzma, size: 2226519 bytes, 403 inodes, blocksize: 131072 bytes, created: 2019-11-01 09:44:08

obenturk@HomeAssistant:~/uboot-mdb-dump$ binwalk sec.bin

DECIMAL       HEXADECIMAL     DESCRIPTION
--------------------------------------------------------------------------------

obenturk@HomeAssistant:~/uboot-mdb-dump$
