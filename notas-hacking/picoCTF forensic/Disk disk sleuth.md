
──(kali㉿kali)-[~/Downloads]
└─$ sudo apt install sleuthkit
[sudo] password for kali: 
sleuthkit is already the newest version (4.12.1+dfsg-0kali6).
sleuthkit set to manually installed.
Summary:
  Upgrading: 0, Installing: 0, Removing: 0, Not Upgrading: 0
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Downloads]
└─$ sudo apt install autopsy
autopsy is already the newest version (2.24-6kali1).
autopsy set to manually installed.
Summary:
  Upgrading: 0, Installing: 0, Removing: 0, Not Upgrading: 0
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Downloads]
└─$ file dds1-alpine.flag.img.gz 
dds1-alpine.flag.img.gz: gzip compressed data, was "dds1-alpine.flag.img", last modified: Tue Mar 16 00:19:38 2021, from Unix, original size modulo 2^32 134217728
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Downloads]
└─$ mmls dds1-alpine.flag.img.gz
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Downloads]
└─$ gzip -d dds1-alpine.flag.img.gz
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Downloads]
└─$ mmls dds1-alpine.flag.img 
DOS Partition Table
Offset Sector: 0
Units are in 512-byte sectors

      Slot      Start        End          Length       Description
000:  Meta      0000000000   0000000000   0000000001   Primary Table (#0)
001:  -------   0000000000   0000002047   0000002048   Unallocated
002:  000:000   0000002048   0000262143   0000260096   Linux (0x83)
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Downloads]
└─$ srch_strings dds1-alpine.flag.img | grep pico
ffffffff81399ccf t pirq_pico_get
ffffffff81399cee t pirq_pico_set
ffffffff820adb46 t pico_router_probe
^[[B  SAY picoCTF{f0r3ns1c4t0r_n30phyt3_dcbf5942}
