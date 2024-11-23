```
──(kali㉿kali)-[~/picoCTFretos/e3/BOA2]
└─$ cat disassembler-dump0_b.txt 
<+0>:     endbr64 
<+4>:     push   rbp
<+5>:     mov    rbp,rsp
<+8>:     mov    DWORD PTR [rbp-0x14],edi
<+11>:    mov    QWORD PTR [rbp-0x20],rsi
<+15>:    mov    DWORD PTR [rbp-0x4],0x9fe1a
<+22>:    mov    eax,DWORD PTR [rbp-0x4]
<+25>:    pop    rbp
<+26>:    ret
```

Al convertir el número 0x9fe1a en decimal nos da el numéro 654874, dando como flag: picoCTF{654874}