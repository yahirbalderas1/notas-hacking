# Solucion
``
```
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial2/Eavesdrop]
└─$ wireshark capture.flag.pcap                                                
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial2/Eavesdrop]
└─$ openssl des3 -d -salt -in file2.des3 -out file.txt -k supersecretpassword123
*** WARNING : deprecated key derivation used.
Using -iter or -pbkdf2 would be better.
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial2/Eavesdrop]
└─$ cat file.txt                                                                
picoCTF{nc_73115_411_0ee7267a}                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial2/Eavesdrop]
└─$ 

```
