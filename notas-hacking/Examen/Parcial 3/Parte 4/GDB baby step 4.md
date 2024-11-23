```
┌──(kali㉿kali)-[~/picoCTF/tercerparcial/parte4]
└─$ gdb -q debugger0_d
Reading symbols from debugger0_d...
(No debugging symbols found in debugger0_d)
(gdb) set disassembly-flavor intel
(gdb) info functions
All defined functions:

Non-debugging symbols:
0x0000000000401000  _init
0x0000000000401020  _start
0x0000000000401050  _dl_relocate_static_pie
0x0000000000401060  deregister_tm_clones
0x0000000000401090  register_tm_clones
0x00000000004010d0  __do_global_dtors_aux
0x0000000000401100  frame_dummy
0x0000000000401106  func1
0x000000000040111c  main
0x0000000000401150  __libc_csu_init
0x00000000004011c0  __libc_csu_fini
0x00000000004011c8  _fini
(gdb) 

```

```
┌──(kali㉿kali)-[~/picoCTF/tercerparcial/parte4]
└─$ python3       
Python 3.12.6 (main, Sep  7 2024, 14:20:15) [GCC 14.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 0x3269
12905
>>> 

```

