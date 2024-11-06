
# Solucion

```
┌──(kali㉿kali)-[~/Documents/picoCTF/reversing/needforspeed]
└─$ chmod +x need-for-speed 
                                                                                                                               
┌──(kali㉿kali)-[~/Documents/picoCTF/reversing/needforspeed]
└─$ ./need-for-speed 
Keep this thing over 50 mph!
============================

Creating key...
Not fast enough. BOOM!
                                                                                                                               
┌──(kali㉿kali)-[~/Documents/picoCTF/reversing/needforspeed]
└─$ gdb -q need-for-speed                                      
Reading symbols from need-for-speed...
(No debugging symbols found in need-for-speed)
(gdb) 
(gdb) set dissasembly-flavor intel
No symbol table is loaded.  Use the "file" command.
(gdb) dissasemble main
Undefined command: "dissasemble".  Try "help".
(gdb) disassemble main
Dump of assembler code for function main:
   0x000000000000091a <+0>:     push   %rbp
   0x000000000000091b <+1>:     mov    %rsp,%rbp
   0x000000000000091e <+4>:     sub    $0x10,%rsp
   0x0000000000000922 <+8>:     mov    %edi,-0x4(%rbp)
   0x0000000000000925 <+11>:    mov    %rsi,-0x10(%rbp)
   0x0000000000000929 <+15>:    mov    $0x0,%eax
   0x000000000000092e <+20>:    call   0x8d8 <header>
   0x0000000000000933 <+25>:    mov    $0x0,%eax
   0x0000000000000938 <+30>:    call   0x82f <set_timer>
   0x000000000000093d <+35>:    mov    $0x0,%eax
   0x0000000000000942 <+40>:    call   0x87d <get_key>
   0x0000000000000947 <+45>:    mov    $0x0,%eax
   0x000000000000094c <+50>:    call   0x8ac <print_flag>
   0x0000000000000951 <+55>:    mov    $0x0,%eax
   0x0000000000000956 <+60>:    leave
   0x0000000000000957 <+61>:    ret
End of assembler dump.
(gdb) j *(main+35)
The program is not being run.
(gdb) run
Starting program: /home/kali/Documents/picoCTF/reversing/needforspeed/need-for-speed 
[Thread debugging using libthread_db enabled]
Using host libthread_db library "/lib/x86_64-linux-gnu/libthread_db.so.1".
Keep this thing over 50 mph!
============================

Creating key...
Not fast enough. BOOM!
[Inferior 1 (process 28794) exited normally]
(gdb) b *(main+30)
Breakpoint 1 at 0x555555400938
(gdb) run
Starting program: /home/kali/Documents/picoCTF/reversing/needforspeed/need-for-speed 
[Thread debugging using libthread_db enabled]
Using host libthread_db library "/lib/x86_64-linux-gnu/libthread_db.so.1".
Keep this thing over 50 mph!
============================


Breakpoint 1, 0x0000555555400938 in main ()
(gdb) j *(main+35)
Continuing at 0x55555540093d.
Creating key...
Finished
Printing flag:
PICOCTF{Good job keeping bus #24c43740 speeding along!}
[Inferior 1 (process 29330) exited normally]
(gdb) 

```