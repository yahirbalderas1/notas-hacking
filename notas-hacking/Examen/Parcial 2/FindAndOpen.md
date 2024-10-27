# Solucion
```
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial2/findandopen]
└─$ ls
dump.pcap  flag.zip
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial2/findandopen]
└─$ wireshark dump.pcap                               
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial2/findandopen]
└─$ unzip flag.zip                        
Archive:  flag.zip
[flag.zip] flag password: 
password incorrect--reenter: 
 extracting: flag                    
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial2/findandopen]
└─$ ls
dump.pcap  flag  flag.zip
                                                                                                                                                                                                   
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial2/findandopen]
└─$ cat flag    
picoCTF{R34DING_LOKd_fil56_succ3ss_5ed3a878}
                                                  

```
Al abrir el wireshark exploramos el archivo y extraemos los datos
Nos metemos a cyberchef y traducimos de hexadecimal y base64, ahi sera nuestra contrasenia para extrarer el zip y nos dara la bandera
