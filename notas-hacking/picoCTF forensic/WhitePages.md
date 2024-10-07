## Objetivo
I stopped using YellowPages and moved onto WhitePages... but [the page they gave me](https://jupiter.challenges.picoctf.org/static/fa4a277cfa846e07a5981d8a19288a2e/whitepages.txt) is all blank!

## Solucion
┌──(kali㉿kali)-[~/Documents/picoCTF]
└─$ sed "s/\xe2\x80\x83/0/g" whitepages.txt | sed "s/\x20/1/g"
 
## Notas adicionales

## Referencias