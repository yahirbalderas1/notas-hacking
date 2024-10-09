## Objetivo

## Solucion
──(kali㉿kali)-[~/Downloads]
└─$ cd base_images 
┌──(kali㉿kali)-[~/Downloads/base_images]
└─$ unzip 2_c.jpg  
Archive:  2_c.jpg
warning [2_c.jpg]:  187707 extra bytes at beginning or within zipfile
  (attempting to process anyway)
  inflating: base_images/3_c.jpg     
┌──(kali㉿kali)-[~/Downloads/base_images]
└─$ ls
2_c.jpg  base_images
┌──(kali㉿kali)-[~/Downloads/base_images]
└─$ cd base_images 

┌──(kali㉿kali)-[~/Downloads/base_images/base_images]
└─$ unzip 3_c.jpg 
Archive:  3_c.jpg
warning [3_c.jpg]:  123606 extra bytes at beginning or within zipfile
  (attempting to process anyway)
  inflating: base_images/4_c.jpg     
  
┌──(kali㉿kali)-[~/Downloads/base_images/base_images]
└─$ cd base_images 

┌──(kali㉿kali)-[~/Downloads/base_images/base_images/base_images]
└─$ unzip 4_c.jpg 
Archive:  4_c.jpg
warning [4_c.jpg]:  79578 extra bytes at beginning or within zipfile
  (attempting to process anyway)
  inflating: flag.txt                
┌──(kali㉿kali)-[~/Downloads/base_images/base_images/base_images]
└─$ ls
4_c.jpg  flag.txt
┌──(kali㉿kali)-[~/Downloads/base_images/base_images/base_images]
└─$ cat flag.txt  
picoCTF{4cf7ac000c3fb0fa96fb92722ffb2a32}       

## Notas adicionales

## Referencias