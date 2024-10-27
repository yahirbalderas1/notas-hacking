# Solucion 
```
┌──(kali㉿kali)-[~/Documents/picoCTF/parcial2/whireshartwoo]
└─$ tshark -nr shark2.pcapng -Y 'dns' | grep -v '8.8.8.8' | grep -v response | grep local | awk -e '{print $12}' | sed -e 's/\..*//' | base64 -d
picoCTF{dns_3xf1l_ftw_deadbeef}} 
```
