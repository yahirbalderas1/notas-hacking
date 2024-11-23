```
┌──(kali㉿kali)-[~/picoCTFretos/e3/transformation]
└─$ cat enc          
灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸彤㔲挶戹㍽                                                                             
┌──(kali㉿kali)-[~/picoCTFretos/e3/transformation]
└─$ python 
Python 3.12.6 (main, Sep  7 2024, 14:20:15) [GCC 14.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> enc = open("enc").read()
>>> enc
'灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸彤㔲挶戹㍽'
>>> print(hex(ord(enc[0])))
0x7069
>>> for c in enc:
...     print(hex(ord(c)).lstrip("0x"), end='')
... 
7069636f4354467b31365f626974735f696e73743334645f6f665f385f64353263366239337d>>> 
```
