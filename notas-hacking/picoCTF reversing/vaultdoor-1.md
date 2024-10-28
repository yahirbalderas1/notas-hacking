# Solucion
```
                                                                                           
┌──(kali㉿kali)-[~/Documents/picoCTF/reversing/vault-door1]
└─$ cat flag.txt | sort | awk '{print($3)}' | tr -d "'" | tr -d "\n" 
d35cr4mbl3_tH3_cH4r4cT3r5_f6daf4;==                                                                                           
┌──(kali㉿kali)-[~/Documents/picoCTF/reversing/vault-door1]
└─$ javac VaultDoor1.java 
Picked up _JAVA_OPTIONS: -Dawt.useSystemAAFontSettings=on -Dswing.aatext=true
                                                                                           
┌──(kali㉿kali)-[~/Documents/picoCTF/reversing/vault-door1]
└─$ java VaultDoor1      
Picked up _JAVA_OPTIONS: -Dawt.useSystemAAFontSettings=on -Dswing.aatext=true
Enter vault password: picoCTF{d35cr4mbl3_tH3_cH4r4cT3r5_f6daf4}
Access granted.

```
